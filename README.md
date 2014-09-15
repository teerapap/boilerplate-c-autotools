woof (sample name)
===================

<Brief description>

## Features

  * Feature 1

## Features in the future

  * Future feature 1

## Documentation

See in `doc/` directory. Markdown is used as default format for documentation.

## Requirements

woof is designed to have fairly minimal requirements to build for unix 
users.  Currently, we support woof on Linux and Mac OS X.

### Build environment requirements

These are the base requirements to build woof from source:

  * GNU-compatible Make or "gmake"
  * POSIX-standard shell
  * A C99 standards compliant compiler

Furthermore, if you are building woof from a git clone, there are 
further requirements:

  * Autotools with autoreconf command version 2.59 or newer

Or if you are building woof for Mac OS X, there are further
requirements:

  * Mac OS X 10.7 Lion or newer

## Building

If you are building woof from a source package.(woof-x.x.tar.gz), you 
can skip autotools step.

You will need to prepare the GNU Autotools build system, if you
are using Linux, Mac OS X, or FreeBSD. Enter the target directory
and proceed with the following command:

    autoreconf -i

Once you have completed this step, you are ready to build the library. Note
that you should only need to complete this step once. The subsequent `make`
invocations will automatically re-generate the bits of the build system that
need to be changed.

    mkdir build
    cd build
    ../configure  # Standard GNU configure script, --help for more info
    make          # Standard makefile following GNU conventions
    make check    # Builds and runs all tests - all should pass

The following command will install all of the libraries, public headers, and 
utilities necessary for other programs and libraries to leverage it:

    sudo make install  # Not necessary, but allows use by other programs


## Testing

When you run `make check`, it build test executables in `build/test`, e.g.
`unit_test`, and run them.  You can manually execute these tests on 
command-line as well. 

## Contributing

These are recommendded development tools if you want to contribute to the project in addition to
build environment requirements (as described above):

  * Git 1.7.0 or newer
  * Vim 7 or newer

woof development is usually done in vim so we provide vimrc file in `contrib/vimrc`
to start contribution. Please copy it or source it in your .vimrc so it sets the 
correct indent size and stuff for the contribution.

Source it with `:source contrib/.vimrc`

## Dependencies 

  * xxxx-y.zzz

  Dependency libraries are in `deps` directory along with their respective 
  licenses in `deps/LICENSES` and tracking version in `deps/VERSIONS`

