# angular-universal-localize-prerender

WIP: A PoC of an Angular app which

- has SSR
- is localized (en-US, de-CH, fr-CH),
- prerender-able

## running

```sh
npm install
npm run build:ssr
npm run prerender
```

then serve localized SSR app

```sh
npm run serve:ssr:en
npm run serve:ssr:de
npm run serve:ssr:fr
```
