# react-native-cyberpunk-button
Button with glitch display effect inspired by cyberpunk 2077 game webpage. Button is styled to resemble component on [cyberpunk web page](https://www.cyberpunk.net/).
Button component is highly customisable. You can change animation params, button and text style.


![](Example/)

# Usage
Install module:
```
npm install --save react-native-cyberpunk-button
```

or

```
yarn add react-native-cyberpunk-button
```

Import button and use it in your app:
```js
import CyberButton from 'react-native-cyberpunk-button';

export default function App() {
  return (
    <View>
      ...
      <CyberButton label="cyberpunk_"  buttonHeight={80}/>
    </View>
  );
}
```

# CybeButton props
| Props                | Type          | Description  | Default      |
| --------------------- |:-------------:| ------------ | ------------ |
| `height` | `Integer`     | Height of the button. |`80` |
| `label`  | `string` | Button text.| `''` |
| `mainColor`  | `string` | Button background.| `#ff003c` |
| `shadowColor`  | `string` | Glitch effect shadow and borders.| `#add8e6` |
| `disableAutoAnimation`  | `boolean` | Disable animation autoplay.| `false` |
| `glitchDuration`  | `number` | Duration of glitch animation (lower value means faster blinking).| `1500` |
| `glitchAmplitude`  | `number` | Size of horizontal (X axis) glitch swing.| `5` |
| `repeatDelay`  | `number` | Delay before animation auto replay.| `2000` |
| `labelContainerStyle`  | `object` | Styles to be applied to label container.| |
| `labelTextStyle`  | `object` | Styles to be applied to label text component.| |
\
Default label container style:
```
{
  height: buttonHeight,
  paddingRight: buttonHeight /  2,
  paddingLeft: buttonHeight / 4,
  borderColor: shadowColor,
  backgroundColor: mainColor,
  borderRightWidth: 2,
  alignItems: 'center',
  justifyContent: 'center',
}

```

Default label text style:
```
{
  color: '#ffffff',
  fontWeight: 'bold',
  letterSpacing: 3,
  fontSize: buttonHeight / 2.5
}
```

# React Native Epicode Academy
This package is a part of [React Native Epicode Academy](https://www.youtube.com/channel/UCjeodJlopQe4b91Y-uS18Ow) YouTube series.