<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>
# Logging in to an instance

This page contains:

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc:minLevel=2}</div></div>

You can log in to an instance in a web shell window or in a separate SSH window. For a basic introduction to instances and images, see[Using Instances](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Instances "Using Instances").

## Logging in to an instance through the Web Shell

1.  If necessary,[log in to Atmosphere](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+Atmosphere "Logging In to Atmosphere") and[launch the instance](https://pods.iplantcollaborative.org/wiki/display/atmman/Launching+a+New+Instance "Launching a New Instance").
2.  Continue for your Atmosphere version:
    *   **For Atmosphere Beta:**
        1.  When the status shows as Active, click**Projects** on the menu bar.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip}</div><div class="wysiwyg-macro-body">

            You may need to refresh your browser to view the updated status.

            </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div>
        2.  Click the image name to use.
        3.  In the**Links** list on the right, click**Open Web Shell**.<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{note:title=Web Shell not available?}</div><div class="wysiwyg-macro-body">

             See[Why can't I open a Shell window?](https://pods.iplantcollaborative.org/wiki/display/atmman/Atmosphere+FAQs#AtmosphereFAQs-NoAirportShell)  

            </div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{note}</div></div>
        4.  Enter your iPlant username and password, and click to open the window in Gate One. The terminal window opens.

## Logging in via SSH

If the Shell tab is unavailable in Atmosphere, you can log in to your instance via SSH for your operating system.

### Mac OS X SSH login

1.  Copy the instance IP address, either from the confirmation email or from the IP address displayed in your Instances list.
2.  Open a terminal window for Mac OS X (from**Finder**, go to**Applications**, click**Utilities**, and then double-click**Terminal**):  
    ![](https://pods.iplantcollaborative.org/wiki/download/attachments/14090267/Terminal1.jpg?version=1&modificationDate=1423515634000)
3.  In the terminal window, enter the following command, substituting your iPlant username and password, and the instance IP address:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">ssh iplantusername@ip_address</pre></div></div></div>

    Example: ssh kkennedy@328.196.142.3

4.  Press**Enter**.

### Windows using PuTTY SSH login

You can use PuTTY for logging in to an SSH window on a Windows operating system. PuTTY is an SSH client for Windows, and operates a bit differently than Terminal to make the initial SSH connection. For a useful guide to using PuTTY, see[PuTTY – Remote Terminal and SSH Connectivity](http://linux.about.com/od/softinternet/a/Putty-Remote-Terminal-And-Ssh-Connectivity.htm).

1.  Copy the instance IP address, either from the confirmation email or from the IP address displayed in the My Instances list.
2.  [Download the PuTTY application](http://www.putty.org/).
3.  Launch PuTTY.
4.  Enter your iPlant username.
5.  Enter the instance IP address and then click**Connect**.
6.  Enter your password and click**Enter**.

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{tip:title=Having problems with your instance?}</div><div class="wysiwyg-macro-body">

You can[report a problem](https://pods.iplantcollaborative.org/wiki/display/atmman/Reporting+a+Broken+Instance "Reporting a Broken Instance").

</div><div class="wysiwyg-macro-tag wysiwyg-macro-endtag">{tip}</div></div><div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoFeedbackSupport}</div></div>