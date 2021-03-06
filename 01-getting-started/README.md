# Getting started - Hello Clang LibTooling!

## Prerequisite - Downloading LLVM Clang

- http://releases.llvm.org/download.html

#### Mac OS X

```shell
cd path/to/your/dir
wget http://releases.llvm.org/3.9.0/clang+llvm-3.9.0-x86_64-apple-darwin.tar.xz
tar xaf clang+llvm-3.9.0-x86_64-apple-darwin
```

## Compiling the application

```shell
git clone https://github.com/mogemimi/negicco.git
cd negicco/01-getting-started

# Compiling for any platforms
make build CLANG_DIR=/path/to/your/dir/clang+llvm-3.9.0

# Compiling under Mac OS X
make build CLANG_DIR=/path/to/your/dir/clang+llvm-3.9.0-x86_64-apple-darwin
```

## Running the application

```shell
.negicco -help
```

Result:

```
USAGE: negicco [options] <source0> [... <sourceN>]

OPTIONS:

Generic Options:

  -help                      - Display available options (-help-hidden for more)
  -help-list                 - Display list of available options (-help-list-hidden for more)
  -version                   - Display the version of this program

my-tool options:

  -extra-arg=<string>        - Additional argument to append to the compiler command line
  -extra-arg-before=<string> - Additional argument to prepend to the compiler command line
  -p=<string>                - Build path
```
