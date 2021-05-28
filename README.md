# react-native-simple-date

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

react-native-simple-date is a beautiful and simple datepicker for react native and expo

[DEMO](https://snack.expo.io/@stealkiller06/react-native-simple-date)


## Installation
```sh
npm i react-native-simple-date
yarn add react-native-simple-date
```


## Example

```javascript
import React, { useState } from 'react';
import { StyleSheet, Text, View,ViewStyle } from 'react-native';
import DatePicker from 'react-native-simple-date'
import { Entypo } from '@expo/vector-icons'; 
export default function App() {

  const [date,setDate] = useState(new Date().toString())

  return (
    <View style={styles.container}>
      <DatePicker date={date}   
      onChange={(date)=>setDate(date)} 
      icon={<Entypo name="chevron-right" size={40} color="#689CA3" />}
      />
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center',
  },
});

```
## Properties
| Property | Description |
| ------ | ------ |
| date | Current date selected |
| icon |Icon |
| fontStyle | Input text style|
| containerStyle | Container Style |


## Events
| Property | Description |
| ------ | ------ |
| onChange | (date:string)=>void|



## License

MIT

**Free Software, Hell Yeah!**
