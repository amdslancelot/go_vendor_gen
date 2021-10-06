# go_vendor_gen

This is a tool I built to specifically fix the golang vendor data common issues. It's been a while we have build issues for rclone, packer and other golang based projects. I'm collecting answers to the issues we were facing and trying to solve them at once by creating this tool.

Sometimes we don't have the latest golang version so I added this feature to assign the golang executable location. Also you can customize the test git tag name.

## Install and Run

1. Checkout this git repo
2. Go to the project main folder (that need to generate vendor data with)
3. (optional) Download the latest golang binaries if needed
4. Run the command. ex:

(easy)
```sh
   (path_to)/go_vendor_gen -d -b --dry-run
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
