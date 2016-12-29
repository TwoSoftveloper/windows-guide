# TouchPad

## Inverting direction of TouchPad scroll

There is a registry setting named `FlipFlopWheel` and `FlipFlopHScroll` that does this!

`HKEY_LOCALMACHIN\SYSTEM\CurrentControlSet\Enum\HID\VID_??\VID_??\Device Parameters`

There might be multiple mouse entries. The default value for `FlipFlopWheel` and `FlipFlopHScroll` should already be 0. Change it to 1 to invert scrolling. Reboot for changes to take effect.

To get the `VID_??`:
- Go to the mouse control panel, click the Hardware tab, then click Properties.
- Now in the HID-compliant mouse Properties window click the Details tab and select the Device instance Path property. The register path is in there. You only have to reboot for this to take effect.

> Reference: http://superuser.com/questions/310681/inverting-direction-of-mouse-scroll-wheel
