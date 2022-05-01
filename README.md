# web-ext-newtab-override

```sh
web-ext --version # 6.8.0

npm i

npm run dev
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
- https://github.com/jimschubert/NewTab-Redirect
