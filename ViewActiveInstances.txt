# About viewing your active Atmosphere instances

This page contains:

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div>

You can view your Atmosphere instances in the Instance Details tab.

Other ways in which you can view and access your Atmosphere instances include:

*   [Shell](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+an+Instance#LoggingIntoanInstance-Shell): Available for login via either through an SSH window or in the Airport Shell tab.
*   [VNC](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+VNC+Viewer+to+Connect+to+an+Atmosphere+VM "Using VNC Viewer to Connect to an Atmosphere VM"): Java-based VNC client that provides instant access to the desktop of the selected instance, accessible either in the Atmosphere Airport VNC tab or via a separate VNC Viewer application.

This page describes using Airport to view your running instances.

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip:title=Want to know more about instances?}</div><div class="wysiwyg-macro-body">

See[Using Instances](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Instances "Using Instances").

</div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div><div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:ViewInstances}</div></div>
## Viewing instance details

After an instance is active, you can view information about it, including the IP address of the image, the IDs for the instance and the parent image (Based on Image), and the date you launched the image. Also displayed are tags, if any were entered when the instance was launched, as well as the status of the instance, such as whether it is pending or running.

You also can attach and detach your storage volumes to the instance, and view metrics about how your resources (memory, disk space, CPU, and AU usage) are being used on this instance.

1.  If necessary,[log in to Atmosphere](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+Atmosphere "Logging In to Atmosphere").
2.  In the**My Instances** list, click the instance to view.
3.  If necessary, click the**Instance Details** tab:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/8411419/InstanceDetails-1.png?version=1&modificationDate=1369082867000)

## Understanding instance metrics

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:ResourceUsage}</div></div>

Each instance provides details, such as the CPU load, RAM, and used disk space.

*   **My Resource Usage** at the top of the screen shows how much of your quota in CPUs and GB of memory is being used by your running instances. When selecting a new instance to launch, the resource usage reflects how much resources will be allocated according to the selected instance size. You can reuse your resources only after the instance has been terminated and is no longer displayed in the My Instances list. For more information on allocations, see[Allocation Policies](https://pods.iplantcollaborative.org/wiki/display/atmman/Allocation+Policies "Allocation Policies").

*   **Instance Details** tab displays important information about the instance, including the ID assigned to the instance when it was launched, name of the image it is using, unique EMI ID, the instance size, the date you launched the image, and the IP address, which you will need when[logging in](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+an+Instance "Logging In to an Instance") to the instance.

*   **Instance Metrics** allow you to drill down into the usage expended for the running image, including percentage used for RAM and used disk space, and CPU load. Not all images provide instance metrics.

## Adding instance tags to a running instance

You can add tags to your instance to help you find it more easily in search.

1.  If necessary, open the running instance.
2.  On the Instance Details tab, click the**Edit Tags** icon.
3.  In the text field, enter the tag to add and click**Add**:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/8411419/Tags-1.png?version=1&modificationDate=1369083148000)
4.  Repeat for each additional instance tag to add.
5.  When done, click**Done**.

You also can[add image tags](https://pods.iplantcollaborative.org/wiki/display/atmman/Request+an+Image+of+Your+Instance "Request an Image of Your Instance") when you request an image of your instance.

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip:title=Having a problem with your instance?}</div><div class="wysiwyg-macro-body">

You can[report a problem with an instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Reporting+a+Broken+Instance "Reporting a Broken Instance").

</div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div><div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoFeedbackSupport}</div></div>