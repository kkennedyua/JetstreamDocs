<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div><div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div>
## Before you begin

Before you begin, you may want to learn more about[instances and instance size](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Instances "Using Instances").

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_atmo_login}</div></div>
## About launching instances

Atmosphere provides a number of images you can use for launching an instance.You can select from a list of featured, favorite, and all images, sorted by list view or grid view. You also can search for an image by image name, tag, and description.

You can launch an instance either from a project or from an image.

### Launching an instance from a project

1.  If necessary,[log in to Atmosphere](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+Atmosphere "Logging In to Atmosphere").
2.  Click**Projects** on the top toolbar and then click to open the project from which you want to launch the instance.
    *   To create a new project, see[Using Projects](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Projects "Using Projects").
3.  Click**New** and then click**Instance**. The Select Image window opens.  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/13600796/ImagesList.png?version=1&modificationDate=1421105388000)
4.  To search for an image, click in the search field at the top; enter the image name, tag (displayed in green under the image name), description, or OS.
5.  Click the image to use.
6.  In the Review Image window, click**Configure**.
7.  In the Configure Image window:
    1.  Enter the name for the instance.
    2.  Select the version of the image to use.
    3.  Select the[provider](https://pods.iplantcollaborative.org/wiki/display/atmman/Selecting+Your+Cloud+Provider "Selecting Your Cloud Provider") to use.
    4.  Select the instance[size](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Instances+%28Atmo-Beta%29#UsingInstances%28Atmo-Beta%29-AboutInstanceSize).  
        The size you may choose depends on the amount of resources that will be used by the image and your resource availability.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip:title=Start small}</div><div class="wysiwyg-macro-body">

        Start with the smallest size until you know for certain what size you need for that image.

        </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div>
    5.  Click**Launch Instance**. The instance is added to the project's Instances list and you can view its status as it is being launched. Once the status is Active you may begin using it.<div class="wysiwyg-macro"><div class="panel" style="border-width: 1px;"><div class="panelContent">

        It may take up to 30 minutes for the instance to be accessible. Click![](https://pods.iplantcollaborative.org/wiki/download/attachments/13600796/RefreshInstanceIcon.gif?version=1&modificationDate=1421106395000) to see if your instance status has changed to Active.  
        Once Active, you will receive an email with the instance ID and IP address.

        </div></div></div>

### Launching an instance from the Images list

1.  Click**Images** on the menu bar.
2.  To search for an image, click in the search field at the top; enter the image name, tag (displayed in green under the image name), description, or OS.
3.  Click the image name to use.
4.  In the image window, click**Launch**.
5.  In the instance form:
    1.  Enter the name for the instance.
    2.  Select the version of the image to use.
    3.  Select the[provider](https://pods.iplantcollaborative.org/wiki/display/atmman/Selecting+Your+Cloud+Provider "Selecting Your Cloud Provider") to use.
    4.  Select the instance size.  
        The size you may choose depends on the amount of resources that will be used by the image and your resource availability.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip:title=Start small}</div><div class="wysiwyg-macro-body">

        Start with the smallest size until you know for certain what size you need for that image.

        </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div>
    5.  Click**Launch Instance**. The instance is added to the project's Instances list and you can view its status as it is being launched. Once the status is Active you may begin using it.<div class="wysiwyg-macro"><div class="panel" style="border-width: 1px;"><div class="panelContent">

        It may take up to 30 minutes for the instance to be accessible. Click![](https://pods.iplantcollaborative.org/wiki/download/attachments/13600796/RefreshInstanceIcon.gif?version=1&modificationDate=1421106395000) to see if your instance status has changed to Active.  
        Once Active, you will receive an email with the instance ID and IP address.

        </div></div></div>

## After the instance is launched

[Ask iPlant](http://ask.iplantcollaborative.org/questions/scope:all/sort:activity-desc/tags:Atmosphere/page:1/) gives answers to questions from other users about Atmosphere, such as[How long to get a new instance?](http://ask.iplantcollaborative.org/question/24/how-long-to-get-a-new-instance/)  

When done with the instance, you should[suspend](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspending+and+Resuming+an+Instance "Suspending and Resuming an Instance"),[stop](https://pods.iplantcollaborative.org/wiki/display/atmman/Stopping+and+Starting+an+Instance "Stopping and Starting an Instance"), or[delete](https://pods.iplantcollaborative.org/wiki/display/atmman/Terminating+an+Instance "Terminating an Instance") it.

To request that your instance be made into an image to reuse and share, or to add code to the instance before it is imaged that executes a script that runs after the image is booted, see[Request an Image of Your Instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Request+an+Image+of+Your+Instance "Request an Image of Your Instance").