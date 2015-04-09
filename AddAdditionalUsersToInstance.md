# Adding users to an instance

You can add additional users to an instance. The new user must be a[registered iPlant user](https://pods.iplantcollaborative.org/wiki/display/start/Registering+for+an+iPlant+Account "Registering for an iPlant Account").

1.  If necessary,[connect to your instance via SSH](https://pods.iplantcollaborative.org/wiki/display/atmman/Logging+In+to+an+Instance "Logging In to an Instance").
2.  Log in as the root user and enter your iPlant password when prompted, to be given root privileges:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">sudo su -</pre></div></div></div>
3.  Open the**/etc/group** file:
    1.  Find the line listing all users who belong to the**users** group. In most cases, this will be your userid (e.g.,_jane_).
    2.  Enter the following command, substituting your userid for_jane_, as in the following example:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">users:x:100:jane,</pre></div></div></div>
    3.  Add the new username to the end of the line, substituting the new username for_henri_, as in the following example:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">users:x:100:jane,henri</pre></div></div></div>
4.  Repeat for each additional user to add to the instance.
5.  When done, save the changes and exit the file.

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoFeedbackSupport}</div></div>