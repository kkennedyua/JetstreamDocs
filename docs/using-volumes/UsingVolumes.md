# Using Volumes

## About volumes

A volume is a type of virtual hard drive storage for data. It is the most useful mechanism for managing large data files. For a more in-depth explanation of volumes and large data sets in Atmosphere, see Ask iPlant [Importing files to use in Atmosphere](http://ask.iplantcollaborative.org/question/326/importing-files-from-your-pc-to-use-on-atmosphere/).

Each volume is tied to a specific **project (NEED LINK)**. You can attach a volume to one or more running instances.

After you are finished using the instance, you can save your data and then unmount and detach the volume for later use, or you can delete the volume. You also can **back up and restore (NEED LINK)** your data to the Data Store.

You can use iRODS for volumes. Volumes are local-based and somewhat more volatile than network-based iRODS. For more information on using iRODS, please go to **Storing and Accessing Your Data in the Data Store (NEED LINK)**.

## Before you begin

Before you begin, you may want to google **_man page on mount_** for more information on mounting file systems on devices.

You also may want to watch a YouTube  [video](http://www.youtube.com/watch?v=y_9O6ld0bHc) about interactions with volumes.

# Creating a volume

1 Click **Projects** on the menu bar and then click the project to which you want to add a volume.
2. Click **New** and then click **Volume**.
3. In the Create Volume form:
  1. Enter the name of the volume.
  2. Select the size of the volume, up to your allotted quota.
  For larger volumes, consider using **iRODS|DS:Storing and Accessing Your Data in the Data Store (NEED LINK)**, or you can [contact iPlant Support|mailto:support@iplantcollaborative.org] to create a larger volume.
  3. Select the **provider (NEED LINK)** to use for the volume.
  4. Review the projected usage with the selected settings and adjust as needed.
  5. Click **Create volume**. The volume is added to the project. When the status shows as Unattached you can **attach it to an instance (NEED LINK)**. **Be patient:** Larger volumes may take some time to create; you may need to click !RefreshBtn.png|border=1!.

  If you have a problem, you can **report a broken volume (NEED LINK)**.

# Attaching a volume to an instance

You can attach a volume to an instance that exists in the same project.

This procedure assumes you have already created the volume, as outlined in the previous section, and it is in a status of Unattached.

1. Click **Projects** on the menu bar and then click the project with the instance to which you want to attach a new volume (the status must be Unattached).
2. Click the unattached volume name to open the volume.
3. In the Actions list on the right, click **Attach**.
4 In the Attach Volume window:
  1. Select the instance to which you want to attach the volume.
  2. Click **Attach volume to instance**. The status changes to _attaching_ and then to _Attached to <instance>_. (You may need to refresh your browser window to update the status.) The file system is created and mounted.

## Granting user write access to a volume

1. Open a terminal window.
2. Change permissions on the mounted volume:
{code}sudo chown myusername /mydata{code}
where _myusername_ is your iPlant username, and _mydata_ is the name of your mounted volume.
3.Enter your iPlant password.

# Unmounting an attached volume from an instance

You can detach a volume that is attached to an instance. Before you detach the volume, however, you must first save all your data to the Data Store or you risk losing the data.

## Step 1: **Save your data (NEED LINK)**

## Step 2: Detach the volume from the instance
1. Open the Resources window by clicking **Projects** and then clicking the project with the volume to detach.
2. In the Volumes section, click the checkbox for the volume to detach.
3 Click !VolumeDetachIcon.jpg|border=1! at the top right.
4. Click **yes** to the warning prompt.
The volume's status changes to Unattached.

After you have detached the volume from the instance, you can **delete (NEED LINK)** the instance.

# Viewing and managing volumes

You can view the list of images and volumes in a project. From that list, you can then view details about each volume and take action on them.

You can attach, detach, and delete one or more attached to any instance in the same project. You also can view details about its status, size, provider, and ID, and submit an issue report on the volume.

1. Open the Project Resources window
  1. Click **Projects** at the top and then click the project with the volume to view.
2. To view volume details, click the checkbox for the volume to view its Details pane:
  * **Status:** Current status of this volume.
  * **Size:** Current allocated size for the volume.
  * **Provider:** The **provider (NEED LINK)** selected for the volume.
  * **ID:** Unique identifier assigned to this volume.

## Detaching, attaching, and deleting a volume

1. Click an icon at the top right:
!VolumeDetachIcon.jpg|border=1! [Detach|atmman:Detaching a Volume from an Instance (Atmo-Beta)]: Available when the volume is attached.
!VolumeAttachIcon.jpg|border=1,width=19,height=19! [Attach|atmman:Attaching a Volume to an Instance (Atmo-Beta)]: Available when the volume is unattached.
!InstanceDeleteIcon.jpg|border=1,width=19,height=19! [Delete|atmman:Suspend and Resume, Stop and Start, Delete Instances (Atmo-Beta)#Deleting_an_instance]: Delete an unattached volume.

## Moving a detached volume to a different project

You can move a volume that has been detached from its instance.

1. **Save the data (NEED LINK)** to the Data Store.
2. On the Projects page, click to open the project with the volume to move and then click the checkbox for the instance.
3. If the volume is attached to an instance, **detach (NEED LINK)** the volume from all instances.
4. Click the checkbox for the volume to move.
5. Click !MoveSelectedResourceIcon.png|border=1,width=19,height=19! (Move selected resources).
6. In the Move Resources window, select the project to which you want to move the volume.
7. Click **Move resources**.

## Renaming a volume

1. Click the volume name to open the volume.
2. Hover over the name until a pencil icon is displayed to the right of the name:
!RenameVolume.jpg|border=1!
3. Click the pencil icon.
4. Edit the name and press **return**.


## Backing up data from an instance to the Data Store

1. To start the backup process, execute the following in a terminal window under your iPlant account:
{code}
$iplant_backup{code}
2. In the first prompt, enter **backup**.
3. In the second prompt asking you to specify the full path of the instance, enter the **full path to your local directory or file for the instance**.
4. In the third prompt asking you specify the path on the Data Store, enter the full path of the directory or file in the Data Store to which you want to back up the data.
The default option for this step is **/iplant/home/<username>/atmosphere**. If the **atmosphere** directory does not exist, it will be created and the data will be stored there.
5. Enter your iPlant paswword to begin the backup request.

## Restoring data from the Data Store to an instance

1. To start the restore process, execute the following in a terminal window under your iPlant account:
{code}$iplant_backup{code}
2. In the prompt asking if you want to back up or restore the data, enter **restore**.
3 In the prompt asking you to specify the path on the Data Store, enter the full path of the directory or file in the Data Store to which you want to restore the data.
4. In the prompt asking you to specify the local path on the instance, enter the full path to your local directory or file for the instance.
5. Enter your iPlant password to begin the restore process.

## Deleting a volume from a project

If you no longer want a volume, you can delete it from its project.

**Warning:** Each volume lives only in one project, so removing it destroys all changes you made to it while working on the project. You can move the volume to a different project.

1. On the Projects page, click to open the project with the volume to remove.
2.  Click the checkbox next to the volume.
3.  Click !InstanceDeleteIcon.jpg|border=1,width=19,height=19!  (Delete selected resources).
4. Click **yes** to the warning prompt.


# About inactive volumes

**Volumes that have not been used for more than three (3) months will be considered inactive.**

Once marked as inactive, the data is copied to the user's Data Store home directory (under /iplant/home/username/atmo/volume-name) and the volume is deleted.  
You can request a new volume and copy your data back to the new volume. iPlant Staff are available to assist with restoring data to the new volume, if necessary. For more information, see the iPlant [Service Level Agreement](http://www.iplantcollaborative.org/node/1933).

For more information about volumes, see[Using Volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Volumes "Using Volumes").

## Next steps

Next, you may want to [attach an instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance "Attaching a Volume to an Instance") to the volume.
