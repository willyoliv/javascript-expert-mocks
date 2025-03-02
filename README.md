# CSV to JSON Converter

This project is a simple Node.js application that reads a CSV file and converts it into a JSON format. It also includes unit tests using mocks to validate different scenarios.

## Project Structure

```
📦 javascript-expert-mocks
├── 📂 src
│   ├── constants.js  # Contains error messages and configuration
│   ├── file.js       # Handles file reading and conversion logic
├── 📂 mocks          # Mock data for tests
├── index.test.js     # Unit tests for the application
├── package.json      # Project dependencies and scripts
└── README.md         # Project documentation
```

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/willy-oliv/javascript-expert-mocks.git
   cd javascript-expert-mocks
   ```

2. Install dependencies:
   ```sh
   npm install
   ```

## Usage

To convert a CSV file to JSON, use the `csvToJSON` method in `file.js`. Example:

```js
const File = require('./src/file');

(async () => {
  try {
    const jsonData = await File.csvToJSON('./mocks/threeItems-valid.csv');
    console.log(jsonData);
  } catch (error) {
    console.error(error.message);
  }
})();

```

## Running Tests

To run tests, use the following command:
```sh
npm test
```
This will execute `index.test.js`, which includes test cases using mocks.

## Lessons Learned

- How to create and use mocks in unit testing.
- How to validate file content before processing.
- How to handle errors and limit input size.

## Next Steps

- Add more test cases for edge scenarios.
- Improve error handling.
- Implement support for different delimiters.

---
Created while learning about **mocks in unit testing**. 🚀