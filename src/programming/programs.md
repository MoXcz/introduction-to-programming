# What is a Program?

A program is simply a set of instructions that *solve* something through an applied medium—plain and simple. The act of *programming* refers to the process of *teaching* or *instructing* a system how to perform a task, and the result of that process is a program.

So if I say I want a program that performs multiplication and division, I need to define the rules and steps that, when followed, allow someone—or something—to do exactly that:

### Multiplication

1. You need at least two numbers: `x` and `y`.
2. To *multiply* the two numbers, compute `x * y`.
3. Conceptually, multiplication can be defined as adding `x` to itself `y` times.

### Division

1. Again, you need two numbers: `x` and `y`.
2. To *divide*, compute `x / y`.
3. Conceptually, division can be thought of as figuring out how many times `y` can be added until it equals `x`.

That’s a rough, human-level algorithm—a *programmable* way to think about solving a problem.

Now, putting that into code, here's how such logic might look in Rust. Don't worry about the details like `i32` or `f64` just yet. For now, it's enough to know that:

- `i32` represents a whole number (integer).
- `f64` represents a number with decimals (a floating-point number).

```rust
fn multiply(x: i32, y: i32) -> i32 {
    x * y
}

fn divide(x: i32, y: i32) -> f64 {
    x as f64 / y as f64
}
```

At this stage, the functions above (think of them as named sets of instructions) might not make complete sense, especially because Rust is a relatively low-level language. That’s okay. The key takeaway is that *programs* are formalized instructions—like recipes—that tell the computer how to solve a specific problem.

