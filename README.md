# eslint-formatter-multiple

A meta formatter for eslint that will output to multiple formats

## Install

`npm install --save-dev https://github.com/magarcia/eslint-formatter-multiple.git`

`yarn add --dev https://github.com/magarcia/eslint-formatter-multiple.git`

## Usage

Update your package.json to have a new section:

```
  "eslint-formatter-multiple": {
    "formatters": [
      {
        "name": "stylish",
        "output": "console"
      },
      {
        "name": "checkstyle",
        "output": "file",
        "path": "eslint-checkstyle.xml"
      }
    ]
  }
```

Finally, add the `--format multiple` when calling the `eslint` command.
