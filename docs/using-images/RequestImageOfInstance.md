# Requesting an image of an instance
===

You may request an image of your running instance. This saves a complete copy of all changes and updates you made to the instance since launching it from its image, and also saves resources by launching an instance only when you need it.

## Executing scripts that run after an Atmosphere image is booted

An image creator can add a script to an instance before it is converted to an image that will execute after the Atmosphere image is launched and active.

*   To do so, create or symlink the script into the **/etc/atmo/post-scripts.d** directory.
*   The first line of the script must be:

            #!/bin/bash
         
*   The folder and script both must be marked with read and write (**+rx** or **0755**) permissions.

After the image is launched and active, the script will be executed.

1. Before you begin, you MUST remove all licensed software that was not purchased by iPlant, and all software whose licensing otherwise prevents the use within a cloud or virtualized environment. See the IMPORTANT NOTES section (NEED LINK).
2.  If necessary, log in to Jetstream.
3.  **Detach all attached volumes (NEED LINK)** from the instance.
4.  Click **Projects** on the menu bar and open the project with the instance to use for the new image.
5.  Click the instance name.
6.  In the **Actions** list on the right, click **Image**.
7.  On the Request Imaging form, enter the necessary information:
    -   **Image Name**: Enter the name, up to 30 characters, to assign to the new image.
    -   **Description of the Image:** Enter the description of the image as it will appear in Atmosphere. The description should concisely describe the tools installed, the purpose of the tools (e.g., _This image performs X analysis_), and the initial intent of the machine image (e.g., _designed for XYZ workshop_).
    -   **Image Tags (Optional):** Click in the field and select the tags that will enhance search results for this image. You can **add and remove tags (NEED LINK) later, if needed.
    -   **Cloud for Deployment:** Select the cloud **provider (NEED LINK)** to use for the image. The list depends on the providers to which you have been granted access.
    -   **Image Visibility:** Select the image visibility, either **Public** (visible and launchable by any user), **Private** (visible and launchable only to you), or **Specific Users** (visible and launchable only by specified iPlant users). If you want to share the image with a specific user or users (restricted visibility), [email Support](mailto:support@iplantcollaborative.org) with a list of the iPlant user names, or submit [an online request](http://www.iplantcollaborative.org/forms/support).
8.  Click **Show advanced options** to view and select more options for the image:
    -   **List Installed Software:** Enter the name of any software applications that you have installed and the paths to the executables, if different from /usr/bin or /usr/local/bin.
    -   **iPlant-managed System Files**: If your machine image requires a change in an iPlant-managed system file (see **Important Notes NEED LINK]**), enter the specifics for the change and why the change is necessary.
    -   **Files to exclude:** List any files, one path per line, that you do not want included in the image.
    -   Checkbox: Click to acknowledge that the image contains no license-restricted software that is prohibited from distribution within a virtual or cloud environment.
9.  Click **Request Imaging**.

**Note: Do not stop or suspend the instance until you receive notification that the image has been created.**

You will receive an email when the image is being processed and again when it has been completed. Please email questions to [Atmosphere Support](mailto:support@iplantcollaborative.org).

## Viewing the list of your images

1.  Click **Images** on the top menu bar.
2.  Click **My Images** on the top of the screen.  
    The list of your images is displayed.

## Important notes before you request an image

**Before submitting your request for an image of your instance, you MUST remove the following software from the instance:**

-   Licensed software that was not purchased by iPlant.
-   Software in which the licensing otherwise prevents the use within a cloud or virtualized environment.

**The following directories are deleted as part of the imaging process:**

-   /home/<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{note:title=About your /home/ directory}</div><div class="wysiwyg-macro-body">
    -   All files, directories, and icons located under**/home/<username>/Desktop** will be deleted. To preserve them, please email [iPlant Support](mailto:support@iplantcollaborative.org).
    -   Any files installed in /home **must** be saved to your volume, to iRODS, or to another storage external to your VM.

-   /mnt/
-   /tmp/
-   /root/

**Volumes and iRODS FUSE mounts are not copied as part of the image.**

**The following system files are typically overwritten by iPlant for security or operational reasons:**

-   /etc/fstab
-   /etc/group
-   /etc/host.allow
-   /etc/host.conf
-   /etc/host.deny
-   /etc/hosts
-   /etc/ldap.conf
-   /etc/passwd
-   /etc/resolve.conf
-   /etc/shadow
-   /etc/sshd/
-   /etc/sysconfig/iptables
-   /root/
-   /var/log
