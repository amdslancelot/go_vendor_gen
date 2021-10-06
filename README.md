# go_vendor_gen

## Install and Run

1. Checkout this git repo
2. Go to the project main folder (that need to generate vendor data with)
3. (optional) Download the latest golang binaries if needed
4. Run the command. ex:
(easy)
```sh
   (path_to)/go_vendor_gen -d -b -c ~/golang-1.17.1/go/bin/go -n ol7/rclone-1.56.2-1.0.1-lanstest --dry-run
```

(more complicated)
```sh
   (path_to)/go_vendor_gen -d -b -c ~/golang-1.17.1/go/bin/go -n ol7/rclone-1.56.2-1.0.1-lanstest -nc --dry-run
```

## Help

Golang project vendor data generator tool

Intro:
        go_vendor_gen is a Go Vendor Data Generator Tool.

Usage: 

        go_vendor_gen <tag> [arguments]


Available options:

        -c, --go-exec-path           Specify go command location
        -n, --tagname                Customize git tag name to commit
        -b, --dev                    Commit to git and trigger autobuild
        -nc, --no-version-check      Skip version match check
        -m, --gomod-path GOMOD_PATH  Specify go.mod file location
        -d, --debug                  Enable debug log
        -h, --help                   Print this help and exit
