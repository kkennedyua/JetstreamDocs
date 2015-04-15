<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>

This page contains:

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div>
# About viewing and managing your Atmosphere instances

You can view the list of resources —[images](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Instances "Using Instances") and[volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Volumes+%28Atmo-Beta%29 "Using Volumes (Atmo-Beta)")— in a project. From that list, you can then view details about each instance and take action on them, such as suspending and resuming, stopping and starting, and deleting an instance.

You also can view and access your Atmosphere instances using[Web Shell or Remote Desktop](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+an+Instance+Through+the+Web+Shell+or+Via+Remote+Desktop+%28Atmo-Beta%29 "Logging In to an Instance Through the Web Shell or Via Remote Desktop (Atmo-Beta)").

After an instance is active, you can view information about it, including the IP address of the image, the IDs for the instance and its parent image (_Based on Image_), and the date you launched the image. Also displayed are any tags, as well as the status of the instance.

You can[attach and detach one or more volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Viewing+and+Managing+Volumes+%28Atmo-Beta%29 "Viewing and Managing Volumes (Atmo-Beta)")in the same project to the same instance, and view metrics about how your resources (memory, disk space, CPU, and AU usage) are being used on this instance.

# Open the Project Resources window

1.  If necessary,[log in to Atmosphere](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+and+Signing+Out+of+Atmosphere+%28Atmo-Beta%29 "Logging In to and Signing Out of Atmosphere (Atmo-Beta)").
2.  Click**Projects** at the top and then click the project with the instance to view.

# Viewing instance details

1.  Click the checkbox for the instance to view its Details panel:
    *   **ID:** Unique identifier assigned to this instance.
    *   **Status:** Current status of this instance.
    *   **Size:** Amount of CPUs, memory, and disk size used by the instance.
    *   **IP Address:** Assigned IP address. Use this to log in via[SSH window](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+an+Instance+Through+the+Web+Shell+or+Via+Remote+Desktop+%28Atmo-Beta%29 "Logging In to an Instance Through the Web Shell or Via Remote Desktop (Atmo-Beta)").
    *   **Launched:** Date the instance was launched.
    *   **Based on:** *mage upon which this instance was based.
    *   **Provider:**[Provider](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Providers+%28Atmo-Beta%29 "Using Providers (Atmo-Beta)") selected for the instance.

# Performing actions on an instance

## Suspending, resuming, stopping, and deleting an instance

1.  Click an icon at the top right:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090410/InstanceSuspendIcon.jpg?version=1&modificationDate=1424815166000)[Suspend](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspend+and+Resume%2C+Stop+and+Start%2C+Delete+Instances+%28Atmo-Beta%29#SuspendandResume%2CStopandStart%2CDeleteInstances%28Atmo-Beta%29-Suspendinganinstance): Available when the instance is active.  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090410/InstanceResumeIcon.jpg?version=1&modificationDate=1424815278000)[Resume](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspend+and+Resume%2C+Stop+and+Start%2C+Delete+Instances+%28Atmo-Beta%29#SuspendandResume%2CStopandStart%2CDeleteInstances%28Atmo-Beta%29-Resuminganinstance): Available when the instance is suspended.  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090410/InstanceStopIcon.jpg?version=1&modificationDate=1424815377000)[Stop](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspend+and+Resume%2C+Stop+and+Start%2C+Delete+Instances+%28Atmo-Beta%29#SuspendandResume%2CStopandStart%2CDeleteInstances%28Atmo-Beta%29-Stoppinganinstance): Available when the instance is active or suspended.  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090410/InstanceDeleteIcon.jpg?version=1&modificationDate=1424815435000)[Delete](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspend+and+Resume%2C+Stop+and+Start%2C+Delete+Instances+%28Atmo-Beta%29#SuspendandResume%2CStopandStart%2CDeleteInstances%28Atmo-Beta%29-Deletinganinstance): Status will display as_shutoff_. Available when the instance is active, suspended, or shutoff (deleted).

## Renaming an instance

1.  If necessary, click the instance name to open the instance.
2.  Hover over the name until a pencil icon is displayed to the right of the name:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090410/RenameInstance.jpg?version=1&modificationDate=1425341463000)
3.  Click the pencil icon.
4.  Edit the name and press Return.

# See also

*   [Viewing and Managing Volumes (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Viewing+and+Managing+Volumes+%28Atmo-Beta%29 "Viewing and Managing Volumes (Atmo-Beta)")  

*   [Using Instances (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Instances+%28Atmo-Beta%29 "Using Instances (Atmo-Beta)")  

*   [Reporting an Issue with a Project, Instance, or Volume](https://pods.iplantcollaborative.org/wiki/display/atmman/Reporting+an+Issue+with+a+Project%2C+Instance%2C+or+Volume "Reporting an Issue with a Project, Instance, or Volume")  

*   [Requesting an Image of an Instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Requesting+an+Image+of+an+Instance "Requesting an Image of an Instance")  

*   [Rebooting an Instance (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Rebooting+an+Instance+%28Atmo-Beta%29 "Rebooting an Instance (Atmo-Beta)")  

*   [Logging In to an Instance Through the Web Shell or Via Remote Desktop (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+an+Instance+Through+the+Web+Shell+or+Via+Remote+Desktop+%28Atmo-Beta%29 "Logging In to an Instance Through the Web Shell or Via Remote Desktop (Atmo-Beta)")  

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoFeedbackSupport}</div></div>