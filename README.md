# gnome-shortcuts

gsettings get org.gnome.settings-daemon.plugins.media-keys custom-keybindings (list custom-keybindings)


gsettings set org.gnome.settings-daemon.plugins.media-keys custom-keybindings "['/org/gnome/settings-daemon/plugins/media-keys/custom-keybindings/custom0/', '/org/gnome/settings-daemon/plugins/media-keys/custom-keybindings/custom1/', '/org/gnome/settings-daemon/plugins/media-keys/custom-keybindings/custom2/']" (Create 3 empty bindings)

gsettings set org.gnome.settings-daemon.plugins.media-keys.custom-keybinding:/org/gnome/settings-daemon/plugins/media-keys/custom-keybindings/custom0/ name 'gnome-terminal'(Setting name of shortcut)

gsettings set org.gnome.settings-daemon.plugins.media-keys.custom-keybinding:/org/gnome/settings-daemon/plugins/media-keys/custom-keybindings/custom0/ command 'gnome-terminal'(Setting command of shortcut)

gsettings set org.gnome.settings-daemon.plugins.media-keys.custom-keybinding:/org/gnome/settings-daemon/plugins/media-keys/custom-keybindings/custom0/ binding '<Alt>c' (Setting the shortcut keys)
  
  
# Saving key bindings:
  dconf dump /org/gnome/settings-daemon/plugins/media-keys/custom-keybindings/ > apni_custom_key_bindings.txt
  
# Loading key bindings
  dconf load /org/gnome/settings-daemon/plugins/media-keys/custom-keybindings/ < apni_custom_key_bindings.txt

Note: th directory path might be different on different systems 
