# openmw-vr-void
OpenMW VR xbps-src template for Void Linux

Install using xbps-src from void-packages repo.  
Add openmw-vr, osg-multiview and osg-multiview-devel (symlink) into srcpkgs.  
Overwrite common/shlibs.

Alternatively just clone my void-packages openmw-vr branch: https://github.com/lkroll/void-packages/tree/openmw-vr

OpenMW VR "requires" a fork of osg, using osg 3.6.5 available in the repos leads to random crashes.  
That's why we need to build our own osg.

Build osg-multiview-devel and openmw-vr, then install openmw-vr:

```bash
./xbps-src pkg osg-multiview-devel
./xbps-src pkg openmw-vr
xi openmw-vr
```

After installation and initial configuration run `openmw_vr` with your VR runtime of choice.  
Confirmed to work with SteamVR, had issues starting OpenMW VR using Monado.

If you want the latest git version use the -git template and update `_openmwvr_commit` to the commit you want to use.  
Update checksum using `xgensum -i openmw-vr`.  
Use at your own risk!

Note: Remove your regular OpenMW and OSG installation as they conflict with each other.
