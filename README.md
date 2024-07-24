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

### ActivityIndicator
A spinner to indicate loading
