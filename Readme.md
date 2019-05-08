# Get Started

```
ln -s /Users/edki/Desktop/launchdaemonexample/im.eddiek.hello.plist /Users/edki/Library/LaunchAgents/im.eddiek.hello.plist
```

# launchctl

## List Jobs

```
sudo launchctl list
```

## Blame

```
launchctl blame system/com.example.app.plist (for launch daemon)
```

## Load/Unload

```
launchctl load ~/Library/LaunchAgents/com.example.app.plist
launchctl unload ~/Library/LaunchAgents/com.example.app.plist
```

## Start/Stop

```
launchctl start com.example.app
launchctl stop com.example.app
```

## Debug

```
sudo launchctl debug gui/$UID/im.eddiek.hello --stdout --stderr
```

# Debugging

## Lint the Plist

plutil -lint com.example.app.plist

# Reference

* [Daemons and Services Programming Guide](https://developer.apple.com/library/archive/documentation/MacOSX/Conceptual/BPSystemStartup/Chapters/Introduction.html#//apple_ref/doc/uid/10000172i-SW1-SW1)
* [Technical Note TN2083: Daemons and Agents](https://developer.apple.com/library/archive/technotes/tn2083/_index.html#//apple_ref/doc/uid/DTS10003794-CH1-SECTION30)
* [plist file permissions](https://stackoverflow.com/questions/28063598/error-while-executing-plist-file-path-had-bad-ownership-permissions)
