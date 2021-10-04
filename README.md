# go_vendor_gen

## Usage

1. Go to the project main folder
2. Run the command. ex:
```sh
   (path_to)/go_vendor_gen -m go.mod -c ~/golang-1.17.1/go/bin/go -d -b -n ol7/rclone-1.56.2-1.0.1-lanstest -nc --dry-run
```

## Help

Golang project vendor data generator tool

Intro:
        go_vendor_gen is a Go Vendor Data Generator Tool.

Usage: 

	go_vendor_gen <tag> ([arguments]


Available options:

        -m, --gomod-path GOMOD_PATH  Specify go.mod file location
        -c, --go-exec-path           Specify go command location
        -d, --debug                  Enable debug log
        -n, --tagname                Customize git tag name to commit
        -b, --dev                    Commit to git and trigger autobuild
        -nc, --no-version-check      Skip version match check
        -h, --help                   Print this help and exit

