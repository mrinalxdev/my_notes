## Fundamentals knowledge 
There are points to be noted before learning go 
- ##### Statically typed language 
	This means we have to declare the type of the variable explicitly or they have to be inferred and there types cannot be changed until you have done the type-conversion !!
	```go
	var newVar string = "newVariable"
	var newStrVar = "newStrVar" // Automatically detects 
```

- ##### Strongly typed language
	In golang one cannot concatenate string and integer at once, either you typeChange one of the variable.
	Strongly typed languages do help you with errors handling before the execution takes place. 
	```go
	var a = 1
	var b = "something"
	var c = a + b // error
```

- ##### Go is compiled and is fastest among other backend languages
	Which means it compiles the whole programme into binary files which exist as `0` and `1` , Compiling programme are much more faster than interpreter languages coz interpreter languages interprets the code one by one whereas compiling languages compiles the the whole programme at once

- ##### Built in concurrency 
	Golang has inbuilt concurrency also known as `goroutines` which we will be talking later in this docs. 
	In general *concurrency* in programming languages refers to the ability of a program to execute multiple tasks or thread simultaneously which contributes to many outcomes of a programme.

- ##### Simplicity of golang
	Doing lots of things in less line of codes. Here is an example 
	```go
	// Walrus operator is used in golang to declare variables and constants in more efficient way
	a := 23
	fmt.Println(a) // printing a 
```
	golang has also `garbage collection` which freezes unused memory, which in other like `c++` we have to manage by ourself !!

This is all about the overview of Golang and why to use golang as your next backend language 

### A little more to know before we start 

Before we initialise our project we need to know what are packages and modules in golang
#### Modules and packages 
`Packages` are the folders that contains the go files and collection of packages makes up a `Module`.

How to make a module and initialise a project ??
```terminal
mkdir first_programme
cd first_programme

go mod init github.com/mrinalxdev/first_programme
```

Usually while building up big projects in golang we use the real Github repository to define a module

The file now contains a `go.mod` which will consists all the third party libraries we have installed for our project !! It also consist of the go version you are using !!

```go

package main // or the name of the folder in which the file exists

import (
	"fmt" // library to print stuffs and variables
)

func main(){
	fmt.Println("Hello World")
}
```

```Terminal
go run main.go

>>> Hello World
```

This is how we write files in golang !!

`Package main` in and folder mean that will be the main entry point to any `Module or Package` 