# rmc-date-picker
---

React Mobile DatePicker Component (web and react-native)


[![NPM version][npm-image]][npm-url]
![react-native](https://img.shields.io/badge/react--native-%3E%3D_0.30.0-green.svg)
![react](https://img.shields.io/badge/react-%3E%3D_15.2.0-green.svg)
[![build status][travis-image]][travis-url]
[![Test coverage][coveralls-image]][coveralls-url]
[![gemnasium deps][gemnasium-image]][gemnasium-url]
[![node version][node-image]][node-url]
[![npm download][download-image]][download-url]

[npm-image]: http://img.shields.io/npm/v/rmc-date-picker.svg?style=flat-square
[npm-url]: http://npmjs.org/package/rmc-date-picker
[travis-image]: https://img.shields.io/travis/react-component/m-date-picker.svg?style=flat-square
[travis-url]: https://travis-ci.org/react-component/m-date-picker
[coveralls-image]: https://img.shields.io/coveralls/react-component/m-date-picker.svg?style=flat-square
[coveralls-url]: https://coveralls.io/r/react-component/m-date-picker?branch=master
[gemnasium-image]: http://img.shields.io/gemnasium/react-component/m-date-picker.svg?style=flat-square
[gemnasium-url]: https://gemnasium.com/react-component/m-date-picker
[node-image]: https://img.shields.io/badge/node.js-%3E=_0.10-green.svg?style=flat-square
[node-url]: http://nodejs.org/download/
[download-image]: https://img.shields.io/npm/dm/rmc-date-picker.svg?style=flat-square
[download-url]: https://npmjs.org/package/rmc-date-picker

## Screenshots

### web

<img src="https://img.alicdn.com/tps/TB1nH_4KpXXXXaCXFXXXXXXXXXX-404-607.png" width="288"/>

### ios

<img src="https://img.alicdn.com/tps/TB1saD1KpXXXXb_XFXXXXXXXXXX-420-729.png" width="288"/>

### android

<img src="https://img.alicdn.com/tps/TB1APgXKpXXXXXZXpXXXXXXXXXX-1920-1080.png" width="400"/>

## Usage

see example

config webpack to resolve .web.js

```
resolve: {
  extensions: ['', '.web.tsx', '.web.ts', '.web.jsx', '.web.js', '.ts', '.tsx', '.js', '.jsx', '.json'],
},
```

## Development

```
npm i
npm start
```

## Example

http://localhost:8000/examples/

online example: http://react-component.github.io/m-date-picker/

## react-native

```
npm run watch-tsc
./node_modules/rc-tools run react-native-init
react-native run-ios
```

## install

[![rmc-date-picker](https://nodei.co/npm/rmc-date-picker.png)](https://npmjs.org/package/rmc-date-picker)


## API

### DatePicker props

| name     | description    | type     | default      |
|----------|----------------|----------|--------------|
|className(web) | additional css class of root dom node | String | '' |
|prefixCls(web) | prefix class | String | 'rmc-date-picker' |
|pickerPrefixCls(web) | picker prefix class | String | 'rmc-picker' |
|defaultDate | default selected date. | moment | |
|date | The currently selected date. | moment |  |
|mode | The date picker mode. | String | 'date' enum('date', 'time', 'datetime') |
|minDate | min date | moment | 2000-1-1 |
|maxDate | max date | moment | 2030-1-1 |
|locale | the locale of area | Object | import from 'rmc-date-picker/lib/locale/en_US' |
|onDateChange | Date change handler. | Function(date: moment) | '' |
|minuteStep | The amount of time, in minutes, between each minute item. | Number | 1 |
|formatMonth | Customize display value of months | (month:number, current:moment) => React.Node | |
|formatDay | Customize display value of days | (day:number, current:moment) => React.Node | |

### rmc-date-picker/lib/Popup props

| name     | description    | type     | default      |
|----------|----------------|----------|--------------|
|className(web) | additional css class of modal node | String | '' |
|style(web) | additional modal style | object | {} |
|popupTransitionName(web) |  | String | |
|maskTransitionName(web) |  | String | |
|prefixCls(web) | popup's prefix class | String | 'rmc-picker-popup' |
|styles(react-native) | PopupPicker's styles | StyleSheet.create |  |
|datePicker | DatePicker element | React DatePicker element |  |
|date | The currently selected date. | moment |  |
|visible | whether pop picker is visible | Boolean | false |
|onChange | exec on ok | Function(date: moment) |  |
|onVisibleChange | called when pop picker visible change | Function | |
|onDismiss | exec on dismiss | function |  |
|okText | ok button text | string/React.ReactElement | 'Ok' |
|dismissText | dismiss button text | string/React.ReactElement | 'Dismiss' |
|title | Popup title | string/React.ReactElement | '' |


## Test Case

```
npm test
npm run chrome-test
```

## Coverage

```
npm run coverage
```

open coverage/ dir

## License

rmc-date-picker is released under the MIT license.
