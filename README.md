# web-ext-newtab-override

```sh
pnpm i
pnpm dev
pnpm build
```

## icons

```sh
curl https://raw.githubusercontent.com/feathericons/feather/master/icons/chrome.svg > src/assets/chrome.svg
for px in 16 32 48 128; do
  convert -density 1000 -resize "${px}x${px}" -background none src/assets/chrome.svg "src/assets/icon-${px}.png"
done
```

## references

- https://github.com/mozilla/web-ext
- https://developer.chrome.com/docs/extensions/mv3/manifest
- https://developer.chrome.com/docs/extensions/mv3/override/
- https://developer.chrome.com/docs/extensions/mv3/linux_hosting/
- https://github.com/jimschubert/NewTab-Redirect
