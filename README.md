# eslint-react-native

### step 1
```
 yarn add -D eslint-config-airbnb eslint-plugin-babel eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react babel-preset-react-native eslint
```

### step 2
create .eslintrc.json
```
touch .eslintrc.json
```

### step 3
to add rules in .eslintrc

```json
{
  "env": { "node": true, "browser": true, "es6": true },
  "parser": "babel-eslint",
  "extends": [
    "airbnb",
    "eslint:recommended",
    "plugin:react/recommended"
  ],
  "rules": {
    "react/jsx-filename-extension": [1, { "extensions": [".js", ".jsx"] }],
    "react/jsx-wrap-multilines": 0,
    "react/jsx-curly-brace-presence": [0, { "props": "always", "children": "always" }],
    "jsx-quotes": ["error", "prefer-double"],
    "quote-props": 0,
    "object-curly-spacing": ["error", "always"],
    "camelcase": 0,
    "no-nested-ternary": 0,
    "object-curly-newline": 0,
    "no-use-before-define": 0,
    "operator-linebreak": 0,
    "global-require": 0,
    "max-len": 0,
    "import/no-cycle": 0,
    "no-underscore-dangle": 0,
    "no-return-assign": 0,
    "import/prefer-default-export": 0,
    "no-console": "error",
    "react/jsx-no-bind": [1, { "ignoreRefs": 1, "allowArrowFunctions": true }],
    "react/jsx-one-expression-per-line": 0,
    "react/destructuring-assignment": [0, "never"],
    "semi": ["error", "never"],
    "spaced-comment": 0,
    "comma-dangle": ["error", "never"],
    "react/prop-types": 0,
    "no-extra-boolean-cast": 0
  },
  "globals": {
    "__DEV__": true
  }
}
```

### done
