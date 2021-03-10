# `react-app-rewire-fast-refresh`

this project is reedited from [`react-app-rewire-hot-loader`](https://github.com/cdharris/react-app-rewire-hot-loader)

Add the [`react-refresh-webpack-plugin`](https://github.com/pmmmwh/react-refresh-webpack-plugin) to your `create-react-app` app via [`react-app-rewired`](https://github.com/timarney/react-app-rewired).

Because who wants their app, state, and styles automatically reloading all the time?

## Installation

```
npm install --save react-app-rewire-fast-refresh

```

## Usage

In the `config-overrides.js` of the root of your project you created for `react-app-rewired` add this code:

```JS
const rewireReactFastRefresh = require('react-app-rewire-fast-refresh')

/* config-overrides.js */
module.exports = function override (config, env) {
  config = rewireReactFastRefresh(config, env)
  return config
}
```

That's it, you now have hot reloads!


## License

Licensed under the MIT License, Copyright ©️ 2021 Kent Wood. See [LICENSE.md](LICENSE.md) for more information.
