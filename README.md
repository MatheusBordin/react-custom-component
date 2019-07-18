# React Custom Componentis
Use web-components inside React application without issues.

## Usage
```javascript
import connectCustom from 'react-custom-component';

const CustomComponent = connectCustom('custom-component', ['custom-event']);

const App = (props) => (
	<CustomComponent onCustomEvent={() => console.log('make it works')} />
);
```

## API

#### connectCustom(tag: string, events: string[])
React component wrapper for custom-components. Resolve issues like: custom event triggers, object attribute values parser.

##### Arguments

| Properties | Description                            | Required |
| ---------- | -------------------------------------- | -------- |
| tag        | Custom component tag name              | Yes      |
| events     | Custom events used by custom component | Yes      |
