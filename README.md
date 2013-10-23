pavol
=====

PulseAudio volume control from the command line. Controls all inputs simultaneously. Would be simple to control them separetely (just needs another flag, and a thing at the bottom to honor it), patches welcome.


Openbox key bindings
===================

Add to `~/.config/openbox/rc.xml`

    <!-- Volume keys -->
    <keybind key="XF86AudioRaiseVolume">
      <action name="Execute">
        <command>pavol +</command>
      </action>
    </keybind>
    <keybind key="XF86AudioLowerVolume">
      <action name="Execute">
        <command>pavol -</command>
      </action>
    </keybind>
    <keybind key="XF86AudioMute">
      <action name="Execute">
        <command>pavol !</command>
      </action>
    </keybind>


Fluxbox key bindings
===================

Add to `~/.fluxbox/keys`

    None XF86AudioRaiseVolume :execCommand pavol +
    None XF86AudioLowerVolume :execCommand pavol -
    None XF86AudioMute :execCommand pavol !
