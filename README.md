# Electron DevTools Offline Installer

> Base on [electron-devtools-installer](https://github.com/GPMDP/electron-devtools-installer), add offline extensions folder install support.

## Why

Because in somewhere can not connect ChromeStore, so add offline install support.

The `extensions` folder is store extensions file. When install extensions, will looking for the folder, if doesn't exits then connect ChromeStore to download.

## Install

    $ npm install electron-devtools-install-offline --save-dev

## Usage

```js
import installExtension, { REACT_DEVELOPER_TOOLS } from 'electron-devtools-installer';

installExtension(REACT_DEVELOPER_TOOLS)
```

## API

**installExtension(chromeStoreID, forceDownload=false)**

Install DevTool extensions into Electron.

- `chromeStoreID` is ChromeStore ID of the extension
- `forceDownload` set true will ignore the offline extensions files.

**EMBER_INSPECTOR/REACT_DEVELOPER_TOOLS/ANGULARJS_BATARANG/VUEJS_DEVTOOLS/REDUX_DEVTOOLS**

This DevToll extensions are all download already in extensions folder, so you can install these extensions offline.