# truffle-export-abi

Simple tool to extract ABI from truffle build/ directory to a single file. This is a trivial tool but it can be handy when you're debugging your contract.

# Install

```shell
$ npm install -g truffle-export-abi
```

# Usage

Run it from your truffle project directory:
```shell
$ truffle-export-abi
notice: ABI extracted and output file wrote to: build/ABI.json
```

Run it from anywhere:
```shell
$ truffle-export-abi -d /home/user/myproject/build/contracts/ -o /home/user/myproject/build/abi.json -v
notice: ABI extracted and output file wrote to: /home/user/myproject/build/abi.json
```

Options:
 - `-d / --directory`: location of the build files, [build/contracts] by default
 - `-o / --output`: output file, [build/ABI.json] by default
 - `-v / --verbose`

# Build, run, example

```shell
# Setup the project
$ npm install
```

I included a stripped example of a ERC721 token files, you can ru

```shell
$ node index.js -v -d example/ -o abi.json
```
