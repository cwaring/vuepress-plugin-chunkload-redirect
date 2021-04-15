# vuepress-plugin-chunkload-redirect

␥ Catch chunkload errors from a stale deploy and route to destination.

Clientside apps remain in the browser memory and if a new build is deployed sometimes the JS chunks will change, resulting in errors routing to a desired destination. This plugin will detect when a page chunk is no longer available by catching the error and redirecting to the latest version of the application transparently.

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