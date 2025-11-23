# openmw-vr-void
OpenMW VR xbps-src template for Void Linux

Install using xbps-src from void-packages repo.
Put template file into srcpkgs/openmw-vr.

```bash
./xbps-src pkg openmw-vr
xi openmw-vr
```

After installation and initial configuration run `openmw_vr` with your VR runtime of choice.
Tested with SteamVR.

If you want the latest git version use the -git template and update `_openmwvr_commit` to the commit you want to use.
Use at your own risk!

Note: Remove your regular OpenMW installation as they conflict with each other.
