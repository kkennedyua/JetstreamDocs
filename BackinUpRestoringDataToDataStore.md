<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>
# Backing up and restoring volume data to the Data Store

<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{toc}</div></div>
## Backing up data from an instance to the Data Store

1.  To start the backup process, execute the following in a terminal window under your iPlant account:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">$iplant_backup</pre></div></div></div>
2.  In the following prompt, enter**backup**:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">Do you want to backup or restore local instance/volume data?[backup/restore]: backup</pre></div></div></div>
3.  In the following prompt, enter the**full path to your local directory or file for the instance**:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">Specify local file/directory's full path on the instance [eg: /home/username, /home/username/file.txt]: /home/username/Desktop</pre></div></div></div>
4.  In the following prompt, enter the**full path of the directory or file in the Data Store to which you want to back up the data**:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">Specify file/directory path on iPlant datastore [eg: /iplant/home/username, /iplant/home/username/file.txt] [Default is /iplant/home/username/atmosphere]: /iplant/home/username/atmosphere/test.sh</pre></div></div></div>

    The default option for this step is**/iplant/home/<username>/atmosphere**. If the**atmosphere** directory does not exist, it will be created and the data will be stored there.

5.  Enter your iPlant paswword to begin the backup request.

## Restoring data from the Data Store to an instance

1.  To start the restore process, execute the following in a terminal window under your iPlant account:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">$iplant_backup</pre></div></div></div>
2.  In the following prompt, enter**restore**:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">Do you want to backup or restore local instance/volume data?[backup/restore]: restore</pre></div></div></div>
3.  In the following prompt, enter the**full path of the directory or file in the Data Store to which you want to restore the data**:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">Specify file/directory path on iPlant datastore [eg: /iplant/home/username, /iplant/home/username/file.txt]: /iplant/home/username/atmosphere/test.sh</pre></div></div></div>
4.  In the following prompt, enter the**full path to your local directory or file for the instance**:<div class="wysiwyg-macro"><div class="code panel" style="border-width: 1px;"><div class="codeContent panelContent"><pre class="theme: Default; brush: java; gutter: false">Specify local file/directory's full path on the instance [eg: /home/username, /home/username/file.txt]: /home/username/Desktop</pre></div></div></div>
5.  Enter your iPlant password to begin the restore process.