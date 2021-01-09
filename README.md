# Next.js Progressbar Without Spinner

A simple Next.js progressbar based on [Next.js Progressbar](https://www.npmjs.com/package/nextjs-progressbar).

## How to install?

```bash
npm i @taishikato/nextjs-progressbar
```

## How to use?

After installing the package, import this in your `pages/_app.js` file.

```bash
import NextNprogress from '@taishikato/nextjs-progressbar';
```

And for rendering add `<NextNProgress />` inside `Container` component.

### Default Config

```
<NextNprogress
  color="#29D"
  startPosition={0.3}
  stopDelayMs={200}
  height="3"
/>
```

- `color`: to change the default color of progressbar. You can also use `rgb(,,)` or `rgba(,,,)`.
- `startPosition`: to set the default starting position : `0.3 = 30%`.
- `stopDelayMs`: time for delay to stop progressbar in `ms`.
- `height`: height of progressbar in `px`.

### Advanced Config

You can use [other configurations](https://github.com/rstacruz/nprogress#configuration) which NProgress provides by adding a JSON in `options` props.

```
<NextNprogress
  options={{ easing: 'ease', speed: 500 }}
/>
```
