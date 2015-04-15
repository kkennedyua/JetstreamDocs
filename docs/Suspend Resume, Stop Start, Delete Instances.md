<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>
# About managing instances

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div>

There are different ways to stop and start instances, depending on your needs. You can:

*   **Suspend and resume an instance:** Allows you to save your instance state for a later time and restore the networking to an active instance that may have lost its connectivity. Allocation time for suspended instances is not used; however, the CPU and memory resources are still allocated for the instance and cannot be used for other instances.

*   **Stop and start an instance:** A stopped instance continues to use time allocation, so you may want to suspend the instance instead. To restart a stopped instance, you must have sufficient quota and the cloud provider must have enough room to support your instance's size.

*   **Delete an instance:** When you know you no longer need an instance, you can delete (terminate) it.

# Suspending and resuming an instance

Suspending an instance can be useful for saving your instance state for a later time. When you suspend an instance, its state is frozen, your time allocation no longer counts against you, and the IP address may be released. A suspended instance frees up its resources for other users and allows you to safely preserve the instance's state without[imaging](https://pods.iplantcollaborative.org/wiki/display/atmman/Request+an+Image+of+Your+Instance "Request an Image of Your Instance").

You can suspend up to four instances that were launched with the iPlant Cloud-Tucson provider.

If you run out of allocation resources, your instances will be suspended automatically and maintained in that state up to the limit for that provider, as outlined in[Allocation Policies (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Allocation+Policies+%28Atmo-Beta%29 "Allocation Policies (Atmo-Beta)"). You can resume them after your allocation is reset at the beginning of the month.

## Suspending an instance

1.  If necessary,[log in](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+and+Signing+Out+of+Atmosphere+%28Atmo-Beta%29 "Logging In to and Signing Out of Atmosphere (Atmo-Beta)") to Atmosphere.
2.  Click**Projects** on the menu bar and then click to open the project with the instance to suspend.
3.  Click the checkbox for the active instance to suspend.
4.  Click![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090415/InstanceSuspendIcon.jpg?version=1&modificationDate=1424812235000) (Suspend) at the top right.
5.  Click yes to the prompt.  
    The status changes to_Active - suspending_ and finally to_Suspended_, and the IP address changes to 0.0.0.0 to indicate it is now unassigned. This process may take up to 30 minutes to complete so please be patient.  
    You may[resume](https://pods.iplantcollaborative.org/#SuspendandResume%2CStopandStart%2CDeleteInstances%28Atmo-Beta%29-Resuminganinstance) or[delete](https://pods.iplantcollaborative.org/#SuspendandResume%2CStopandStart%2CDeleteInstances%28Atmo-Beta%29-Deletinganinstance) the instance at any time, up to the limit specified in[Allocation Policies (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Allocation+Policies+%28Atmo-Beta%29 "Allocation Policies (Atmo-Beta)").

## Resuming an instance

A resumed instance may be assigned a different IP address from the IP address it had before the instance was suspended. If the instance was launched using[Web Shell or Remote Desktop](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+an+Instance+Through+the+Web+Shell+or+Via+Remote+Desktop+%28Atmo-Beta%29 "Logging In to an Instance Through the Web Shell or Via Remote Desktop (Atmo-Beta)"), the shell access also may be reconfigured and the Remote Desktop session will be relaunched.

1.  Click**Projects** on the menu bar and then click to open the project with the instance to resume.
2.  Click the checkbox for the suspended instance to resume.
3.  Click![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090415/InstanceResumeIcon.jpg?version=1&modificationDate=1424812820000) (Resume) at the top right.
4.  Click yes to the prompt.
5.  In the Actions panel on the right, click**Resume**.
6.  After reading the message, click**Yes, resume this instance**.
7.  The instance status changes to_Suspended - resuming_ and finally to_Active_.

# Stopping and starting an instance

You can stop an instance and then restart it. This is equivalent to shutting down your computer: all programs and documents are closed and the machine is powered off.

**A stopped instance continues to use time allocation.** To preserve resources and time allocation, you may want to[suspend the instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspending+and+Resuming+an+Instance "Suspending and Resuming an Instance") instead.

You must have sufficient quota to restart the instance, and the provider must have enough room available to support your instance's size.

## Stopping an instance

1.  Click**Projects** on the menu bar and then click to open the project with the instance to stop.
2.  Click the instance name to open the instance.
3.  In the Actions list on the right, click**Stop**.
4.  After reading the message, click**Yes, stop this instance**.  
    The status changes to Shutoff.

## Starting a stopped instance

In order to start a stopped instance, you must have sufficient quota_and_the cloud provider must have enough room to support your instance's size. You also will need to reopen the applications and documents.

1.  Click**Projects** on the menu bar and then click the project with the instance to restart.
2.  Click the instance name to open the instance.
3.  In the Actions list on the right, click**Start**.
4.  After reading the message, click**Start Instance**. The status changes to Active.

# Deleting an instance

You can delete an instance that is in a status of active, suspended, or stopped. To preserve your data you must first detach any volumes that are attached to the instance before deleting the instance.

1.  If you have not already done so,[detach any volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance#AttachingaVolumetoanInstance-UnmountDetachVolume) that are attached to the instance.
2.  Click**Projects** on the menu bar and then click the project with the instance to delete.
3.  Click the instance checkbox for the instance or instances to delete.
4.  Click![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090415/DeleteResourceIcon.png?version=1&modificationDate=1421194051000).
5.  After reading the message, click**Yes, delete the resources**.  
    The instance is deleted from your Instances list and your resource usage is updated.

# Questions or need help?

For questions about or assistance with any of these actions, please contact[iPlant Support](mailto:support@iplantcollaborative.org).