Change terminal in .profile
Add dev tools - yarn, android-studio, watchman, npm, jdk (openjdk 17)
Install react-native in project directory: yarn add react-native
Android studio: Basic install then:
Install Android 13 SDKs (show package details):
Google APIs Intel x86_64 Atom System Image
Android SDK Platform 33
Add an android 13 device
Configure vm accel:
https://developer.android.com/studio/run/emulator-acceleration?utm_source=android-studio#vm-linux
Android studio env vars:
set -Ux ANDROID_HOME $HOME/Android/Sdk
fish_add_path $ANDROID_HOME/emulator
fish_add_path $ANDROID_HOME/platform-tools
typescript-language-server, prettier, eslint
rust: rustup & rust-analyzer packages.

speed up pacman:
add the following to ~/.makepkg.conf:
`# Override extension 
PKGEXT='.pkg.tar'
# Don't use debug
OPTIONS=(strip docs !libtool !staticlibs emptydirs zipman purge !debug lto)`


hide acpi errors: add loglevel=3 to /etc/kernel/cmdline
gsimplecal
patch tuxedo-drivers
kernel-modules-hook
swaylock-effects (replace with hyprlock)
swayidle (replace with hypridle???)
redshift (but figure out how to control it)
blueman & start blueman-applet
zen kernel? (not good for laptop - higher batt use)
polkit-gnome
mako
nm-applet
dex
hyprland
hyprpaper
waybar
fuzzel
sddm (if not using gnome)
eos-sddm-theme (if not using gnome)
tuxedo drivers may need to be forked
Add github ssh key
need script for dotfiles overwrite to current dir (init then add remote)
set git config globals (can script) git config --global user.email "nickdowsett42@gmail.com" git config --global user.name "Nick Dowsett"
nerd fonts: symbols, jetbrainsmono
blueberry
endeavouros theming stuff
Warning: Not yet git cloned
# Apps
helix
fish
fisher
google-chrome
kitty
broot

# paru?
# Laptop setup
# Enable bluetooth and start it
systemctl enable bluetooth.service
systemctl start bluetooth.service
# Install Tuxedo control center
# Not currently working
yay -Syu tuxedo-control-center-bin
# install tide (need to be inside fish shell)
# note - need to delete _tide_init.fish
fisher install IlanCosman/tide@v6
# tide config doesn't seem to work.
# tide config can be run as a single command so maybe do that instead.
