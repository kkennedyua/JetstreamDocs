<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>
# Requesting an image of an instance

This page contains:

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=1}</div></div>

An image is a type of template for a virtual machine. You may request an image of your running instance. This saves a complete copy of all changes and updates you made to the instance since launching it from its image, and also saves resources by launching an instance only when you need it.

# Executing scripts that run after an Atmosphere image is booted

An image creator can add a script to an instance before it is converted to an image that will execute after the Atmosphere image is launched and active.

*   To do so, create or symlink the script into the**/etc/atmo/post-scripts.d** directory.
*   The first line of the script must be<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">#!/bin/bash</pre></div></div></div>
*   The folder and script both must be marked with read and write (**+rx** or**0755**) permissions.

After the image is launched and active, the script will be executed.

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{section}</div><div class="wysiwyg-macro-body"><div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{column:width=65%}</div><div class="wysiwyg-macro-body">
## Requesting an image

The process of requesting an image is easily done using the Request Imaging form.

1.  **Before you begin, remove any non-iPlant-purchased licensed software, or non-cloud-compatible software, per the instructions in the**<span style="color: rgb(255, 0, 0);">**Important notes**</span>**section at the right.**
2.  If necessary,[log in to Atmosphere](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+and+Signing+Out+of+Atmosphere+%28Atmo-Beta%29 "Logging In to and Signing Out of Atmosphere (Atmo-Beta)").
3.  [Detach all attached volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance#AttachingaVolumetoanInstance-VolumeUnmountDetach) from the instance.
4.  Click**Projects** on the menu bar and open the project with the instance to use for the new image.
5.  Click the instance name.
6.  In the**Actions** list on the right, click**Image**.
7.  On the Request Imaging form, enter the necessary information:
    *   **Image Name**: Enter the name, up to 30 characters, to assign to the new image.
    *   **Description of the Image:** Enter the description of the image as it will appear in Atmosphere. The description should concisely describe the tools installed, the purpose of the tools (e.g.,_This image performs X analysis_), and the initial intent of the machine image (e.g._designed for XYZ workshop_).
    *   **Image Tags**: (Optional) Click in the field and select tags that will enhance search results for this image. You can[add and remove tags](https://pods.iplantcollaborative.org/wiki/display/atmman/Adding+and+Removing+Instance+Tags+%28Atmo-Beta%29 "Adding and Removing Instance Tags (Atmo-Beta)") later, if needed.
    *   **Cloud for Deployment:** Select the cloud[provider](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Providers+%28Atmo-Beta%29 "Using Providers (Atmo-Beta)") to use for the image. The list depends on the providers to which you have been granted access.
    *   **Image Visibility:** Select the image visibility, either**Public** (visible and launchable by any user),**Private** (visible and launchable only to you), or**Specific Users**(visible and launchable only by specified iPlant users). If you want to share the image with a specific user or users (restricted visibility),[email Support](mailto:support@iplantcollaborative.org) with a list of the iPlant user names, or submit[an online request](http://www.iplantcollaborative.org/forms/support).
8.  Click**Show advanced options** to view and select more options for the image:
    *   **List Installed Software:** Enter the name of any software applications that you have installed and the paths to the executables, if different from /usr/bin or /usr/local/bin.
    *   **iPlant-managed System Files**: If your machine image requires a change in an iPlant-managed system file (see Important Notes), enter the specifics for the change and why the change is necessary.
    *   **Files to exclude:** List any files, one path per line, that you do not want included in the image.
    *   Checkbox: Click to acknowledge that the image contains no license-restricted software that is prohibited from distribution within a virtual or cloud environment.
9.  Click**Request Imaging**.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{warning}</div><div class="wysiwyg-macro-body">

    Do not stop or suspend the instance until you receive notification that the image has been created.

    </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{warning}</div></div>

You will receive an email when the image is being processed and again when it has been completed. Please email questions to[Atmosphere Support](mailto:support@iplantcollaborative.org).

# Viewing the list of your images

1.  <div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_atmo_login}</div></div>
2.  Click**Images** on the top menu bar.
3.  Click**My Images** on the top of the screen.  
    The list of your images is displayed.

</div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{column}</div></div><div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{column:width=35%}</div><div class="wysiwyg-macro-body"><div class="wysiwyg-macro"><div class="panel" style="border-width: 1px;"><div class="panelContent">
# <span style="color: rgb(255, 0, 0);">Important notes before you request an image</span>

**Before submitting your request for an image of your instance, you must remove the following software from the instance:**

*   Licensed software that was not purchased by iPlant.
*   Software in which the licensing otherwise prevents the use within a cloud or virtualized environment.

**The following directories are deleted as part of the imaging process:**

*   /home/<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{note:title=About your /home/ directory}</div><div class="wysiwyg-macro-body">
    *   All files, directories, and icons located under**/home/<username>/Desktop** will be deleted. To preserve them, please email[iPlant Support](mailto:support@iplantcollaborative.org).
    *   Any files installed in /home**must** be saved to your volume, to iRODS, or to another storage external to your VM.

    </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{note}</div></div>
*   /mnt/
*   /tmp/
*   /root/

**Volumes and iRODS FUSE mounts are not copied as part of the image.**

**The following system files are typically overwritten by iPlant for security or operational reasons:**

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