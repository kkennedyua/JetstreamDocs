<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>
## About projects

A project — a new feature with this release — is the landing place for the instances and volumes you use in your work. A project can have more than one instance or one volume, but each instance or volume can exist in only one project.

You can create, view, add, move, and delete an instance or volume from its project, attach a volume to an instance in the same project, detach a volume from its project, and rename and delete a project. You also can report a problem with a project or its resources.

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div>
## Opening the Projects window

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:OpenProjectWindow}</div></div>
1.  If necessary,[log in to Atmosphere](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+Atmosphere "Logging In to Atmosphere").
2.  Click**Projects** on the top toolbar.  
    The list of your projects is displayed, showing the total number of instances, volumes, and instances in each:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/12224892/ProjectsList.png?version=1&modificationDate=1421451011000)

## Creating a new project

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:CreateNewProject}</div></div>
1.  On the**Projects** page, click**Create New Project**.
2.  Enter the project name and description.
3.  Click**Create**. The project is added to the list.

## Opening a project

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:OpenProject}</div></div>
1.  On the**Projects** page, click the project to open.  
    The project window opens, displaying the Resources and Details tabs.

## Adding instances and volumes to a project

From within the project, you can[create instances](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Instances "Using Instances") and[volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Volumes "Using Volumes"). You also can[move instances](https://pods.iplantcollaborative.org/wiki/display/atmman/Moving+an+Instance+to+a+Different+Project+%28Atmo-Beta%29 "Moving an Instance to a Different Project (Atmo-Beta)") and[volumes](https://pods.iplantcollaborative.org/wiki/display/atmman/Managing+Projects "Managing Projects") into a different project.

### Launching an instance

You can launch an instance both from the Projects page. You can also launch an instance from the[Images](https://pods.iplantcollaborative.org/wiki/display/atmman/Launching+a+New+Instance "Launching a New Instance") page.

1.  On the Projects page, open the project, if necessary. The project's Resources screen opens:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/12224892/ProjectResources.png?version=1&modificationDate=1421451110000)
2.  Click**New** and then click**Instance**. The Select Image list opens:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/12224892/ImagesList.png?version=1&modificationDate=1420670929000)
3.  To search for the image to use:
    1.  Click in the search field at the top.
    2.  Enter the first few characters of the image name, tag (displayed in green under the image name), or OS.
    3.  When the list is displayed, click to select the image to use.
4.  In the Review Image window, click**Configure**.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{warning}</div><div class="wysiwyg-macro-body">

    If you receive a warning that you don't have any AUs (Atmosphere Units) available, click**x** at the top, and then either[suspend, stop, or delete](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspend+and+Resume%2C+Stop+and+Start%2C+Delete+Instances+%28Atmo-Beta%29 "Suspend and Resume, Stop and Start, Delete Instances (Atmo-Beta)") an instance to free resources for the new one. Check your allocation availability in the**Resources in Use** section on your[Dashboard](https://pods.iplantcollaborative.org/wiki/display/atmman/About+the+Atmosphere+Dashboard "About the Atmosphere Dashboard").

    </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{warning}</div></div>
5.  In the Configure Image window:
    1.  Enter the name for the instance.
    2.  Select the version of the image to use.
    3.  Select the[provider](https://pods.iplantcollaborative.org/wiki/display/atmman/Selecting+Your+Cloud+Provider "Selecting Your Cloud Provider") to use.
    4.  Select the instance sizes.  
        The size you may choose depends on the amount of resources that will be used by the image and your resource availability.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip:title=Start small}</div><div class="wysiwyg-macro-body">

        Start with the smallest size until you know for certain what size you need for that image.

        </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div>
    5.  Click**Launch Instance**. The instance is added to the project's Instances list.

## Creating a volume

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{anchor:CreateVolume}</div></div>
1.  On the Projects page, open the project, if necessary.
2.  Click**New** and then click**Volume**.
3.  In the Create Volume form:
    1.  Enter the volume name.
    2.  In the Volume Size field, click the up or down arrows or enter the volume size, up to the size of your allotted AUs, as displayed in the Projected Resource Usage graph below.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{note}</div><div class="wysiwyg-macro-body">

        For larger volumes, consider using[iRODS](https://pods.iplantcollaborative.org/wiki/display/DS/Storing+and+Accessing+Your+Data+in+the+Data+Store "Storing and Accessing Your Data in the Data Store"), or you can[contact iPlant Support](mailto:support@iplantcollaborative.org) to create a larger volume.

        </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{note}</div></div>
    3.  Select the[provider](https://pods.iplantcollaborative.org/wiki/display/atmman/Selecting+Your+Cloud+Provider "Selecting Your Cloud Provider") to use.
    4.  Review the projected resource usage.
    5.  Click**Create volume**. The volume is added to the project's Volumes list.

### Attaching a volume to an instance

You can attach a volume to an instance that exists in the same project. For instructions, see[Attaching a Volume to an Instance (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance+%28Atmo-Beta%29 "Attaching a Volume to an Instance (Atmo-Beta)").

## See also

*   [Managing Projects](https://pods.iplantcollaborative.org/wiki/display/atmman/Managing+Projects "Managing Projects")  

## Need help?

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip}</div><div class="wysiwyg-macro-body">

Need help with a project, instance, or volume? See[Reporting an Issue with a Project, Instance, or Volume](https://pods.iplantcollaborative.org/wiki/display/atmman/Reporting+an+Issue+with+a+Project%2C+Instance%2C+or+Volume "Reporting an Issue with a Project, Instance, or Volume").

</div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div><div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{hidden-data}</div><div class="wysiwyg-macro-body"><div class="wysiwyg-macro"><div class="panel" style="border-width: 1px;"><div class="panelContent">
# For future release

*ADD SECTION ABOUT DETAILS TAB ON PROJECTS PAGE:[https://pods.iplantcollaborative.org/jira/browse/ATMO-599*](https://pods.iplantcollaborative.org/jira/browse/ATMO-599*)  

</div></div></div></div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{hidden-data}</div></div>