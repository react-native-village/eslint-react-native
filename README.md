# eslint + prettierrc

### step 1
```
 yarn add eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react eslint-watch babel-core babel-eslint babel-preset-airbnb babel-preset-react-native pre-commit prettier prettier-eslint eslint-plugin-prettier eslint-config-prettier -D
```

### step 2
create .eslintrc.json
```
touch .eslintrc.json
```

### step 3
to add rules in .eslintrc.json

```json
{
  "parser": "babel-eslint",
  "extends": "airbnb",
  "plugins": ["react", "jsx-a11y", "import"],
  "rules": {
    "react/jsx-filename-extension": ["off"],
    "react/jsx-one-expression-per-line": 0,
    "linebreak-style": ["off"],
    "no-undef": ["error"],
    "react/sort-comp": ["off"],
    "react/prefer-stateless-function": ["off"],
    "react/destructuring-assignment": 1,
    "semi": ["error", "never"],
    "spaced-comment": 0,
    "comma-dangle": ["error", "never"],
    "react/prop-types": 0,
    "no-extra-boolean-cast": 0,
    "quote-props": 0,
    "object-curly-spacing": ["error", "always"],
    "camelcase": 0,
    "no-nested-ternary": 0,
    "object-curly-newline": 0,
    "operator-linebreak": 0,
    "no-unused-expressions": 0,
    "global-require": 0,
    "max-len": 0,
    "import/no-cycle": 0,
    "no-underscore-dangle": 0,
    "no-return-assign": 0,
    "import/prefer-default-export": 0,
    "no-console": "error"
  },
  "globals": {
    "it": 0,
    "expect": 0,
    "describe": 0,
    "navigator": 0
  }
}
```

### step 4
Open up your package.json and make the following updates.
 ``` 
"scripts": {
    "start-ios": "react-native run-ios --simulator='iPhone SE' && npm run lint-watch",
    "start-android": "react-native run-android && npm run lint-watch",
    "lint": "esw src/**",
    "lint-watch": "esw -w --changed src/**"
  },
"precommit": [
    "lint"
],
"prettier": {
    "singleQuote": true,
    "printWidth": 120,
    "tabWidth": 2,
    "trailingComma": "none",
    "bracketSpacing": true,
    "semi": false,
    "useTabs": false,
    "jsxBracketSameLine": false
}
```


### step 5
Create `touch .prettierrc` 
``` 
{
  "singleQuote": true,
  "printWidth": 120,
  "tabWidth": 2,
  "trailingComma": "none",
  "bracketSpacing": true,
  "semi": false,
  "useTabs": false,
  "jsxBracketSameLine": false
}
```

### step 6
create folder `src` and to transfer flie `src/App.js`

### step 7
restart project 
`yarn start-ios`
or
`yarn start-android`

### done
