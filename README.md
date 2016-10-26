# Whitelist
Whitelist homebrew for PSVita/PSTV (based on AntiBlacklist by Rinnegatamante)

This is a fork of Rinnegatamante's AntiBlacklist which implements both v1 and v2 whitelist patches on the PSVita/PSTV.

Some of the new changes are disruptive; it seemed safer to rename the application so that both can be installed side by side. 

2016-10-26 (1.21)
- now tests for installed v1 patch
- now tests for installed v2 patch
- can now reinstall on ur0 without reboot (partially fixes undesired behavior introduced in 1.20)
- consolidated v2 install/uninstall under circle
- introduced initial Status Pane on main menu
- added button graphics
- created new icon0, startup, and bg images
- breadcrumb trail navigation
- instruction changes to support patch install states
- included sqlite-3.6.23.1 (workaround for msys2 under Windows where sqlite was installed but the project did not build)
- added unrelated memory card swap function (mainly for convenience) using square
- minor text changes
- some makefile changes

2016-09-26 (1.20)
- vitarw integration for v1 patch

2016-09-26 (1.12)
- changed blacklist values to the correct versions installed under 3.60

Additional notes: 
I'm still not aware of a reliable way to remount vs0 so a reboot is necessary when patching v1 on vs0.
With the new checks (if v1 vs0 is already applied) you can re-install v1 on ur0 without this inconvenience.

Could use some help with:
- A safe way to remount vs0 without rebooting
- including statically compiled images in a sub-directory (which is why they are in the root >.>)
