# Get Go

For easy download, installation and switching between different versions of Golang (linux-amd64).

## Usage

    $ ./get-go GOVERSION

The first run per version takes time as the tarball is downloaded but the active version of Golang can be quickly switched with subsequent calls.

You can verify that it worked by issuing

    $ go version

## Example

    $ ./get-go 1.5.3

## Permissions

You must have write access to the current directory as this script will create a `.cache` directory and stash the tarballs it downloads there.

You'll also need write access to `/usr/local/` as the tarballs will be unpacked there and a symlink created at `/usr/local/go`.

## Environment variables

You should ensure that `/usr/local/go/bin` is on your path and set `GOPATH` and `GOBIN` as usual but *you do not need to set `GOROOT`*.
