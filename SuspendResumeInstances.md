# Suspending and resuming an instance

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div>

Suspending an instance can be useful for saving your instance state for a later time, and for restoring the networking to an active instance that may have lost its connectivity. Suspending an instance releases the IP address of the instance and freezes its state without the need for imaging. You can suspend up to four instances that were launched with the iPlant Cloud-Tucson (Beta) provider.

Allocation time for suspended instances is not used; however, be aware that the CPU and memory resources are still allocated for the instance and cannot be used for other instances.

In addition to being able to resume a suspended instance, you also may[request an image](https://pods.iplantcollaborative.org/wiki/display/atmman/Request+an+Image+of+Your+Instance "Request an Image of Your Instance") of an instance, terminate a suspended instance, or ask[Support](mailto:support@iplantcollaborative.org) to help with resuming a suspended instance if you encounter capacity issues when resuming.

You can view a screencast of how to suspend and resume an instance[here](https://vimeo.com/100855170).

## Suspending an instance

1.  If necessary,[log in to Atmosphere](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+Atmosphere "Logging In to Atmosphere").
2.  Open the My Instances list and click the instance to suspend.
3.  On the Instance Details tab, click**Suspend**:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/11438755/OpenStackInstanceOptionsSuspend.gif?version=1&modificationDate=1391020472000)<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip:title=Suspend not displayed?}</div><div class="wysiwyg-macro-body">

    Instance suspending is only available for OpenStack-Tucson (Beta).

    </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div>
4.  After reading the dialog, click**Suspend Instance**.  
    When the instance has been suspended (it may take up to a minute), its status displays**suspended**. To verify, you may need to click![](https://pods.iplantcollaborative.org/wiki/download/attachments/11438755/RefreshInstanceIcon.gif?version=1&modificationDate=1393534754000).

## Resuming an instance

Resuming an instance may result in a different IP address than previously used for the instance. When an instance is resumed, the IP address may be changed, the shell access may be reconfigured and the VNC session will be relaunched.

1.  Open the My Instances list and click the suspended instance to resume.
2.  On the Instance Details tab, click**Resume**.
3.  Click**Resume Instance**.  
    When the instance is running again (it may take up to 5 minutes), its status displays**active**. To verify, you may need to click![](https://pods.iplantcollaborative.org/wiki/download/attachments/11438755/RefreshInstanceIcon.gif?version=1&modificationDate=1393534754000).

For questions on suspending and resuming instances, please contact[iPlant Support](mailto:support@iplantcollaborative.org).

# Suspended Atmosphere instances policy

To ensure the active and efficient use of iPlant’s cloud resources for maximum community benefit, the following time limits apply to Atmosphere instances that have been suspended:

*   iPlant Cloud – Tucson: Users may suspend their instance(s) for no more than four (4) continuous weeks (28 continuous days).
*   iPlant Cloud – Austin: Users may suspend their instance(s) for no more than four (4) continuous weeks (28 continuous days).
*   iPlant Cloud – Workshop: Users may suspend their instance(s) for no more than two (2) continuous weeks (14 continuous days).

One week (7 days) prior to the applicable time limit, the user will receive a single email notification of the termination of the impending instance(s) due to the time limit. When the time limit has been reached, iPlant will administratively[terminate](https://pods.iplantcollaborative.org/wiki/display/atmman/Terminating+an+Instance "Terminating an Instance") the suspended instance(s).

Volumes attached to a terminated instance will retain their data; however, data stored directly on a terminated instance is irretrievable.