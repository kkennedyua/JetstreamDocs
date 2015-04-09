<div class="wysiwyg-macro"><div class="wysiwyg-macro-tag wysiwyg-macro-starttag">{include:docs:_AtmoRelease_AtmoBetaUI}</div></div>
# Installing binaries, storing data, and using the Data Store in Atmosphere

You can install binaries and store your iPlant Data Store data in Atmosphere.

## Installing binaries

Install your tool binaries in<tt>/usr/local/bin/</tt>

## Storing your data

To retrieve your data in the future, store your data in<tt>/mydata</tt>, where you have[mounted your volume](https://pods.iplantcollaborative.org/wiki/display/atmman/Attaching+a+Volume+to+an+Instance "Attaching a Volume to an Instance").

## Using your iPlant Data Store in Atmosphere

There are three ways to access data from the iPlant Data Store (iDS):

*   **Use FUSE to mount the Data Store:** For direct-file system-based access where your data appears as a drive on your instance, see[Using FUSE to mount the iPlant Data Store](https://pods.iplantcollaborative.org/wiki/display/DS/Using+FUSE+to+Mount+the+iPlant+Data+Store "Using FUSE to Mount the iPlant Data Store"). Although not a high-throughput method, this method does not require modifications to your existing programs.[Using iDrop Desktop](https://pods.iplantcollaborative.org/wiki/display/DS/Using+iDrop+Desktop "Using iDrop Desktop")  

*   **Use iCommands or iDrop to copy the data to your instance:**
    *   [iCommands](https://pods.iplantcollaborative.org/wiki/display/DS/Using+iCommands "Using iCommands") is preinstalled on all Atmosphere instances, so you only need to type**iinit** to get started.
    *   If you need GUI access,[iDrop](https://pods.iplantcollaborative.org/wiki/display/DS/Using+iDrop+Desktop "Using iDrop Desktop") is preinstalled on most Atmosphere images that have VNC-based access.  

        If you do not have sufficient disk space on your instance, you will need to[mount additional space](https://pods.iplantcollaborative.org/wiki/display/atmman/Using+Volumes "Using Volumes").  
        You can also use the iRODS[irsync](https://www.irods.org/index.php/irsync) command to synchronize data between your instance and the Data Store.

*   **Use Parrot (for advanced users only):** Advanced users may use[Parrot](http://www3.nd.edu/%7Eccl/software/parrot/), a higher-performance method than FUSE-based access. Parrot requires additional setup; please contact[iPlant Support](mailto:support@iplantcollaborative.org) for assistance.