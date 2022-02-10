# React Native Workshop #2

## JavaScript

### Variables

#### `const` keyword

```javascript=
const counter = 1

const added = counter + 1
// counter =&gt; 1
// added =&gt; 2
```

### Functions

#### `function` keyword

```javascript=
function functionName(arguments) {}
```

#### arrow function syntax

```javascript=
const functionName = (arguments) =&gt; {}
```

#### object &amp; array

```javascript=
const object = { &#34;alpha&#34;: &#34;a&#34;, &#34;beta&#34;: &#34;b&#34; }
// object.alpha =&gt; &#34;a&#34;
// object[&#34;beta&#34;] =&gt; &#34;b&#34;

const array = [ &#34;alpha&#34;, &#34;beta&#34; ]
// array[0] = &#34;alpha&#34;
// array[1] = &#34;beta&#34;
```

#### deconstruction

```javascript=
const { alpha, beta } = { &#34;alpha&#34;: &#34;a&#34;, &#34;beta&#34;: &#34;b&#34; }
// alpha =&gt; &#34;a&#34;
// beta =&gt; &#34;b&#34;

const [ alpha, beta ] = [ &#34;alpha&#34;, &#34;beta&#34; ]
// alpha =&gt; &#34;alpha&#34;
// beta =&gt; &#34;beta&#34;
```

### `export` &amp; `import`

```javascript=
// default exports
import React from &#39;react&#39;

// to use it
React.createElement()

export default () =&gt; {} // name is not important

// named exports
import { createElement } from &#39;react&#39;

// to use it
createElement()

export const Component = () =&gt; {}
```



## React Basics

### Everything in JavaScript

### JSX

```jsx=
const variable = &#39;hello&#39;

&lt;View prop1={props.prop1}&gt;
    &lt;Text&gt;Some Text&lt;/Text&gt;
    
    &lt;Text&gt;Use a variable like {variable}.&lt;/Text&gt;
&lt;/View&gt;
```

### Hooks

```jsx=
const Component = (props) =&gt; {
    return (
        &lt;View prop1={props.prop1}&gt;
            &lt;Text&gt;Some Text&lt;/Text&gt;
        &lt;/View&gt;
    )
}
```

#### `useState`

```javascript=
const [currentState, setState] = React.useState(false)

// currentState =&gt; false
// setState(true)
// currentState =&gt; true
```

```jsx=
const Component = (props) =&gt; {
    const [currentState, setState] = React.useState(false)
    
    return (
        &lt;View show={currentState}&gt;
            &lt;Text&gt;Some Text&lt;/Text&gt;
        &lt;/View&gt;
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
    backgroundColor: &#39;#fff&#39;,
    alignItems: &#39;center&#39;,
    justifyContent: &#39;center&#39;,
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
