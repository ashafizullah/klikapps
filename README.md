# Klik Apps

Landing page for Adam's free, open-source apps: [KlikDB](https://github.com/ashafizullah/klikdb), [KlikSnap](https://github.com/ashafizullah/kliksnap), [KlikReel](https://github.com/ashafizullah/klikreel), [KlikDesign](https://github.com/ashafizullah/klikdesign), [KlikBand](https://github.com/ashafizullah/klikband) for Xiaomi Smart Band 9, and [KlikDash](https://github.com/ashafizullah/klikdash) for Android car headunits.

Live at **https://klikapps.pages.dev**.

A single static page in `public/`. Versions and download links are read from each repo's latest GitHub release in the browser, so a new app release needs no change here.

## Deploy

Every push to `main` deploys through GitHub Actions (`.github/workflows/deploy.yml`, secrets `CLOUDFLARE_API_TOKEN` and `CLOUDFLARE_ACCOUNT_ID`). To deploy by hand:

```sh
npx wrangler pages deploy public --project-name klikapps --branch main
```

## License

[MIT](LICENSE)
