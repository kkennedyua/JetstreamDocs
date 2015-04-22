# Using Images and Instances

An **_image_** is a kind of template for an_instance_. It runs on a virtual machine (_VM_) that is already installed with a specific operating system, software, and configuration for use with that setup.

An **_instance_**, in the Atmosphere world, is a VM image that has been launched. Each instance is a specific VM, existing on a physical compute node, with its own dedicated RAM, CPUs, and disk space.

You use an instance in Atmosphere just as you use a physical computer for most tasks. Once you have selected the image to use, you launch an instance of the image.

You can view details about and manage your instances, including suspending and resuming, stopping and starting, and deleting an instance.

You also can view and access your Atmosphere instances using **Web Shell or Remote Desktop (NEED LINK)**.

You can **attach and detach one or more volumes (NEED LINK)** in the same project to the same instance, and view metrics about how your resources (memory, disk space, CPU, and AU usage) are being used on this instance.

# Managing your instances

## Launch an instance

You can launch instances either from the Projects screen or from the Images screen.

### Launching from the Projects screen

1.  Click **Projects** on the top toolbar and then click to open the project from which you want to launch the instance.
    *   To create a new project, see Using Projects **NEED LINK**.
2.  Click **New** and then click **Instance**.
  1.  In the Select Image screen, either click in the search field at the top and enter the image name, tag (**NEED LINK**), description, or OS.
  2.  Click the image to use.
3.  In the Review Image window, click **Configure**.
4.  In the Configure Image window:
  1.  Enter the name for the instance.
  2.  Select the version of the image to use.
  3.  Select the **provider (NEED LINK) to use.
  4.  Select the instance **size (NEED LINK)**.  
        The size you may choose depends on the amount of resources that will be used by the image and your resource availability. Start with the smallest size until you know for certain what size you need for that image.
    5.  Click **Launch Instance**.
    The instance is added to the project's Instances list and you can view its status as it is being launched. Once the status is Active you may begin using it.
    It may take up to 30 minutes for the instance to be accessible. Click![] **NEED IMAGE** to see if your instance status has changed to Active.  
    You will receive an email with the instance ID and IP address once the instance is in active status.

### Launching from the Images screen

1.  Click **Images** on the menu bar.
2.  To search for an image, click in the search field at the top, and enter the image name, tag (displayed in green under the image name), description, or OS.
3.  Click the image name to use.
4.  In the image window, click **Launch**.
5.  In the instance form:
    1.  Enter the name for the instance.
    2.  Select the version of the image to use.
    3.  Select the provider **(NEED LINK**) to use.
    4.  Select the instance size.  
        The size you may choose depends on the amount of resources that will be used by the image and your resource availability.
        Start with the smallest size until you know for certain what size you need for that image.
    5.  Click **Launch Instance**. The instance is added to the project's Instances list and you can view its status as it is being launched. Once the status is Active you may begin using it.

    It may take up to 30 minutes for the instance to be accessible. Click **REFRESH (NEED IMAGE)**  to see if your instance status has changed to Active.  
    You will receive an email with the instance ID and IP address once the instance is in active status.

To request that your instance be made into an image to reuse and share, or to add code to the instance before it is imaged that executes a script that runs after the image is booted, see **Request an Image of Your Instance (NEED LINK)**.

### Suspend, resume, stop, and delete an instance

You can suspend, resume, stop, or delete an instance.

1.  Click an icon at the top right:
    * **SUSPEND ICON (NEED IMAGE)**: Available when the instance is active.  
    * **RESUME ICON (NEED IMAGE)**: Available when the instance is suspended.  
    * **STOP ICON (NEED IMAGE):** Available when the instance is active or suspended.  
    * **SHUTOFF ICON (NEED IMAGE):** Available when the instance is active, suspended, or shutoff (deleted). Status will display as _shutoff_.

### Rename an instance

1.  If necessary, click the instance name to open the instance.
2.  Hover over the name until a pencil icon is displayed to the right of the name:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090410/RenameInstance.jpg?version=1&modificationDate=1425341463000)
3.  Click the pencil icon.
4.  Edit the name and press Return.

## Using Favorite images

You can create and manage your list of favorite images. Favorite images have a yellow star on the right side of the image.

1. To view your Favorites list, click **Images** and then click **Favorites**.
2. To add a favorite:
  1.  Find the image to add by scrolling through the list, or search for the image by entering the image name, tag, or description in the search field.
  2.  Click ![] (https://pods.iplantcollaborative.org/wiki/download/attachments/12225026/FavoriteImages-StarIcon.gif?version=1&modificationDate=1406915420000) on the right side of the image.  
    The image is added to your Favorites list with a yellow star:![](https://pods.iplantcollaborative.org/wiki/download/attachments/12225026/FavoriteImages-StarIconSelected.gif?version=1&modificationDate=1406915420000)
3. To remove an image from your list, click the yellow star on the right side of the image in your Favorites list.


## Viewing instance details

After an instance is active, you can view information about it, including the IP address of the image, the IDs for the instance and its parent image (its _Based on Image_), and the date you launched the image. Also displayed are its status and any tags that have been applied to the instance.

1.  If necessary, **log in to Atmosphere (NEED LINK)**.
2.  Click **Projects** at the top.
3.  Click the project with the instance to view.
4.  Click the checkbox for the instance to view its Details panel on the right (the same details are available when the instance is opened by clicking its checkbox):
    *   **ID:** Unique identifier assigned to this instance.
    *   **Status:** Current status of this instance.
    *   **Size:** Amount of CPUs, memory, and disk size used by the instance.
    *   **IP Address:** Assigned IP address, used to log in via **SSH window (NEED LINK)**
    *   **Launched:** Date the instance was launched. **NEED LINK**
    *   **Based on:** Image that was selected when the instance was launched.
     **Provider: (NEED LINK)** to which the instance is located.

## About instance metrics

Each instance provides details, such as the CPU load, RAM, and used disk space.

*   **My Resource Usage** at the top of the screen shows how much of your quota in CPUs and GB of memory is being used by your running instances. When selecting a new instance to launch, the resource usage reflects how much resources will be allocated according to the selected instance size. You can reuse your resources only after the instance has been terminated and is no longer displayed in the My Instances list. For more information on allocations, see [Allocation Policies](https://pods.iplantcollaborative.org/wiki/display/atmman/Allocation+Policies "Allocation Policies").

*   **Instance Details** tab displays important information about the instance, including the ID assigned to the instance when it was launched, name of the image it is using, unique EMI ID, the instance size, the date you launched the image, and the IP address, which you will need when[logging in](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+an+Instance "Logging In to an Instance") to the instance.

*   **Instance Metrics** allows you to drill down into the usage expended for the running image, including percentage used for RAM and used disk space, and CPU load. Not all images provide instance metrics.

## Add tags

You can add tags to a running instance to help you find it more easily in search.

1.  If necessary, open the running instance.
2.  On the Instance Details tab, click the**Edit Tags** icon.
3.  In the text field, enter the tag to add and click**Add**:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/8411419/Tags-1.png?version=1&modificationDate=1369083148000)
4.  Repeat for each additional instance tag to add.
5.  When done, click**Done**.

## Have a problem?

Here's how to report a problem with an instance, image, or volume **(NEED LINK)**.
