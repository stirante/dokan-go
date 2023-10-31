# [Dokan](https://github.com/dokan-dev/dokany) bindings for Go

Dokan is a library for implementing user mode filesystems on Windows. 
This library provides a thin binding to the library for Go programs.

## Fork

This fork is just a copy of changes from [keybase/client](https://github.com/keybase/client).

It's compatible with [Dokany 1.2](https://github.com/dokan-dev/dokany/releases/tag/v1.2.2.1000)

# Documentation

https://godoc.org/github.com/stirante/dokan-go

# Licensing

The go binding itself is BSD3 licensed as featured in the LICENSE.

Additionally we ship Dokan C headers in the dokan_header directory. These
are subject to LGPL and are from the Dokan project. These are used to
compile the code without a Dokan installation in the path.

To use the library you will need to have installed a version of the LGPL
licensed Dokany DLL licensed from https://github.com/dokan-dev/dokany

The Go library uses LoadLibrary to load the Dokan DLL, it is not linked
with the DLL. Using different builds of the DLL works fine.


