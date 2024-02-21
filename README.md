<div align="center">

# asdf-docker [![Build](https://github.com/doriancodes/asdf-docker/actions/workflows/build.yml/badge.svg)](https://github.com/doriancodes/asdf-docker/actions/workflows/build.yml) [![Lint](https://github.com/doriancodes/asdf-docker/actions/workflows/lint.yml/badge.svg)](https://github.com/doriancodes/asdf-docker/actions/workflows/lint.yml)

[docker](https://github.com/doriancodes/docker) plugin for the [asdf version manager](https://asdf-vm.com).

</div>

# Contents

- [Dependencies](#dependencies)
- [Install](#install)
- [Contributing](#contributing)
- [License](#license)
- [Notes](#notes)

# Dependencies

- `bash`, `curl`, `tar`, and [POSIX utilities](https://pubs.opengroup.org/onlinepubs/9699919799/idx/utilities.html).
- `ASDF_DOWNLOAD_PATH`: the path at which you wish to download the file.
- `ASDF_INSTALL_VERSION`: the version to install.
- `ASDF_INSTALL_PATH`: the path at which you wish to install the tool.
- `ASDF_INSTALL_TYPE`: the type of install. It's ignored if it's equal to the `ASDF_INSTALL_VERSION`.

# Install

Plugin:

```shell
asdf plugin add docker
# or
asdf plugin add docker https://github.com/doriancodes/asdf-docker.git
```

docker:

```shell
# Show all installable versions
asdf list-all docker

# Install specific version
asdf install docker latest

# Set a version globally (on your ~/.tool-versions file)
asdf global docker latest

# Now docker commands are available
docker --help
```

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to
install & manage versions.

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/doriancodes/asdf-docker/graphs/contributors)!

# License

See [LICENSE](LICENSE) © [Dorian C.](https://github.com/doriancodes/)

# Notes
Please note that the [github docker repository](https://github.com/docker/docker-ce) is deprecated and has been archived. It is uncertain if the project will remain open source. You might want to look into [moby](https://www.docker.com/blog/introducing-the-moby-project/).