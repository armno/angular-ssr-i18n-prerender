# angular-universal-localize-prerender

WIP: A PoC of the Angular Tour of Heros app with:

- SSR
- Localization using `@angular/localize` (locales: en-GB, de-CH, fr-CH, it-CH)
- Prerendering

## running

```sh
npm install
npm start
# or
npm run dev:ssr
```

extract translations from the source language (en-GB)

```sh
npm run extract
```

This creates `src/locale/messages.xlf`. Translations in other languages have to be managed externally.

Once we finish translations of other locales, build in SSR mode for all locales

```sh
npm run build:ssr
```

To prerender `/dashboard/index.html` and `/heroes/index.html` for all locales

```sh
npm run prerender
```

Then we can serve localized SSR app

```sh
npm run serve:ssr:en
npm run serve:ssr:de
npm run serve:ssr:fr
npm run serve:ssr:it
```
