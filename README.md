# CivicSource `react-jss` Preset

> Shareable [`react-jss`](https://github.com/cssinjs/react-jss) preset to be used in CivicSource client applications

## Install

```
npm install react-jss-preset-civicsource -S
```

## Usage

```jsx
import useSheet from "react-jss-preset-civicsource";

const styles = {
	fancy: {
		outline: "3px solid #0f0"
	}
};

const Widget = ({
	children,
	sheet: { classes },
	...props
}) => (
	<div {...props}>
		<div className={classes.fancy}>
			{children}
		</div>
	</div>
);

export default useSheet(Widget, styles, { meta: __filename });

```


### Versioning

When making changes, be sure to [follow semantic versioning](http://semver.org/).

* Any change to this preset or any of its dependencies which alters the signature of `useSheet` should be a major version bump.