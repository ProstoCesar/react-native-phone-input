# React Native Phone Input
Phone input box for React Native

![2560-02-07 01_32_33](https://cloud.githubusercontent.com/assets/21040043/22661097/aa41852e-ecd6-11e6-84da-375cbe05020f.gif)

## Installation
```
npm i react-native-phone-input --save
```

## Basic Usage
```jsx
import PhoneInput from 'react-native-phone-input'

render(){
    return(
        <PhoneInput ref='phone'/>
    )
}
```
[see full basic example](https://github.com/thegamenicorus/react-native-phone-input/blob/master/examples/BasicExample/app.js)

### Configuration
##### Properties:
| Property Name | Type | Default | Description |
|---------------|----------|-------------|----------------------------------------------------------------|
| initialCountry | string | 'us' | initial selected country |
| value | string | null | initial phone number |
| style | object | null | custom styles to be applied if supplied |
| flagStyle | object | null | custom styles for flag image eg. {{width: 50, height: 30, borderWidth:0}} |
| textStyle | object | null | custom styles for phone number text input eg. {{fontSize: 14}} |
| textProps | object | null | properties for phone number text input eg. {{placeholder: 'Telephone number'}} |
| offset | int | 10 | distance between flag and phone number |
| pickerButtonColor | string | '#007AFF' | set button color of country picker |
| pickerBackgroundColor | string | 'white' | set background color of country picker |
| pickerItemStyle | object | null | custom styles for text in country picker eg. {{fontSize: 14}} |
| cancelText | string | 'Cancel' | cancel word |
| confirmText | string | 'Cancel' | confirm word |
| buttonTextStyle | object | null | custom styles for country picker button |
| onChangePhoneNumber | function(number) | null | function to be invoked when phone number is changed |
| onSelectCountry | function(iso2) | null | function to be invoked when country picker is selected |
| onPressFlag | function() | null | function to be invoked when press on flag image |

##### Functions:
| Function Name | Return Type | Parameters | Description |
|---------------|----------|-------------|----------------------------------------------------------------|
| isValidNumber | boolean | none | return true if current phone number is valid |
| getNumberType | string | none | return true type of current phone number |
| getValue | string | none | return current phone number |
| getFlag | object | iso2:string | return flag image |
| getAllCountries | object | none | return country object in country picker |
| selectCountry | void | iso2:string | set phone input to specific country |