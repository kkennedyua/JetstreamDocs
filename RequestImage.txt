This page contains:

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=1}</div></div>
# About requesting an image of an instance

An image is a type of template for a virtual machine. You may request an image of your running instance, which helps you retain a complete copy of all changes and updates you made to the instance since launching it from its image. Images also save resources, since you can launch an instance of it at any time instead of keeping the instance running when you don't need to use it.

To request an image of an instance, simply complete the Request Imaging form within Atmosphere Airport.

After submitting your form, the Atmosphere support staff completes the request. Future versions of Atmosphere will allow users to initiate the VM imaging process automatically.

For a basic introduction to instances and images, see[Using Instances](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Instances "Using Instances").

**Before you begin, read the Important notes section.**

## Executing scripts that run after an Atmosphere image is booted

An image creator can add a script to the instance before it is converted to an image that will execute after the Atmosphere image is launched and active.

*   To do so, create or symlink the script into the**/etc/atmo/post-scripts.d** directory.
*   The first line of the script must be<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">#!/bin/bash</pre></div></div></div>
*   The folder and script both must be marked with read and write (**+rx** or**0755**) permissions.

After the image is launched and active, the script will be executed.

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{section}</div><div class="wysiwyg-macro-body"><div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{column:width=60%}</div><div class="wysiwyg-macro-body">
## Requesting an image

The Request Imaging form provides the necessary information for creation of the VM machine image by the Atmosphere support staff.

1.  **Before you begin, remove any non-iPlant-purchased licensed software, or non-cloud-compatible software, per the instructions in the Important notes section to the right.**
2.  If necessary,[log in](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+Atmosphere "Logging In to Atmosphere") to Atmosphere.
3.  [Detach all attached volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance#AttachingaVolumetoanInstance-VolumeUnmountDetach) from the instance.
4.  If necessary,[launch](https://pods.iplantcollaborative.org/wiki/display/atmman/Launching+a+New+Instance "Launching a New Instance") the instance. The instance must be running in order to create the image.
5.  In your**My Instances** list, click to open the instance you want to save to an image.
6.  On the Instance Details tab, click the**Image** button.
7.  On the Request Imaging form, enter the necessary information:
    *   **Image Name**: Enter the name, up to 30 characters, to assign to the machine image.  
        Instance ID and IP Address are the non-editable assigned ID and current IP address of the instance.
    *   **Cloud for Deployment:** Currently only iPlant Cloud-Tucson is available.
    *   **Description of the Image:** Enter the description of the machine image as it will appear in Atmosphere. The description should concisely describe the tools installed, the purpose of the tools (e.g.,_This image performs X analysis_), and the initial intent of the machine image (e.g.,_designed for XYZ workshop_).
    *   **List Installed Software:** Enter the name of all software applications that you have installed and the paths to the executables, if different from**/usr/bin** or**/usr/local/bin**.
    *   **iPlant-managed System Files**: If your machine image requires a change in an iPlant-managed system file (see Important Notes to the right), enter the specifics for the change and why the change is necessary.
    *   **Files to exclude:** List all files you do not want included in the image, one path per line.
    *   **Image Tags**: (Optional) Click**Edit Tags** to enter tags that will enhance search results for this image.
    *   **Image Visibility:** Defines whether you want the image visibility to be Public (visible and launchable by any user), Private (visible and launchable only by you), or Specific Users (visible and launchable only by specified iPlant users). If you want to share the image with a specific user or users (restricted visibility),[email Support](mailto:support@iplantcollaborative.org) with a list of the iPlant user names, or submit[an online request](http://www.iplantcollaborative.org/forms/support).
    *   **Certification checkbox:** Click to acknowledge that the image contains no license-restricted software that is prohibited from distribution within a virtual or cloud environment.
8.  Click**Request Imaging**.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{warning}</div><div class="wysiwyg-macro-body">

    Do not suspend or stop the instance until you receive notification that the image has been created.

    </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{warning}</div></div>

You will receive an email when the image is being processed and again when it has been completed. Please email questions to[Atmosphere Support](mailto:support@iplantcollaborative.org).

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{hidden-data}</div><div class="wysiwyg-macro-body">

Process from[https://pods.iplantcollaborative.org/wiki/display/csmgmt/SOP+for+dealing+with+imaging+requests](https://pods.iplantcollaborative.org/wiki/display/csmgmt/SOP+for+dealing+with+imaging+requests)  

</div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{hidden-data}</div></div></div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{column}</div></div><div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{column:width=40%}</div><div class="wysiwyg-macro-body"><div class="wysiwyg-macro"><div class="panel" style="border-width: 1px;"><div class="panelContent">
### <span style="color: rgb(255, 0, 0);">Important notes before you request an image</span>

**Before requesting creation of a machine image, you must remove the following software from the instance:**

*   Licensed software that was not purchased by iPlant.
*   Software in which the licensing otherwise prevents the use within a cloud or virtualized environment.

**The following directories are DELETED as part of the imaging process:**

*   /home/<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{note}</div><div class="wysiwyg-macro-body">

    All files, directories, and icons located under**/home/<username>/Desktop** will be deleted. To preserve them, please email[iPlant Support](mailto:support@iplantcollaborative.org).  

    Any files installed in /home**must** be saved to your volume, iRODS, or to another storage external to your VM.

    </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{note}</div></div>
*   /mnt/
*   /tmp/
*   /root/

**The following are NOT COPIED as part of the image:**

*   Volumes
*   iRODS FUSE mounts

**The following system files are typically OVERWRITTEN by iPlant for security or operational reasons when the instance is launched:**

*   /etc/fstab
*   /etc/group
*   /etc/host.allow
*   /etc/host.conf
*   /etc/host.deny
*   /etc/hosts
*   /etc/ldap.conf
*   /etc/passwd
*   /etc/resolve.conf
*   /etc/shadow
*   /etc/sshd/
*   /etc/sysconfig/iptables
*   /root/
*   /var/log

</div></div></div></div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{column}</div></div></div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{section}</div></div>