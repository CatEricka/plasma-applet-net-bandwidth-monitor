![1a](https://user-images.githubusercontent.com/72889808/217653034-4ed63b12-875b-4001-84f7-b3159d933a99.png)

# plasma-applet-net-bandwidth-monitor
Network bandwidth monitor for plasma using dbus


Plasma 5 widget that displays network bandwidth data. Built upon the foundations of the excellent work by dfaust and bstrong5280:

https://github.com/dfaust/plasma-applet-netspeed-widget/  |  https://www.opencode.net/bstrong5280/system-monitor-plasmoid

I've taken the UI element from netspeed-widget and the dbus workings from system-monitor, glued them together and added a few additional UI nice to haves. This widget doesn't need ksysguard to function.
This is extremely BETA software and the first plasma widget I've done. If you find something or many things that aren't working, let me know and I'll take a look when I can.


## v0.3.1:
Small fix release to corrected issue with multiple decimal fraction digits being shown when using 'Update Interval' above 1 second and using 'Average' or 'Accumulated' for Interval data relay options.  Had some issue with compiling so made some modification's to CMakeLists.txt file. Added CatEricka edits to configGeneral.qml (staging for translations) and setup my IDE and GitHub for correct source control.


## v0.3.2: 
Added a small fix for when unchecking all networks the UI didn't update to reflect with 0. It now forces one final update to reset the UI. Added the foundation for translations and added zh_CN translation files - thanks to CatEricka for providing.  Corrected many spelling mistakes! Words are hard.


## v0.3.3:
Update to the translations.  Fixed issue with UI text and icon alignment in Horizontal layout.  Added code to disable padding selection in Horizontal mode.  Doubled padding option from 10 to 20. 



Thanks to all those that feedback their experiences using the widget and the thanks received.


## IF EXPERIENCING ISSUES AFTER INSTALL / UPGRADE:
When upgrading via the Plasma 'get widgets' section, make sure you have the new version in the 'about' section.  If in doubt, download the .plasmoid and install via commandline with ``` plasmapkg2 -i /PATH/xxx.plasmoid ```.  Once installed, I've found its a good idea to reboot or log out and in again, it seems to refresh the serialized stored settings.


## OPTIONS:
- Layout
- Display Order
- Show speeds separately
- Font size
- Update interval
- Interval data relay
- Layout Padding
- Hide when inactive
- Show speed units
- Speed units
- Shorten speed units 
- Show speed icons
- Show 'per seconds' suffix -- NEW
- 'Per seconds' prefix -- NEW
- Icon style
- Icon position
- Numbers [binary, metric]
- Decimal place
- Monitor individual or multiple interfaces


## TODO:
- Main options:
    - shrink area on taskbar when hidden
    - minimum activity for hidden
    - Translations
- ToolTip options:
    - Show ToolTip 
    - Show bandwidth Totals
    - Bandwidth Units
    - Show Interface name
    - Show IP address
    - Show additional IP info
    - Show Icon
    - Icon option (Wired, Wireless, Globe)
    - Show WiFi signal strength

## TO FIX:
- Settings window can be resized over page elements, doesn't do it in 'plasmoidviewer' environment. Is this normal?



## SCREENSHOTS
![4](https://user-images.githubusercontent.com/72889808/209709200-9f4c045e-2b54-4fb3-9758-62c4096e8fc9.png)

![A](https://user-images.githubusercontent.com/72889808/217652964-20a0556a-a403-40e5-9e54-5a49bdb83fd5.png)

![1](https://user-images.githubusercontent.com/72889808/209696486-0419dd51-f7c8-47a4-aba6-1f2fc4590812.png)

![B](https://user-images.githubusercontent.com/72889808/217652736-9e8c7d27-d5eb-486f-ab66-e8bcc28b87ca.png)

![C](https://user-images.githubusercontent.com/72889808/217652754-07799096-c390-4bde-a974-8632371cd54d.png)

![D](https://user-images.githubusercontent.com/72889808/217654861-3e6d21ac-91bd-41eb-a592-5aedf321624b.png)


