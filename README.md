# go_vendor_gen

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
        -h, --help                   Print this help and exit
