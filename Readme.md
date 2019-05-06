# Get Started

```
ln -s /Users/edki/Desktop/launchdaemonexample/im.eddiek.hello.plist /Users/edki/Library/LaunchAgents/im.eddiek.hello.plist
```

# launchctl

## List Jobs

```
launchctl list
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