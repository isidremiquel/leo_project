# leo_project
enable/disable touchpadOff synclient's variable in openbox linux

copy touchpadOnOff.sh in /usr/bin/ and make it executable.
remember! you need root permissions to do it!

copy code below inside /home/your_user/.config/openbox/rc.xml


<!-- Keybindings for desktop switching -->
    <!--TODO for fn keys-->
    <!--"XF86Display" allows in my laptop to use fn+f3 -->
    <!-- you must figure out your own key -->

    <keybind key="XF86Display">
      <action name="Execute">
        <startupnotify>
          <enabled>true</enabled>
          <name>on-off-touchpad</name>
        </startupnotify>
        <command>cb-touchpadOff</command>
      </action>
    </keybind>
