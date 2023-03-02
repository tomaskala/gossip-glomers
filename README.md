# Gossip Glomers

A series of distributed systems challenges found at <https://fly.io/dist-sys/>.

## Prerequisites

* Download [maelstrom 
  0.2.2](https://github.com/jepsen-io/maelstrom/releases/tag/v0.2.2) and 
  extract it to the root of this repository.
* Install `maelstrom` prerequisites.
  ```
  # pacman -S jre-openjdk graphviz gnuplot
  ```

## Initializing a new module

* Create the module.
  ```
  $ mkdir my-module
  $ cd my-module
  $ go mod init my-module
  $ go mod tidy
  ```
* Write your code.
* Install `maelstrom-go` and the module.
  ```
  $ go get github.com/jepsen-io/maelstrom/demo/go
  $ go install .
  $ ./run ../maelstrom
  ```

## Debugging

* Run the `maelstrom` web server to view results.
  ```
  $ ./maelstrom serve
  ```
