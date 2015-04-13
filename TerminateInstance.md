# Terminating an instance

You can terminate an instance that is in a status of pending or running. To preserve your data you must first[unmount and detach any attached volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance#AttachingaVolumetoanInstance-UnmountDetachVolume) the instance before terminating it.

**iPlant Support also may terminate an instance that has been suspended for an extended period of time. For more information, see[Suspending and Resuming an Instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspending+and+Resuming+an+Instance "Suspending and Resuming an Instance").**

Volumes attached to a terminated instance will retain their data; however, data stored directly on a terminated instance is irretrievable.

1.  If necessary,[log in to Atmosphere](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+Atmosphere "Logging In to Atmosphere").
2.  In the**My Instances** list on the left, click the instance to terminate.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{warning:title=Warning!}</div><div class="wysiwyg-macro-body">

    Before terminating an instance, you must[unmount and detach any attached volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance#AttachingaVolumetoanInstance-UnmountDetachVolume).  
    Terminating an instance that is still mounted may cause corruption to your data and volume.

    </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{warning}</div></div>
3.  Click**Terminate**.
4.  Click**Yes, terminate this instance** to the warning message.  
    The instance status changes to shutting-down. Your resource usage will not reflect the change until the instance has completed the termination and is no longer displayed in your instances list. You may need to click![](https://pods.iplantcollaborative.org/wiki/download/attachments/6728775/RefreshInstanceIcon.gif?version=1&modificationDate=1393535781000).