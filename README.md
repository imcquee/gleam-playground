# gleam chat

Learning Gleam. Svelte frontend using types and functions from Gleam.

Sources:
- [connellr023/chatter-reborn](https://github.com/connellr023/chatter-reborn)
- [hayleigh-dot-dev/fosdem-2023](https://github.com/hayleigh-dot-dev/fosdem-2023)
- [bcpeinhardt/learn_otp_with_gleam](https://github.com/bcpeinhardt/learn_otp_with_gleam)

## Development

### Setup
Use [asdf](https://asdf-vm.com/guide/getting-started.html) to `asdf install` gleam and other dependencies defined in [.tool-versions](./.tool-versions).

### Easy
```sh
gleam run
```
Open [localhost:3000/test.html](http://localhost:3000/test.html) in your browser.

### Svelte Frontend
```sh
# run backend
gleam run

# build shared types
cd src/shared
gleam build --target javascript
rm -rf ../../frontend/src/generated
cp -r build/dev/javascript ../../frontend/src/generated

# run frontend
cd frontend
bun dev
```

Open: [localhost:3000](http://localhost:3000) in your browser.

## Screenshot

![Screenshot](./docs/screenshot.png)