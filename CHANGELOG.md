# astro-netlify-cms

## 0.6.0

### Minor Changes

- Switch from netlify-cms to decap-cms

## 0.5.4

### Patch Changes

- [#76](https://github.com/delucis/astro-netlify-cms/pull/76) [`2e24122`](https://github.com/delucis/astro-netlify-cms/commit/2e241229a38d7aa783ea9df462e66b8c15ffa963) Thanks [@Marocco2](https://github.com/Marocco2)! - Support for Astro v3

## 0.5.3

### Patch Changes

- [#63](https://github.com/delucis/astro-netlify-cms/pull/63) [`e3884e3`](https://github.com/delucis/astro-netlify-cms/commit/e3884e303ba49fd70fb90fc412715de6dec6cfbd) Thanks [@dependabot](https://github.com/apps/dependabot)! - Bump simple-git from 3.15.1 to 3.16.0

## 0.5.2

### Patch Changes

- [`8f23e86`](https://github.com/delucis/astro-netlify-cms/commit/8f23e8667b591838aff456649d7bc059072dd9b0) Thanks [@delucis](https://github.com/delucis)! - Update peer dependencies to support Astro v2

## 0.5.1

### Patch Changes

- [#56](https://github.com/delucis/astro-netlify-cms/pull/56) [`b5cb7aa`](https://github.com/delucis/astro-netlify-cms/commit/b5cb7aac1d243af7a4e9814be1f47158e28a897c) Thanks [@dependabot](https://github.com/apps/dependabot)! - Bump json5 and react-hot-loader

## 0.5.0

### Minor Changes

- [#53](https://github.com/delucis/astro-netlify-cms/pull/53) [`40d0385`](https://github.com/delucis/astro-netlify-cms/commit/40d03858fa4a049684e1b9cc895c7280e7479cb5) Thanks [@delucis](https://github.com/delucis)! - Don’t automatically inject `@astrojs/react` integration

  ⚠️ BREAKING CHANGE ⚠️

  Previously, this integration included [`@astrojs/react`](https://docs.astro.build/en/guides/integrations-guide/react/) and injected it to Astro’s integrations config for you. This is no longer the case.

  If you are using React components and were relying on this, make sure to add the integration when upgrading. The simplest way to do this is to run:

  ```bash
  npx astro add react
  ```

## 0.4.0

### Minor Changes

- [#48](https://github.com/delucis/astro-netlify-cms/pull/48) [`a1a0002`](https://github.com/delucis/astro-netlify-cms/commit/a1a0002c63c542a4dd82ae093effaf18bb824a84) Thanks [@delucis](https://github.com/delucis)! - Add support for importing npm packages via `previewStyles` config

  ⚠️ **BREAKING CHANGE** ⚠️

  This release changes how you import a local CSS file in `previewStyles`.
  These must now be prefixed with a leading `/`:

  ```diff
  {
    previewStyles: [
  -   'src/styles/base.css',
  +   '/src/styles/base.css',
    ],
  }
  ```

  This allows us to support importing CSS you may have installed from an npm module, for example importing font CSS from Fontsource:

  ```js
  previewStyles: ["@fontsource/roboto"];
  ```

## 0.3.5

### Patch Changes

- [#46](https://github.com/delucis/astro-netlify-cms/pull/46) [`cdbf7d6`](https://github.com/delucis/astro-netlify-cms/commit/cdbf7d63df2bbb1b65c661e87f93369f3977725a) Thanks [@delucis](https://github.com/delucis)! - Include identity widget on admin route even when `disableIdentityWidgetInjection` is set to `true`

## 0.3.4

### Patch Changes

- [#41](https://github.com/delucis/astro-netlify-cms/pull/41) [`7e53467`](https://github.com/delucis/astro-netlify-cms/commit/7e53467096dad33bd2c15f060f3c4c4ad03a7a1e) Thanks [@dependabot](https://github.com/apps/dependabot)! - Bump loader-utils from 1.4.0 to 1.4.2

## 0.3.3

### Patch Changes

- [#38](https://github.com/delucis/astro-netlify-cms/pull/38) [`9b2802c`](https://github.com/delucis/astro-netlify-cms/commit/9b2802cb1727d9e1e2f695ad1631c71af9bb9a52) Thanks [@delucis](https://github.com/delucis)! - Restart Netlify CMS proxy server when astro.config reloads

## 0.3.2

### Patch Changes

- [#33](https://github.com/delucis/astro-netlify-cms/pull/33) [`d62b891`](https://github.com/delucis/astro-netlify-cms/commit/d62b8917f78ba7520c32ba0ba6bd32d818183c28) Thanks [@Marocco2](https://github.com/Marocco2)! - Add `disableIdentityWidgetInjection` option

- [#36](https://github.com/delucis/astro-netlify-cms/pull/36) [`c508be4`](https://github.com/delucis/astro-netlify-cms/commit/c508be466b0c46dcd9bc6897045e0b90f173b9ab) Thanks [@delucis](https://github.com/delucis)! - Fix an issue in some browsers with the rich text editor.

  Adds the workaround documented in [netlify/netlify-cms#5092](https://github.com/netlify/netlify-cms/issues/5092) to the admin dashboard.

## 0.3.2-next.0

### Patch Changes

- [#33](https://github.com/delucis/astro-netlify-cms/pull/33) [`d62b891`](https://github.com/delucis/astro-netlify-cms/commit/d62b8917f78ba7520c32ba0ba6bd32d818183c28) Thanks [@Marocco2](https://github.com/Marocco2)! - Add `disableIdentityWidgetInjection` option

## 0.3.1

### Patch Changes

- [`bd64e05`](https://github.com/delucis/astro-netlify-cms/commit/bd64e057e5df57f8e1b494336a98617fb239f5ac) Thanks [@delucis](https://github.com/delucis)! - Upgrade React dependencies

## 0.3.0

### Minor Changes

- [#30](https://github.com/delucis/astro-netlify-cms/pull/30) [`6757440`](https://github.com/delucis/astro-netlify-cms/commit/6757440b968332f0b1dc6a52ee70a6c1852f7b15) Thanks [@delucis](https://github.com/delucis)! - Refactor to use Astro’s built-in `injectRoute` helper to add the admin dashboard.

  Significantly simplifies the Vite plugin logic and should make future improvements easier to implement.

## 0.2.5

### Patch Changes

- [`013a42d`](https://github.com/delucis/astro-netlify-cms/commit/013a42d0e7d656b760283af19422c9602d83a9e3) Thanks [@delucis](https://github.com/delucis)! - Fix preview styles in production builds

## 0.2.4

### Patch Changes

- [#25](https://github.com/delucis/astro-netlify-cms/pull/25) [`eba6556`](https://github.com/delucis/astro-netlify-cms/commit/eba65563e2815242877498bf43f8a1d8b3e4f41a) Thanks [@Opposedmatty](https://github.com/Opposedmatty)! - Fix typo in description meta tag

## 0.2.3

### Patch Changes

- [#23](https://github.com/delucis/astro-netlify-cms/pull/23) [`26243d5`](https://github.com/delucis/astro-netlify-cms/commit/26243d54ebee46122053d315ad929c4636a123e2) Thanks [@codelastnight](https://github.com/codelastnight)! - remove node join() from vite-plugin-admin-dashboard to allow windows to run dev

## 0.2.2

### Patch Changes

- [`a7c4e43`](https://github.com/delucis/astro-netlify-cms/commit/a7c4e43511af695b91c0b2b19a750d769d692f98) Thanks [@delucis](https://github.com/delucis)! - Hot fix: remove comment clashing with over-eager whitespace collapsing by astro-compress

## 0.2.1

### Patch Changes

- [`cb7adcc`](https://github.com/delucis/astro-netlify-cms/commit/cb7adcc8c0a61756817449cf240efacf82cd79c1) Thanks [@delucis](https://github.com/delucis)! - Fix for compression support: end import statements with semi-colons

## 0.2.0

### Minor Changes

- [`0726494`](https://github.com/delucis/astro-netlify-cms/commit/0726494a5908a50ac859a92c7bf78f18f2399437) — Update to Astro v1 🚀

### Patch Changes

- [`f5b06ed`](https://github.com/delucis/astro-netlify-cms/commit/f5b06ed24ec3f90ed17a6dd33def80e531e9ffd3) — Run `netlify-cms-proxy-server` in shell on Windows (fixes [#13](https://github.com/delucis/astro-netlify-cms/issues/13))

## 0.1.0

Initial release
