# Logging in to an instance through the Web Shell or via Remote Desktop

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>

This page contains:

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div>
# Logging in to an instance

You can log in to an instance using the Web Shell, if available. If Web Shell is not available, you can log in using Remote Desktop. For a basic introduction to instances and images, see[Using Images and Launching Instances (Atmo-Beta)](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Images+and+Launching+Instances+%28Atmo-Beta%29 "Using Images and Launching Instances (Atmo-Beta)").

<div class="wysiwyg-macro wysiwyg-macro-inline"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{hidden-data}</div><div class="wysiwyg-macro-body"><div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{warning}</div><div class="wysiwyg-macro-body">

This link will have to be hard coded with each release.

</div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{warning}</div></div></div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{hidden-data}</div></div>
## Step 1: Open instance details

1.  If necessary,[log in to Atmosphere Airport](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+Atmosphere "Logging In to Atmosphere") and[launch the instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Launching+a+New+Instance "Launching a New Instance").
2.  Click**Projects** at the top and click to open the project to use.
3.  Click the name of the instance.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip}</div><div class="wysiwyg-macro-body">

    The instance must be in Active status.

    </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div>

## Step 2: Log in with Web Shell or Remote Desktop

Log in, either using Web Shell or Remote Desktop.

### Logging in with Web Shell

1.  Click**Open Web Shell** on the right.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip}</div><div class="wysiwyg-macro-body">

    If unavailable, try clicking![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090403/Atmo-Refresh.png?version=1&modificationDate=1421185825000) (Refresh).  
    If it is still not enabled, you can log in using Remote Desktop, or via SSH (steps for both below). You also may want to read  
    [Why can't I open the Shell tab?](https://pods.iplantcollaborative.org/wiki/display/atmman/Atmosphere+FAQs#AtmosphereFAQs-NoAirportShell).

    </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div>
2.  Enter your iPlant username and password.
3.  Click**Connect** and then enter your password again.

### Logging in with Remote Desktop (VPN)

1.  Click**Remote Desktop** on the right.
2.  If necessary, activate Java.
3.  Click**Run**.
4.  Click**Connect**.
5.  In the VNC Viewer - Identity check, click**Continue**.
6.  In the VNC Viewer – Authentication window, enter your iPlant username and password, and then click**OK**.

### Logging in via SSH

If Web Shell or Remote Desktop are unavailable, you can log in to your instance via SSH. Follow the steps below for your operating system.

### Mac OS X

1.  Open the Resources page by clicking**Projects** and then clicking the project with the instance to which you want to log in.
2.  In the Instances list, copy the IP address for the instance.
    1.  Open a terminal window for Mac OS X (Open a**Finder** window, go to**Applications**, click**Utilities**, and then double-click**Terminal**).
    2.  In the terminal window, enter the following command, using your iPlant username and password, and the instance IP address:<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{highlight}</div><div class="wysiwyg-macro-body">

        ssh your_iplantusername@ip_address

        </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{highlight}</div></div>

        **Example:**

        <div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">ssh kkennedy@328.196.142.3</pre></div></div></div>
    3.  If prompted to continue connecting, enter**yes**.
    4.  Press**Enter**.

### Windows

For Windows OS, use**PuTTY**, an SSH client for Windows. For a useful guide to using PuTTY, see[PuTTY – Remote Terminal and SSH Connectivity](http://linux.about.com/od/softinternet/a/Putty-Remote-Terminal-And-Ssh-Connectivity.htm).

1.  If necessary,[download the PuTTY application](http://www.putty.org/).
2.  Open the Resources page by clicking**Projects** and then clicking the project with the instance to which you want to log in.
3.  In the Instances list, copy the IP address for the instance.
4.  Launch PuTTY.
5.  Enter your username and paste the IP address.
6.  Click**Connect**.
7.  Enter your password and click**Enter**.

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoFeedbackSupport}</div></div>

You also can[report a problem with an Atmosphere instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Reporting+a+Broken+Instance "Reporting a Broken Instance").