# babelify-jest

[Babel](https://github.com/babel/babel) [jest](https://github.com/facebook/jest) plugin which handles babelify modules
gently.

## Usage

Make the following changes to `package.json`:

```json
{
  "devDependencies": {
    "babel-jest": "*",
    "jest-cli": "*"
  },
  "scripts": {
    "test": "jest"
  },
  "jest": {
    "scriptPreprocessor": "<rootDir>/node_modules/babelify-jest",
    "testFileExtensions": ["es6", "js"],
    "moduleFileExtensions": ["js", "json", "es6"]
  }
}
```

And run:

    $ npm install

**And you're good to go!**
