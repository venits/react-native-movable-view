# React Native Movable View

Simple component that make your views movable.

It is using PanResponder so it is **performance friendly :)**


### Installation
```javascript
npm install react-native-movable-view --save
```
### Demo


### Usage
1. Import:
```javascript
import MovableView from 'react-native-movable-view'
```
2.  Wrap your views:
```javascript
<MovableView>
	{views_you_want_to_be_movable}
</MovableView>
```
3. That's all. Now you can restart your app and enjoy movable view ;) 

*Example:*
```javascript
<MovableView>
	<View style={{
		width: 60, height: 60,
        backgroundColor:'red',
        borderRadius: 30 }} 
    />
</MovableView>
```

### Callbacks

**MovableView** contains 3 basic callbacks so you can have move control about what is happening.

*Example of getting x and y coordinates of our view:*
```javascript
 <MovableView
   onMove={ values => console.warn(values) } > 
   ...
 </MovableView>
```

*Table of all available callbacks:*

|Name|Note|
|---|---|
| onDragStart | Executed when user starts dragging object around | 
| onDragEnd | Executed when user stops dragging. | 
| onMove | Executed when user is dragging view. **Returns current position of view.**  | 

### Support
In case of any problem or more custom solution you can email me at:
 
tomasz.przybyl.it@gmail.com

**I hope you will find this module useful. Happy Coding :)**

