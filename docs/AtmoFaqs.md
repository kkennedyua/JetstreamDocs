<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>
# About Atmosphere FAQs

This page contains a list of frequently asked questions about Atmosphere. You may also want to go to[Ask iPlant](http://ask.iplantcollaborative.org/questions/scope:all/sort:activity-desc/tags:Atmosphere/page:1/) for answers to questions from other users about Atmosphere.

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div>
## Troubleshooting

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:TroubleshootVolume}</div></div>
# Volumes

*   ## Volume isn't working

    1.  Check to make sure that you[mounted the volume](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance#AttachingaVolumetoanInstance-VolumeAttach).
    2.  If that doesn't fix the problem, it is possible that you[terminated the instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance#AttachingaVolumetoanInstance-VolumeTerminateInstance) before[unmounting and detaching it](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance#AttachingaVolumetoanInstance-VolumeUnmountDetach).
    3.  Read through the questions and answers on this page.
    4.  If you don't find an answer to your volume problem, you can[report the problem](https://pods.iplantcollaborative.org/wiki/display/atmman/Reporting+a+Volume+Problem "Reporting a Volume Problem").  
        _For more information about volumes, see__[Using Volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Volumes "Using Volumes")_.

*   ## Volume lost its data

    There are several reasons why data might not appear in a volume as expected:

    *   **The volume was created with a partition:** Although partitions are not required, some users prefer to format their volume with a partition. It is sometimes easy to forget that your volume was created with a partition. If your volume was created with a partition, you need to mount it with a**1**, e.g., "mount /dev/xvdb1 /mydata".
    *   **The volume has a different file system than expected:** The default mkfs command and the instructions provided by the Atmosphere documentation use ext2\. Advanced users may opt to format the volume as a different file system. If you choose a different file system, please remember the file system you created for your volume.
    *   **The volume is corrupted:** Corrupted volumes can occur when data is being written to the volume at the same time as an instance is being terminated. We highly recommend unmounting the volume before the termination of an instance for this very reason. The chances are low for recovery.
    *   **The volume was accidentally reformatted:** You should execute the**mkfs** command**only once per volume** unless you intend to erase the existing data on that volume. There is no possibility of recovery in this situation.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{warning}</div><div class="wysiwyg-macro-body">

        Users are encouraged to back up any important data stored in instances and volumes to the Data Store using iCommands, FUSE, or iDrop.

        </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{warning}</div></div>

*   ## Volume has been suspended but didn't suspend it

    An instance that has not performed significant computations measured by load average or have not had interactive sessions (via SSH or VNC) for more than three (3) days may be[suspended](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspending+and+Resuming+an+Instance "Suspending and Resuming an Instance"), which preserves the state but frees the resources. You may resume a suspended instance at a later time, depending on available resources.

*   ## Volume is missing and need to find its data

    If you haven't accessed a volume within three (3) months, your volume may have been backed up to your iPlant Data Store and the cloud storage reclaimed. The default location for volume backups is**/iplant/home/username/atmo/vol-XXXXXX**, where "username" is your iPlant username and "vol-XXXXXX" was the original volume ID within Atmosphere. You can request a new volume and then copy your data back to the new volume. iPlant Staff will be available to assist with restoring data to the new volume, if necessary.

# Instances

_For more information about instances, see__[Using Instances](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Instances "Using Instances")_.

*   ## Instance isn't working

    1.  Read through the other questions and answers on this page.
    2.  If you don't find an answer to your instance problem, you can[report the problem](https://pods.iplantcollaborative.org/wiki/display/atmman/Reporting+a+Broken+Instance "Reporting a Broken Instance").<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:NoAirportShell}</div></div>

*   ## Can't open Shell tab for instance

    If**Shell Unavailable** is displayed, check the following:  

    *   **The instance is not in Active status:** The instance may be unavailable because it is not in Active status or has been terminated or suspended.  
        Solution: If the instance is not in Active status, you must wait until it is active. You may need to click![](https://pods.iplantcollaborative.org/wiki/images/icons/attachments/image.gif) in the My Instances list to refresh the status.  

    *   **The instance failed to launch.**  
        Solution:[Terminate](https://pods.iplantcollaborative.org/wiki/display/atmman/Terminating+an+Instance "Terminating an Instance") the instance and[launch a new one](https://pods.iplantcollaborative.org/wiki/display/atmman/Launching+a+New+Instance "Launching a New Instance").
    *   **The instance does not support Airport Shell:** The instance may be based on an old image that doesn't support Web shell or the provider may not provide it for the instance.  
        Solution: Search for a newer version of the image.[Connect using SSH or PuTTY](https://pods.iplantcollaborative.org/wiki/x/Oqxm).  
        _For more information on using the Airport Shell tab, see__[Logging In to an Instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+an+Instance "Logging In to an Instance")_.  

*   ## Active instance lost connectivity and need to recover networking

    On rare occasions, an instance may lose connectivity after maintenance periods. Suspending and then resuming the instance should help restore the instance's networking. A short screencast to suspend and resume an instance can be found here:[https://vimeo.com/100855170](https://vimeo.com/100855170).

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:NoVNC}</div></div>
*   ## VNC issues

    *   ### Can't open VNC tab for instance

        If**VNC Unavailable** is displayed, check the following:

        *   **Instance status is not Active:** The instance may be unavailable because it is not in a status of Active or has been terminated.
            1.  Wait until the instance is running. You may need to click![](https://pods.iplantcollaborative.org/wiki/images/icons/attachments/image.gif) to update the status.
            2.  If you want to use the VNC tab for the instance, you may need to[launch a new instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Launching+a+New+Instance "Launching a New Instance").
        *   **Instance failed to launch**
            1.  [Terminate](https://pods.iplantcollaborative.org/wiki/display/atmman/Terminating+an+Instance "Terminating an Instance") the instance.
            2.  [launch a new one](https://pods.iplantcollaborative.org/wiki/display/atmman/Launching+a+New+Instance "Launching a New Instance").
        *   **Instance does not provide a desktop interface**
            1.  [Connect using SSH or PuTTY](https://pods.iplantcollaborative.org/wiki/x/Oqxm).
        *   **Need to find images tagged with VNC**
            1.  Click**Launch New Instance**.
            2.  In the search field, enter**vnc** and then click the image to use.  
                _For more information on the VNC tab, see__[Using VNC Viewer to Connect to an Atmosphere VM](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+VNC+Viewer+to+Connect+to+an+Atmosphere+VM "Using VNC Viewer to Connect to an Atmosphere VM")__in the Atmosphere Wiki manual_.<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:VNCNotWorkingProperly}</div></div>
    *   ### No desktop, or used to work but doesn't now

        Either the VNC connects but displays no desktop OR the resumed instance's VNC session used to work (e.g. before suspending), but does not work now.  
        We have seen some cases where the VNC remote desktop session is not fully functional, although the VNC remote viewer and Web-based VNC viewer connect properly. Also, when suspended instances are resumed, the instance's IP address may change, causing the VNC server to fail; in this situation, the VNC remote desktop server session will need to be restarted.

        *   **Workaround:**
            1.  Log in to the instance via SSH.
            2.  Sudo to root by typing:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">sudo su -</pre></div></div></div>
            3.  Kill all processes with "vnc" or "Xvnc" by typing:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">ps aux|grep vnc|grep -v grep|awk '{print $2}'|xargs kill -9</pre></div></div></div>
            4.  Exit sudo to return to your user account by typing:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">exit</pre></div></div></div>
            5.  Relaunch vncserver by typing:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">vncserver :1</pre></div></div></div>
            6.  (Optional) If you encounter errors about the existence of files, you might need to delete (i.e.,**rm**) the following files and attempt to relaunch the vncserver:
                *   <tt>/tmp/.X1-lock</tt>
                *   <tt>/tmp/.X11-unix/X1</tt>
            7.  Attempt to reconnect to VNC; if the error still persists (sometimes it takes a couple of times), repeat the steps a few times.<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:EBSVolumeMissing}</div></div>

# Information and definitions

## Images

_For more information on images, see__[Launching a New Instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Launching+a+New+Instance "Launching a New Instance")__in the Atmosphere manual._

*   ### Definition

    An_image_ is a template for an instance. Each image comes preinstalled with an operating system, custom configuration, and related software that is specific to that image.Click any image to view its description and list of installed software, and then double-click the image to launch it with default settings.

*   ### Searching for an image

    You can search images by name, description, or ID number. You also can search by tag using the syntax**tag:tag_to_find**.

## Instances

_For more information on launching and using instances, see__[Using Instances](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Instances "Using Instances")__._

*   ### Definition

    An_instance_ is a specific virtual machine (VM) that exists on a physical compute node, and which has dedicated RAM, CPUs, and disk space. You can use an instance as you would use a physical computer for most tasks.

*   ### Launching a new instance

    To launch an instance, see[Launching a New Instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Launching+a+New+Instance "Launching a New Instance").

    <div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:VolumesDef}</div></div>

*   ### Reporting an issue with an instance

    See[Reporting a Broken Instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Reporting+a+Broken+Instance "Reporting a Broken Instance").

## Volumes

_For more information about volumes, see__[Using Volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Volumes "Using Volumes")__._

*   ### Definition

    A_volume_ is like a virtual USB drive that helps you more easily transfer relatively small data between instances. You can create a volume with a capacity of up to 100 GB using the**Create a Volume**form. To store and transfer more data at once, store it in the iPlant Data Store instead. You can mount the Data Store similarly to a volume.

*   ### Availability of a volume

    A volume is "available" when it is not attached to an instance. You must have at least one running instance in order to put a volume to use. Any newly created volume must be formatted and then mounted after it has been attached before you can use it.

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{hidden-data}</div><div class="wysiwyg-macro-body">

**Atmosphere:** Newly created volumes must be formatted and then mounted after the volume has been attached before you can use it.  
Atmosphere Beta volumes are automatically formatted and mounted behind the scenes.

</div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{hidden-data}</div></div>
*   ### Reporting an issue with a volume

    See[Reporting a Volume Problem](https://pods.iplantcollaborative.org/wiki/display/atmman/Reporting+a+Volume+Problem "Reporting a Volume Problem").

## Data and Atmosphere

*   ### Importing large data files for use in Atmosphere

    See[this page](http://ask.iplantcollaborative.org/question/326/importing-files-from-your-pc-to-use-on-atmosphere/) on Ask iPlant about the best way to import files for use in Atmosphere.

## Other definitions

*   ### My Resource Usage definition

    Resource usage is determined by how many CPUs, GBs, and AUs of memory your instances are using cumulatively. You can reuse your resources only after the instance has been terminated and is no longer displayed in the My Instances list.  
    _For more information on resource usage, see__[Viewing Your Active Instances](https://pods.iplantcollaborative.org/wiki/display/atmman/Viewing+Your+Active+Instances "Viewing Your Active Instances")_ in the Atmosphere manual.

*   ### CPU hour definition

    <div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_def_CPU-hour}</div></div>

*   ### AU definition

    _AU_ stands for Atmosphere Units, the number of Atmosphere CPU hours allocated for your account. One AU is roughly equivalent to one CPU-hour, or one CPU-core used per hour.

# Other resources

*   [Ask iPlant](http://ask.iplantcollaborative.org/questions/scope:all/sort:activity-desc/tags:Atmosphere/page:1/) is a question and answer forum that is moderated by iPlant users.

*   The[Atmosphere-users mailing list](https://pods.iplantcollaborative.org/wiki/display/atmman/Subscribing+to+the+Atmosphere-Users+Mailing+List "Subscribing to the Atmosphere-Users Mailing List")gives you access to postings by the Atmosphere-users group as well as to the collection of prior postings, and the ability to post messages to the Atmosphere group.

*   The[main Frequently Asked Questions page](https://pods.iplantcollaborative.org/wiki/x/mZ5y)provides answers to more general questions about using the Discovery Environment and iPlant Data Store. You may find an answer to your question there as well.