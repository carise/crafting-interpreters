# Crafting interpeters

## Installing openjdk

I never remember how to do this off the top of my head because I do it so infrequently.

Install jenv and add the init functions in .zshrc

Download Adoptium and install

```sh
curl -L https://github.com/adoptium/blah/openjdk_21.tar.gz -o openjdk21.tar.gz
tar xzf openjdk21.tar.gz
sudo mv openjdk21 /opt/jdk21
```

Link up jenv

```sh
jenv add /opt/jdk21
# should show some message about what version got added
```

Then test it out

```sh
javac --version
```

Pin the version using a `.java-version` file

I also was able to install openjdk from `brew` and add it to `jenv`.

## Running java programs

Code is stored in `src/com/craftinginterpeters/lox` (will probably restructure), and
has a package `com.craftinginterpeters.lox`.

To build and run:

```sh
cd src/com/craftinginterpreters/lox
javac Lox.java
cd <root>/src
java com.craftinginterpreters.lox.Lox
```
