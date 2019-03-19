# Code for device detection

The code on this folder was created for detecting the connection and disconnection events
of the device. The code is not used due to compatibility issues with Electron, but it
remains here just in case it is useful in the future. There is no documentation, so it may be
necessary to tests several things to make it work.

## Deleted code

The following dependency, used by this code, was removed from `package.json`:

```
"usb": "^1.3.3"
```

Also, the following script was removed from `package.json`:

```
"make-device-detection": "./node_modules/.bin/babel ./device-detection/*.js ./device-detection/hw-transport/*.js -d device-detection-lib/",
```

For that script to work, it could be necessary to add `"babel-polyfill": "^6.26.0"` to the dependencies
on `package.json`. Also some (or all) of the following dev dependencies may be needed:

```
"babel-cli": "^6.26.0",
"babel-plugin-add-module-exports": "^1.0.0",
"babel-plugin-transform-runtime": "^6.23.0",
"babel-preset-env": "^1.7.0",
"babel-preset-es2015": "^6.24.1",
"babel-preset-flow": "^6.23.0",
"babel-preset-stage-0": "^6.24.1",
```
