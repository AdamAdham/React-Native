# React-Native-Notes
Renders **Native** components instead of html components like react js <br>

**<View>**: Container which uses flexbox
**<Text>**: Used instead of h1 or p 
```jsx
import React from 'react'
import {View, Text} from 'react-native
const App () => {
return (
<View>
<Text> Hello World! </Text>
</View>
```

### TouchableOpacity
Interactive element that fades in opacity when touched (like a button)

```jsx
import { TouchableOpacity, Text } from 'react-native';
function MyButton(props) {
return (
<TouchableOpacity onPress={props.onPress}>
<Text>{props.label} </Text>
</TouchableOpacity>
```

### TouchableHighlight
Interactive element reacting in a unique way

### TouchableWithoutFeedback
Self explanatory

### ActivityIndicator
A spinner to indicate loading

### Button
Self explanatory

### FlatList
**Long** list of elements to be scrolled in (like the map function)

_Extra Features:_ 
- Optimized Scroll Performance
- Item Seperation

### ScrollView
It is like a magic box that can hold multiple components and views, providing a scrolling container for them. (overflow:scroll)


### SafeAreaView
To allow all content to be viewed regardless of screen
```jsx
import SafeAreaView from 'react-native-safe-area-context'
```
### Image
Display an image

### ImgBackground
To display image as background

### Modal
Like a popup

```jsx
import { Modal, Text,View } from 'react—native';

const App = () =>(
<Modal
visible={true}
animationType='slide'
onRequestClose={()-> console.log("close")}
>
  <View style={{flex:1,justifyContent:'center',alignltems:'center'}}>
    <Text> This is a modal</Text>
  </View>
</Modal>
```

### Alert
A popup

```jsx
import {Modal, Text, View } from 'react-native';
const App ) (= )
  <Modal
  visible={true}
  animationType="slide"
  onRequestClose={() ⇒ console.log('Modal closed')}
    <View style={{ flex: 1, justifyContent: 'center', alignItems:
    'center' }}>
      <Text>This is a modal</Text>
    </View>
  </Modal>
);
export default App
```
### Switch
A toggle

```jsx
import { Switch, View } from 'react-native';
const App = () => {
  const [isEnabled, setIsEnabled] ▪ useState(false);
  const toggleSwitch ()setIsEnabled (previous State ⇒
  !previousState);
  return (
    <View>
      <Switch
        trackColor={{ false: '#767577', true: '#81b0ff' }}
        thumbColor={isEnabled ? '#f5dd4b': '#f4f3f4'}
        onValueChange (toggleSwitch)
        value {isEnabled}
      />
    </View>
  );
  };
export default App
```

### StatusBar
To control the appearance top of the screen
