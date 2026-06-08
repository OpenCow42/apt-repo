# OpenCow APT Repository

APT repository for OpenCow CLI packages. Packages are currently published for
`amd64` and `arm64`.

## Ubuntu 24.04

~~~bash
echo 'deb [trusted=yes] https://opencow42.github.io/apt-repo ubuntu24.04 main' | sudo tee /etc/apt/sources.list.d/opencow.list
sudo apt update
sudo apt install metabrain
~~~

## Ubuntu 26.04

~~~bash
echo 'deb [trusted=yes] https://opencow42.github.io/apt-repo ubuntu26.04 main' | sudo tee /etc/apt/sources.list.d/opencow.list
sudo apt update
sudo apt install metabrain
~~~

## Compatibility Alias

`stable` is kept as a compatibility alias:

~~~bash
echo 'deb [trusted=yes] https://opencow42.github.io/apt-repo stable main' | sudo tee /etc/apt/sources.list.d/opencow.list
~~~

The `trusted=yes` setup is temporary until the repository publishes a signing key and signed `InRelease` metadata.

## Packages

- `metabrain`: installs the `mb` CLI at `/usr/bin/mb` and the `mbd` daemon at `/usr/bin/mbd`
- `potassium`: installs the `pot` CLI at `/usr/bin/pot`
