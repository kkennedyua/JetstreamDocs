<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>
# Using instances

<table class="confluenceTable"><tbody><tr><th class="confluenceTh">This page contains</th><th class="confluenceTh">This section contains</th></tr><tr><td class="confluenceTd"><div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div></td><td class="confluenceTd"><div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{pagetree:root=@self}</div></div></td></tr></tbody></table>
## Opening the Images window

1.  <div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_atmo_login}</div></div>
2.  Click**Images** on the top menu bar.

# About launching instances

You can view the list of public and featured images, the images you[created](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Projects "Using Projects"), and your list of favorite images. You also can search by image name, tag, OS, and more.

Atmosphere provides a number of images from which you can launch an instance.

*   An**_image_** is a template for an_instance_ on a virtual machine (_VM_) that is already installed with a specific operating system, software, and configuration for use with that setup.<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:InstanceDef}</div></div>
*   An**_instance_**, in the Atmosphere world, is a VM image that has been launched. Each instance is a specific VM, existing on a physical compute node, with its own dedicated RAM, CPUs, and disk space.

You use an instance in Atmosphere just as you use a physical computer for most tasks. Once you have selected the image to use, you launch an instance of the image.

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip}</div><div class="wysiwyg-macro-body">

To learn how to launch an instance, see[Launching a New Instance (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Launching+a+New+Instance+%28Atmo-Beta%29 "Launching a New Instance (Atmo-Beta)").

</div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div>

For more information on virtual machines, see[Virtual machines](http://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&ved=0CEUQFjAA&url=http%3A%2F%2Fen.wikipedia.org%2Fwiki%2FVirtual_machine&ei=CHSmUbDxJcWbigKpr4G4BA&usg=AFQjCNExT7UOidDfl6IxUB_uPimill1UEA&sig2=JCKk_3upiYfvEFPjFkBbIw&bvm=bv.47244034,d.cGE) on the Wikipedia website.

For a general overview of cloud computing, see[Cloud Computing Explained](http://www.webopedia.com/quick_ref/cloud_computing.asp) on the Webopedia website.

# About instance size

An important consideration is the size of the instance. Instance size determines the amount of resources (CPUs, RAM, Atmosphere Units, or a combination of the three) that will be used when you launch the instance.

The[provider](https://pods.iplantcollaborative.org/wiki/display/atmman/Selecting+Your+Cloud+Provider "Selecting Your Cloud Provider")you select determines the amount of resources and options that are available. Depending on your access, Atmosphere may offer up to three different[cloud provider types](https://pods.iplantcollaborative.org/wiki/display/atmman/Selecting+Your+Cloud+Provider "Selecting Your Cloud Provider").

All new and existing users have a 168 AUs starter allocation, enough time to continuously run a 1 CPU-core instance for 1 week. Users who exceed their allocation will have their instances suspended until their allocation is refreshed. Additional allocation can be obtain using the 'Request more resources' form within Atmosphere, which will be reviewed by an allocation committee.

At this time, xlarge instances are only available on the "iPlant Cloud - Tucson (beta)" provider.

Your resource usage is determined by the cumulative amount of CPUs, RAM, and**Atmosphere Units (AUs)**, or a combination of the three. One AU is roughly equivalent to one CPU-hour, or one CPU-core used per hour. For example, a 16-core instance running for one hour uses 16 AUs. You may[request more resources](https://pods.iplantcollaborative.org/wiki/display/atmman/Requesting+More+Atmosphere+Resources "Requesting More Atmosphere Resources") within Atmosphere Airport.

Instance size is set by default to the smallest amount available in each provider, and this is sufficient for most uses. A larger size gives you more computing power but fewer remaining resources for other running instances, while a smaller size gives you more resources to launch more instances but less computing power.

The size you select determines how much of your resource allocation you use, as well as how much power is available to you for the instance; both are displayed in the**My Projected Resource Usage** section above the instance information section.

If your resource usage bars indicate you are already using 100% of your resources, you must either select a smaller instance size or a different instance,[terminate](https://pods.iplantcollaborative.org/wiki/display/atmman/Terminating+an+Instance "Terminating an Instance") or[suspend](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspending+and+Resuming+an+Instance "Suspending and Resuming an Instance") a different running instance, or[request more resources](https://pods.iplantcollaborative.org/wiki/display/atmman/Requesting+More+Atmosphere+Resources "Requesting More Atmosphere Resources").

Instances are available on a first-come-first-served basis. Depending on Atmosphere's capacity, you may be unable to launch an instance even though you have sufficient allocation.

Your instance may be[suspended](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspending+and+Resuming+an+Instance "Suspending and Resuming an Instance")by Atmosphere Support if it has not performed significant computations, measured by load average, or has not had an interactive session via SSH or VNC for more than three (3) calendar days. It may be resumed at a later time, based on available resources.

For more information on virtual machines, see[Virtual machine](http://en.wikipedia.org/wiki/Virtual_machine) on the Wikipedia website.  
For a general overview of cloud computing, see[Cloud Computing Explained](http://www.webopedia.com/quick_ref/cloud_computing.asp) on the Webopedia website.

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{hidden-data}</div><div class="wysiwyg-macro-body"><div class="wysiwyg-macro"><div class="panel" style="border-width: 1px;"><div class="panelContent">
# NOTE: Do not rename this page. It is referenced in the "Your Atmosphere Instance is available" email that is generated when the instance is running.

**NEED TO FIND OUT HOW THEY WANT TO LINK TO THESE PAGES FOR DIFFERENT VERSIONS.**

</div></div></div></div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{hidden-data}</div></div>