# [danklinux.org](https://danklinux.org) source code
This is the source code for the [danklinux.org](https://danklinux.org) website that will be updated.
Click here for the discord server that thought of the idea! [Discord](https://discord.gg/WNjQMx8bj9)

## Requirements

- [gomplate](https://docs.gomplate.ca/installing/) (`go install github.com/hairyhenderson/gomplate/v4/cmd/gomplate@latest`)

## Building

```sh
gomplate --input-dir=src/ --output-map='build/{{.in|strings.TrimSuffix ".tmpl" }}'
```

Now all of the outputed pages are in the `build` directory
