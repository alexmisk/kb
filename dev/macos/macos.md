### Create a bootable installer for macOS
`sudo /Applications/Install\ macOS\ Catalina.app/Contents/Resources/createinstallmedia --volume /Volumes/<**VOLUME**>`


### Disable font smoothing
`defaults -currentHost write -g AppleFontSmoothing -int 0`