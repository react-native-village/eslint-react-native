# eslint-react-native

### step 1
```
 yarn add -D babel-eslint eslint eslint-plugin-react
```

### step 2
create .eslintrc
```
touch .eslintrc
```

### step 3
to add rules in .eslintrc

```
{
  "parser": "babel-eslint",
    "env": {
      "browser": true
    },
    "plugins": [
      "react"
    ],
    "extends": [
      "eslint:recommended",
      "plugin:react/recommended"
    ],
    "rules": {
			"strict": 0,
			"arrow-body-style": 0, 
			"no-unused-expressions": ["error", { "allowTernary": true }],
			"no-console": 0,
			"react/jsx-uses-react": "error",
			"react/jsx-uses-vars": "error",
			"indent": ["error", 2],
			"linebreak-style": [ "error", "unix" ],
			"quotes": [ "error", "single" ],
			"semi": [ "error", "never" ],
			"spaced-comment": 0,
			"max-len": 0,
			"camelcase": 0,
			"comma-dangle": ["error", "never"],
			"object-curly-spacing": 0,
			"no-nested-ternary": 0
    }
}
```

### done
