# react-google-static-map

Google Static Maps Component for React

Most of the code is from https://github.com/yelled3/react-native-google-static-map

## Installation
```
npm install --save react-google-static-map
```
## Usage
```js
var GoogleStaticMap = require('react-google-static-map');

class MapExample extends React.Component {
  render() {
    return (
        <GoogleStaticMap
            style={styles.map} {...locationProps}
            latitude={'32.064171'}
            longitude={'34.7748068'}
            zoom={13}
            size={{ width: 300, height: 550 }}
        />
    );
  }
}
```
## Props
| Prop | Type | Description |
|---|---|---|
|**`latitude`**|`string`|latitude point.|
|**`longitude`**|`string`|longitude point.|
|**`size`**|`object`| the image size - `{ width: 300, height: 550 }`|
|**`zoom`**|`number`|defines the zoom level of the map.|
|**`scale`**|`number`|scale=2 returns twice as many pixels as scale=1. The default value is calculated from the screen `PixelRatio`. |
|**`format`**|`string`|'png', 'png32', 'jpg', 'gif', 'jpg-baseline'. use the `GoogleStaticMap.ImageFormats` enum. default is `png`.|
|**`mapType`**|`string`|'roadmap', 'satellite', 'terrain', 'hybrid'. use the `GoogleStaticMap.MapTypes` enum. default is `roadmap`.|
|**`hasCenterMarker`**|`bool`|add a marker on the center. default is `true`.|
