# Literate Polyglot
**Hello World in 12 languages**

The first thing you may want to do in a new programming language is write a "Hello, World!". For Entangled, the problem is then: in which language do write our first example? We don't want to play favourites, so here it is in 12 different languages.

## Bash
Little loved language for scripting odds and ends.

``` {.bash file="src/hello.sh"}
echo "Hello, Bash!"
```

``` {.bash .eval}
bash src/hello.sh
```

## C++
This turns out to be one of the more wordy solutions.

``` {.cpp file="src/hello.cc"}
#include <iostream>
#include <cstdlib>

int main() {
    std::cout << "Hello, C++!" << std::endl;
    return EXIT_SUCCESS;
}
```

``` {.bash .eval}
mkdir -p build
g++ src/hello.cc -o build/hello-cpp
./build/hello-cpp
```

## Go
Designed for simplicity and reasonable performance.

``` {.go file="src/hello.go"}
package main

import "fmt"

func main() {
    fmt.Println("Hello, Go!")
}
```

``` {.bash .eval}
go run src/hello.go
```

## Haskell
Lingua franca of the functional programming community.

``` {.haskell file="src/hello.hs"}
main :: IO ()
main = putStrLn "Hello, Haskell!"
```

``` {.bash .eval}
mkdir -p build
ghc src/hello.hs -o build/hello-haskell
./build/hello-haskell
```

## Javascript
Language of the web.

``` {.javascript file="src/hello.js"}
console.log("Hello, Node!")
```

``` {.bash .eval}
node src/hello.js
```

## Julia
High performance language for scientific computing.

``` {.python file="src/hello.jl"}
print("Hello, Julia!")
```

``` {.bash .eval}
julia -O0 src/hello.jl
```

## Lua
Light-weight embeddable scripting language.

``` {.lua file="src/hello.lua"}
print("Hello, Lua!")
```

``` {.bash .eval}
lua src/hello.lua
```

## OCaml
Functional language with focus on safety.

``` {.ocaml file="src/hello.ml"}
let () = Printf.printf "%s\n" "Hello, OCaml!"
```

``` {.bash .eval}
ocaml src/hello.ml
```

## Python
Well, Python is Python.

``` {.python file="src/hello.py"}
print("Hello, Python!")
```

``` {.bash .eval}
python src/hello.py
```

## R
Popular for data analysis.

``` {.r file="src/hello.r"}
write("Hello, R!", stdout())
```

``` {.bash .eval}
R --vanilla -s  < src/hello.r
```

## Rust
Memory safe system programming language.

``` {.rust file="src/hello.rs"}
fn main() {
    println!("Hello, Rust!")
}
```

``` {.bash .eval}
mkdir -p build
rustc src/hello.rs -o build/hello-rust
./build/hello-rust
```

## Scheme
My personal favourite.

``` {.scheme file="src/hello.scm"}
(import (rnrs (6)))

(display "Hello, Scheme!") (newline)
```

``` {.bash .eval}
guile src/hello.scm
```

