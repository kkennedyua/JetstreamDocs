# Using Images and Instances

An **_image_** is a kind of template for an_instance_. It runs on a virtual machine (_VM_) that is already installed with a specific operating system, software, and configuration for use with that setup.

An **_instance_**, in the Atmosphere world, is a VM _image) that has been launched. Each instance is a specific VM, existing on a physical compute node, with its own dedicated RAM, CPUs, and disk space.

You use an instance in Atmosphere just as you use a physical computer for most tasks. Once you have selected the image to use, you launch an instance of the image.

You can view details about and manage your instances, including suspending and resuming, stopping and starting, and deleting an instance.

You also can view and access your Atmosphere instances using **Web Shell or Remote Desktop (NEED LINK)**.

You can **attach and detach one or more volumes (NEED LINK)** in the same project to the same instance, and view metrics about how your resources (memory, disk space, CPU, and AU usage) are being used on this instance.

## Launching instances

You can launch instances either from the Projects screen or from the Images screen.

### Launching from the Projects screen
1.  Click **Projects** on the top toolbar and then click to open the project from which you want to launch the instance.
    To create a new project, see **Using Projects (NEED LINK)**.
2.  Click **New** and then click **Instance**.
3.  In the Select Image screen, click in the search field at the top and enter the image name, [tag](#tag), description, or OS, and then click the image to use.
3.  In the Review Image window, click **Configure**.
4.  In the Configure Image window:

	a.  Enter the name for the instance.
	
	b.  Select the version of the image to use.
	
	c.  Select the **provider (NEED LINK)** to use.
	
    d.  Select the instance **size (NEED LINK)**.
  
    The size you may choose depends on the amount of resources required by the image and your resource availability. Start with the smallest size until you know for certain what size you really need for that image. Also be aware that availability of provider resources may affect your ability to launch instances.
    
    e. Click **Launch Instance**.
    
      The instance is added to the project's Instances list and you can view its status as it is being launched. Once the status is Active you may begin using it.
      
	**Note:** It may take up to 30 minutes for the instance to be accessible. Click **REFRESH (NEED IMAGE)** to see if your instance status has changed to Active. You will receive an email with the instance ID and IP address once the instance is in active status.

### Launching from the Images screen
1.  Click **Images** on the menu bar.
2.  To search for an image, click in the search field at the top, and enter the image name, tag (displayed in green under the image name), description, or OS.
3.  Click the image name to use.
4.  In the image window, click **Launch**.
5.  In the instance form:

    a.  Enter the name for the instance.
    
    b.  Select the version of the image to use.
    
    c.  Select the provider **(NEED LINK**) to use.
    
    d.  Select the instance size.  
    
    The size you may choose depends on the amount of resources that will be used by the image and your resource availability. Start with the smallest size until you know for certain what size you need for that image.
    
    e.  Click **Launch Instance**. The instance is added to the project's Instances list and you can view its status as it is being launched. Once the status is Active you may begin using it.
    
       **Note:** It may take up to 30 minutes for the instance to be accessible. Click **REFRESH (NEED IMAGE)** to see if your instance status has changed to Active. You will receive an email with the instance ID and IP address once the instance is in active status.
       
To request that your instance be made into an image to reuse and share, or to add code to the instance before it is imaged that executes a script that runs after the image is booted, see **Request an Image of Your Instance (MOVE CONTENT TO THIS PAGE)**.

## Suspending, resuming, stopping, and deleting instances

You can suspend an active instance or resume a suspended instance, stop a suspended or active instance, or delete an active, suspended, or shutoff (deleted) instance.

1.  Click an icon at the top right:
    - **SUSPEND ICON (NEED IMAGE)**: Available when the instance is active.  
    - **RESUME ICON (NEED IMAGE)**: Available when the instance is suspended.  
    - **STOP ICON (NEED IMAGE):** Available when the instance is active or suspended.  
    - **SHUTOFF ICON (NEED IMAGE):** Available when the instance is active, suspended, or shutoff. Status will display as _shutoff_.

## Renaming instances
    - **RESUME ICON (NEED IMAGE):** Available when the instance is suspended.  
    - **STOP ICON (NEED IMAGE):** Available when the instance is active or suspended.  
    - **SHUTOFF ICON (NEED IMAGE):** Available when the instance is active, suspended, or shutoff. Status will display as _shutoff_.

1.  Click the instance name to open the instance.
2.  Hover over the name until a pencil icon is displayed to the right of the name:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090410/RenameInstance.jpg?version=1&modificationDate=1425341463000)
3.  Click the pencil icon.
4.  Edit the name and press **Return**.

## Viewing, adding, and removing Favorite images

You can create and manage your list of favorite images. Favorite images have a yellow star on the right side of the image.

### Viewing your Favorites list

To view your Favorites list, click **Images**, and then click **Favorites**.

### Adding a favorite instance to your list
1.  Find the image to add by scrolling through the list, or search for the image by entering the image name, tag, or description in the search field.
2.  Click ![] (https://pods.iplantcollaborative.org/wiki/download/attachments/12225026/FavoriteImages-StarIcon.gif?version=1&modificationDate=1406915420000) to the right of the image. 
The image is added to your Favorites list with a yellow star.

### Removing a favorite image from your list
1. Click the yellow star to the right of the image.

## Adding tags to running instances<a name="tag"></a>

You can add tags to a running instance to help you find it more easily in search.

1.  Open the running instance.
2.  On the Instance Details tab, click the **Edit Tags** icon.
3.  In the text field, enter the tag to add and click **Add**:  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/8411419/Tags-1.png?version=1&modificationDate=1369083148000)
4.  Repeat for each additional instance tag to add.
5.  When done, click **Done**.


## Using the Favorites list

You can create and manage your list of favorite images. Favorite images have a yellow star on the right side of the image.

### Viewing your Favorites list

To view your Favorites list, click **Images** and then click **Favorites**.

### Adding and removing instances from your Favorites list

1.  To add an image to your Favorites list:

    a. Find the image to add by scrolling through the list, or search for the image by entering the image name, tag, or description in the search field.
    
    b. Click ![] (https://pods.iplantcollaborative.org/wiki/download/attachments/12225026/FavoriteImages-StarIcon.gif?version=1&modificationDate=1406915420000) to the right of the image. 
The image is added to your Favorites list with a yellow star.
2. To remove an instance from the list, click the yellow star to the right of the image.


## Adding and removing tags

A _tag_ is a label — a form of metadata — that can be added to a running instance for improved searchability. You can select from the list of existing tags added by the community, add new one to the list, remove a tag from an instance, and request deletion of the tag from the list.

1.  Click **Projects** on the menu bar.
2.  In the Resources list, click the instance to which you want to add a tag.
3.  In the Instances list, click the name of the instance.
4.  Click **Create/Edit tags**.
5.  **To select an existing tag:**

    a.  Click in the field and enter the first few letters.
    
    b.  Click the tag in the list.
    
7.  **To create a new tag for the instance:**

    a.  Enter the new name.
    
    b.  Either press **Enter** or click **+ New tag**.
    
    c.  In the Create Tag form, enter the name and description for the tag and click **Create tag**. The new tag is added to the instance and the list of tags.
    
8. **To remove a tag from an instance:** Click the name of the instance, and then click **Done editing**. The tag is still available in the list for others to choose.

9. **To delete a tag from the list, or to add code to the instance before it is imaged that executes a script that runs after the image is booted:**

    a.  Click **Feedback & Support** at the bottom of the screen.
    
    b.  In the Send Feedback form, enter the tag name to edit or delete, and the justification for the change.
    
    c.  Click **Send feedback**.

9.  When done, click **Done editing**.

10. **To view the master list of tags,** click **Images** on the menu bar, and then click **Tags** at the top of the screen. 
    -   To view the tag's description, if available, hover over the tag name.
    -   To find all images that use a specific tag in the image name or description, enter the tag name or description in the search field:  
        ![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090585/ImageTagList-ListView.png?version=1&modificationDate=1421453336000)
    -   Click **Grid** to view the tag list in table view, or **List** to view in list view (default).

## Viewing instance details

After an instance is active, you can view information about it, including its IP address, the IDs of the instance and its based-on (parent) image, and the date you launched the image. Also displayed are its status and any [tags][] that have been applied to the instance.

1.  Click **Projects** at the top.
2.  Click the project with the instance to view.
3.  Click the checkbox for the instance to view its Details panel on the right (the same details are available when the instance is opened by clicking its checkbox):
    -   **ID:** Unique identifier assigned to this instance.
    -   **Status:** Current status of this instance.
    -   **Size:** Amount of CPUs, memory, and disk size used by the instance.
    -   **IP Address:** Assigned IP address, used to log in via **SSH window** (NEED LINK).
    -   **Launched: (NEED LINK)** Date the instance was launched.
    -   **Based on: (NEED LINK)** Image that was selected when the instance was launched.
    -   **Provider: (NEED LINK)** to which the instance is located.

## About instance metrics

Each instance provides details, such as the CPU load, RAM, and used disk space.

-   **My Resource Usage** at the top of the screen shows how much of your quota in CPUs and GB of memory is being used by your running instances. 
When selecting a new instance to launch, the resource usage reflects how much resources will be allocated according to the selected instance size. You can reuse your resources only after the instance has been terminated and is no longer displayed in the My Instances list. For more information on allocations, see **Allocation Policies (NEED LINK)**.

-   **Instance Details** tab displays important information about the instance, including the ID assigned to the instance when it was launched, name of the image it is using, unique EMI ID, the instance size, the date you launched the image, and the IP address, which you will need when **logging in (NEED LINK)** to the instance.

-   **Instance Metrics** allows you to drill down into the usage expended for the running image, including percentage used for RAM and used disk space, and CPU load. Not all images provide instance metrics.

## Have a problem?

Report a problem with an instance, image, or volume **(NEED LINK)**.
