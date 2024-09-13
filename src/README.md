# @beyond-js/ports

A simple utility package to check if a port is available on the system.

## Installation

Install the package using npm:

```bash
npm install @beyond-js/ports
```

## Usage

Here's a basic example of how to use the `@beyond-js/ports` package:

```javascript
const ports = require('@beyond-js/ports');

async function checkPort(port) {
	const isAvailable = await ports.check(port);
	console.log(`Port ${port} is ${isAvailable ? 'available' : 'in use'}`);
}

checkPort(3000);
```

## API

### `check(port)`

Checks if the specified port is available.

-   `port` (number): The port number to check.
-   Returns: A Promise that resolves to `true` if the port is available, `false` otherwise.

## License

MIT © [[BeyondJS](https://beyondjs)]
