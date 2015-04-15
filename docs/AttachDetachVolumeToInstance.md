<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>
# Attaching a volume to and detaching a volume from an instance

You can attach a volume to an instance that exists in the same project and detach a volume  that is attached to an instance.

This page contains:

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div><div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip}</div><div class="wysiwyg-macro-body">

For more information about volumes, see[Using Volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Volumes "Using Volumes").

</div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div>
# Before you begin

This procedure assumes you have already[created the volume](https://pods.iplantcollaborative.org/wiki/display/atmman/Creating+a+Volume "Creating a Volume") and it is in a status of Unattached.

# Attaching a volume to an instance

1.  Click**Projects** on the menu bar and then click the project with the instance to which you want to attach a new volume (the status must be Unattached).
2.  Click the unattached volume name to open the volume. See[Creating a Volume (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Creating+a+Volume+%28Atmo-Beta%29 "Creating a Volume (Atmo-Beta)") to create a new one for the instance.
3.  In the Actions list on the right, click**Attach**.
4.  In the Attach Volume window:
    1.  Select the instance to which you want to attach the volume.
    2.  Click**Attach volume to instance**. The status changes to**attaching** and then to**Attached to <instance>**. (You may need to refresh your browser window to update the status.)  
        The file system is created and mounted.

## Granting user write access to a volume

1.  Open a terminal window.
2.  Change permissions on the mounted volume:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">sudo chown myusername /mydata</pre></div></div></div>

    where_myusername_ is your iPlant username, and_mydata_ is the name of your mounted volume.

3.  Enter your iPlant password.

# About inactive volumes

**Volumes that have not been used for more than three (3) months will be considered inactive.**

Once marked as inactive, the data will be copied to the user's Data Store home directory (under /iplant/home/yourusername/atmo/volume-name) and the volume will be deleted.  
Users can[create a new volume](https://pods.iplantcollaborative.org/wiki/display/atmman/Creating+a+Volume "Creating a Volume") and copy their data back to the new volume.[Contact iPlant Staff](mailto:support@iplantcollaborative.org) for help restoring data to the new volume, if necessary.

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoFeedbackSupport}</div></div>

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>

# Detaching a volume from an instance

Before detaching the volume you must first unmount it.

## Unmounting an attached volume from an instance

You can detach a volume that is attached to an instance. Before you detach the volume, however, you must first save all your data to the Data Store or you risk losing the data.

### Step 1:[Save your data](https://pods.iplantcollaborative.org/wiki/display/atmman/Backing+Up+and+Restoring+Volume+Data+to+the+Data+Store+%28Atmo-Beta%29 "Backing Up and Restoring Volume Data to the Data Store (Atmo-Beta)").

### Step 2: Detach the volume from the instance

1.  Open the Resources window by clicking**Projects** and then clicking the project with the volume to detach.
2.  In the Volumes section, click the checkbox for the volume to detach.
3.  Click![](https://pods.iplantcollaborative.org/wiki/download/attachments/14583998/VolumeDetachIcon.jpg?version=1&modificationDate=1424898646000) at the top right.
4.  Click yes to the warning prompt.  
    The volume's status changes to Unattached.<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{hidden-data}</div><div class="wysiwyg-macro-body"><div class="wysiwyg-macro"><div class="panel" style="border-width: 1px;"><div class="panelContent">

    *Broken – See ATMO-694, scheduled for Doradito

    </div></div></div></div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{hidden-data}</div></div>

After you have detached the volume from the instance, you can[delete](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspend+and+Resume%2C+Stop+and+Start%2C+Delete+Instances+%28Atmo-Beta%29 "Suspend and Resume, Stop and Start, Delete Instances (Atmo-Beta)") the instance.

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{hidden-data}</div><div class="wysiwyg-macro-body"><div class="wysiwyg-macro"><div class="panel" style="border-width: 1px;"><div class="panelContent">

Cannot test this since it's broken so don't know if this still applies. Should be working per ATMO-665

</div></div></div></div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{hidden-data}</div></div>