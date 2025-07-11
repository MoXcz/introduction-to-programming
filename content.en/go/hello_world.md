---
weight: 1
title: "2.1 Hello, World!"
---

# Hello, world!

> *Going forwards the steps will be given for the CLI; if you are using other OS (Windows, MacOS, etc.) you're probably using a GUI so just create the files just as the instructions go*

With Go installed follow these instructions:

```sh
cd                # go to current user's $HOME
mkdir learning-go # create directory / folder
cd learning-go    # go into the directory / folder
touch main.go     # create main.go file
```

> *Both directory and folder refer to the same idea, as of preference I will use `directory` going forwards*

Now open the file and copy the following code:

```go
package main

import "fmt"

func main() {
	fmt.Println("Hello, World!")
}
```

And now run the code:

```sh
go run main.go
```

And... that's it. You should see a result similar to this:

![](/img/hello_world.png)

You can try and change the text and print whatever you want before continuing. This is as simple as a program gets, I will go over some of the *special* things of Go in the following chapters, but this is a rundown of the program above:

1. Define the `package` name as `main`, which is just short for saying that this is our *entry point*.
2. Import the `fmt` package (it has some *functions*, more on that later).
3. Define a function with the `func` keyword called `main()`
4. From the imported package use the `Println` function to print text.

It might not make much sense if this is your first time seeing code, but with this *simple* starting point lots of amazing things can be done (every page in the Internet involves some kind of code, be it from the server or the application logic itself).

Try to digest a little on what might be happening that makes this program *run*, how is it that the computer understands the above code? Personally I don't think the *keywords* above make much sense outside of a programming context.

## Excercise

1. Make a program that prints this text (in different lines):

```
Look at the pattern
Can you see what's wrong?
It's supposed to be perfect
(But really it's not)
But really it's not
```

{{% details "Hint" %}}
1. Use multiple `fmt.Println()`
2. Backticks can be used to create text in multiple lines
{{% /details %}}

[> Next](/go/control_flow)
