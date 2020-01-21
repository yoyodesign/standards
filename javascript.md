# Yoyo JavaScript standards

## Contents

1. [Whitespace](#whitespace)
2. [Variables](#variables)

## Whitespace

### Space before opening brace, newline before closing brace

```javascript
// Bad :(
function noop(){
	return;
}

// Worse :'(
function noop()
{
	return;
}

// Good :)
function noop() {
	return;
}
```

## Variables

### Use `const`

Use `const` (instead of `let`) when a variable is not going to change.

```javascript
// Bad :(
function add(a, b) {
	let result = a + b;
	return result;
}

// Good :)
function add(a, b) {
	const result = a + b;
	return result;
}
```

### Variable names

Constants should be UPPERCASE:

```javascript
const URL = "https://yoyodesign.com/";
```

Collections of constants should be TitleCase:

```javascript
const UrlParams = {
	START = "start",
	SIZE = "size"
};
```