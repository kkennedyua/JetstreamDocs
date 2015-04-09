<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>
# Managing your projects

You can rename and delete a project.

You can manage resources (instances and volumes) in a project, including viewing details about an instance or volume, deleting an instance or volume, and[moving an instance or volume to a different project](https://pods.iplantcollaborative.org/wiki/display/atmman/Moving+an+Instance+to+a+Different+Project+%28Atmo-Beta%29 "Moving an Instance to a Different Project (Atmo-Beta)").

This page contains:

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div>
### Creating a new project

1.  If necessary,[log in to Atmosphere](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+Atmosphere "Logging In to Atmosphere").
2.  Click**Projects** on the top toolbar.
3.  At the top right, click**Create New Project**.
4.  In the Create Project window, enter the project name and description, and click**Create**.

## Renaming a project

1.  On the Projects page, click the project to rename.
2.  Click**Details** under the project name.
3.  Click**Edit details**.
4.  Edit the name and description as needed.
5.  Click**Save**.

## Deleting a project

Before you can delete a project, all instances in the project must be moved or deleted, and all volumes in the project must be detached.

1.  Open the project to delete.
2.  If you have not already done so,[move](https://pods.iplantcollaborative.org/#ManagingProjects-moveResource) or[delete](https://pods.iplantcollaborative.org/wiki/display/atmman/Suspend+and+Resume%2C+Stop+and+Start%2C+Delete+Instances+%28Atmo-Beta%29 "Suspend and Resume, Stop and Start, Delete Instances (Atmo-Beta)") all instances in the project, and[detach](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance+%28Atmo-Beta%29 "Attaching a Volume to an Instance (Atmo-Beta)") all volumes in the project.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip}</div><div class="wysiwyg-macro-body">

    You may want to[request an image of your instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Requesting+an+Image+of+an+Instance "Requesting an Image of an Instance") before you move or delete it so you can use it again.

    </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div>
3.  Click**Options** on the top right and then click**Delete Project**.
4.  In the Delete Project prompt, click**Okay**.

### Viewing details about an instance or volume

Instance details include the instance ID, and its status, size, IP address, date launched, image upon which it is based, and the provider identity.  
Volume details include the status, size, provider identity, and volume ID.

1.  In the project to view, click the checkbox next to the instance or volume whose details you want to view.
2.  View information about the last selected instance or volume in the Details pane on the right.  
    You also can view details about a resource and take actions on it by clicking the instance name or volume name.

## Managing instances in a project

See the[Using Images and Launching Instances](https://pods.iplantcollaborative.org/wiki/display/atmman/Viewing+and+Managing+Instances+%28Atmo-Beta%29 "Viewing and Managing Instances (Atmo-Beta)") section for information on how to manage your instances.

## Managing volumes in a project

See the[Using Volumes (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Volumes+%28Atmo-Beta%29 "Using Volumes (Atmo-Beta)") section for information on how to manage your volumes.

# See also

*   [Moving an Instance or Volume to a Different Project (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Moving+an+Instance+to+a+Different+Project+%28Atmo-Beta%29 "Moving an Instance to a Different Project (Atmo-Beta)")  

*   [Deleting an Instance or Volume from a Project (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Deleting+an+Instance+from+a+Project+%28Atmo-Beta%29 "Deleting an Instance from a Project (Atmo-Beta)")