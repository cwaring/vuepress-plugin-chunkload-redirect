# vuepress-plugin-chunkload-redirect
🐶 Helper to catch chunkload errors from a stale deploy and route destination

Clientside apps remain in the browser memory and if a new build is deployed sometimes the JS chunks could change resulting in errors routing to a destination. This plugin will detect when a page chunk is no longer avaliable by catching the error and redirect the user to destination url by reloading the latest version of the application.

Compatible with Vuepress 1.x

## Usage

```
npm i -D vuepress-plugin-chunkload-redirect
```

### Setup

Add to `config.js` or `theme/index.js`

```
module.exports = {
  plugins: [
    ['vuepress-plugin-chunkload-redirect'],
  ]
}
```