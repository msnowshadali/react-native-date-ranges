
# react-native-date-ranges

## Getting started

`$ npm install react-native-date-ranges --save`

![alt text](https://raw.githubusercontent.com/pohsiu/react-native-date-ranges/master/ezgif.com-video-to-gif.gif)

## Usage
```javascript
import DatePicker from 'react-native-date-ranges';

//range picker
<DatePicker
	style={ { width: 350, height: 45 } }
	customStyles = { {
		placeholderText:{ fontSize:20 } // placeHolder style
		headerStyle : {  },			// title container style
		headerMarkTitle : { }, // title mark style 
		headerDateTitle: { }, // title Date style
		contentInput: {}, //content text container style
		contentText: {}, //after selected text Style
	} } // optional 
	centerAlign // optional text will align center or not
	allowFontScaling = {false} // optional
	placeholder={'Apr 27, 2018 → Jul 10, 2018'}
	mode={'range'}
/>

//single picker
<DatePicker
	style={ { width: 350, height: 45 } }
	customStyles = { {
		placeholderText:{ fontSize:20 }, // placeHolder style
		headerStyle : {  },			// title container style
		headerMarkTitle : { }, // title mark style 
		headerDateTitle: { }, // title Date style
		contentInput: {}, //content text container style
		contentText: {}, //after selected text Style
	} } // optional 
	centerAlign // optional text will align center or not
	allowFontScaling = {false} // optional
	placeholder={'Apr 27, 2018'}
	selectedBgColor="black"
	selectedTextColor="blue"
/>
```
  
## Props
| Prop | Type | Description |
:------------ |:---------------| :-----|
| **`placeholder`** | `String` | optional. |
| **`customStyles`** | `Object` | optional. customize style e.g.({ placeholderText:{}, headerStyle:{} ... }) |
| **`style`** | `Object` | Optional. date picker's style |
| **`onConfirm`** | `Function` | Optional. call function after click button, that would return a date object {startDate:'', endDate:''} e.g( value=>console.log(value))|
| **`selectedBgColor`** | `String` | Optional. custom your selected date background color e.g {"black"} |
| **`selectedTextColor`** | `String` | Optional. custom your selected date text color e.g {"black"} |
| **`ButtonStyle`** | `Object` | Optional. custom your save button container style |
| **`ButtonTextStyle`** | `Object` | Optional. custom your save button Text style  |
| **`returnFormat`** | `String` | Optional. custom your datetime format e.g.('YYYY/MM/DD') at onConfirm |
| **`headFormat`** | `String` | Optional. custom your datetime format showing at headBlock e.g.('YYYY/MM/DD')|
| **`outFormat`** | `String` | Optional. custom your datetime format showing at outline touchable filed e.g.('YYYY/MM/DD')|
| **`mode`** | `String` | one of ['range', 'single'] , default as single|
....
