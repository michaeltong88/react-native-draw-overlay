
# react-native-draw-overlay
Ask for draw over other apps permission.

## Getting started

`$ npm install react-native-draw-overlay --save`

#### or

`$ yarn add react-native-draw-overlay`

## Usage
add 
```xml
<uses-permission android:name="android.permission.SYSTEM_ALERT_WINDOW"/>
```
to AndroidManifest.xml

```javascript
import DrawOverlay from 'react-native-draw-overlay';

// TODO: What to do with the module?
DrawOverlay.requestDispalayOverOtherAppsPermission()
	     .then(res => {
		 // res will be true if permission was granted 
	     })
	     .catch(e => {
		 // permission was declined
	     })
```
  
