# React Native Workshop #2

## JavaScript

### Variables

#### `const` keyword

```javascript=
const counter = 1

const added = counter + 1
// counter => 1
// added => 2
```

### Functions

#### `function` keyword

```javascript=
function functionName(arguments) {}
```

#### arrow function syntax

```javascript=
const functionName = (arguments) => {}
```

#### object &amp; array

```javascript=
const object = { "alpha": "a", "beta": "b" }
// object.alpha => "a"
// object["beta"] => "b"

const array = [ "alpha", "beta" ]
// array[0] = "alpha"
// array[1] = "beta"
```

#### deconstruction

```javascript=
const { alpha, beta } = { "alpha": "a", "beta": "b" }
// alpha => "a"
// beta => "b"

const [ alpha, beta ] = [ "alpha", "beta" ]
// alpha => "alpha"
// beta => "beta"
```

### `export` &amp; `import`

```javascript=
// default exports
import React from 'react'

// to use it
React.createElement()

export default () => {} // name is not important

// named exports
import { createElement } from 'react'

// to use it
createElement()

export const Component = () => {}
```



## React Basics

### Everything in JavaScript

### JSX

```jsx=
const variable = 'hello'

<View prop1={props.prop1}>
    <Text>Some Text</Text>
    
    <Text>Use a variable like {variable}.</Text>
</View>
```

### Hooks

```jsx=
const Component = (props) => {
    return (
        <View prop1={props.prop1}>
            <Text>Some Text</Text>
        </View>
    )
}
```

#### `useState`

```javascript=
const [currentState, setState] = React.useState(false)

// currentState => false
// setState(true)
// currentState => true
```

```jsx=
const Component = (props) => {
    const [currentState, setState] = React.useState(false)
    
    return (
        <View show={currentState}>
            <Text>Some Text</Text>
        </View>
    )
}
```

## React Native flavoured

### `View`, `Text`

![Rendering layers](https://i.imgur.com/398xAtS.png)

### Stylesheet

```javascript=
const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center',
  },
})
```

#### Flow

- top to bottom
- Flexbox



## Next Workshop

- Get data from API
- Create a list component
- Display data into list

###### tags: `React Native` `Workshop`
