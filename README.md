# OpenCow APT Repository

APT repository for OpenCow CLI packages.

## Ubuntu 24.04 / Debian amd64

~~~bash
echo 'deb [trusted=yes] https://opencow42.github.io/apt-repo stable main' | sudo tee /etc/apt/sources.list.d/opencow.list
sudo apt update
sudo apt install metabrain
~~~

The `trusted=yes` setup is temporary until the repository publishes a signing key and signed `InRelease` metadata.

## Packages

- `metabrain`: installs the `mb` CLI at `/usr/bin/mb`
