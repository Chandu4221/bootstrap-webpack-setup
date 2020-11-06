# ❤️ 🥳 [Bootstrap](https://getbootstrap.com) Bootstrap Webpack Setup

# ✋ PLEASE GO THROUGH THE README COMPLETELY

## This Repo is the setup for the Bootstrap CSS Framework

Instructions

- `Clone` or `download` the repo
- run
  ```
  npm install
  ```
- to run the dev server

  ```
  npm run start
  ```

  dev server runs on the [http://localhost:9000](http://localhost:9000)

- to create build
  ```
  npm run build
  ```
  List of dev dependencies used

| package                 | version  |
| ----------------------- | -------- |
| @babel/core             | ^7.11.6  |
| @babel/preset-env       | ^7.11.5  |
| babel-loader            | ^8.1.0   |
| css-loader              | ^4.3.0   |
| fibers                  | ^5.0.0   |
| file-loader             | ^6.1.0   |
| html-loader             | ^1.3.0   |
| html-webpack-plugin     | ^4.4.1   |
| mini-css-extract-plugin | ^0.11.2  |
| purgecss-webpack-plugin | ^3.0.0   |
| sass                    | ^1.26.10 |
| sass-loader             | ^10.0.2  |
| webpack                 | ^4.44.1  |
| webpack-cli             | ^3.3.12  |
| webpack-dev-server      | ^3.11.0  |

---

List of dependencies used

| package   | version |
| --------- | ------- |
| bootstrap | ^4.5.3  |

---

you can add new pages(multiple html files) by importing them into the `src/js/index.js`

### 💡 don't forget to add the entry in the webpack.config.js under plugins setion

```
  plugins: [
    new HtmlWebpackPlugin({
      template: "src/index.html",
    }),
    new HtmlWebpackPlugin({
      filename: "page.html",
      template: "src/page.html",
    }),
    ... create new pages and add entry here and import them into the src/js/index.js
  ],
```

⚠️ don't forget to add the `filename` otherwise it is taken as the default entry creating a `index.html`(also overrides the actual index.html) instead of the actual filename(page.html)

## Made with 💖 - by Chandra Shekhar
