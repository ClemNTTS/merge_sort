# 🦀 Merge Sort in Rust

This project implements the **merge sort algorithm** in **Rust**. Merge sort works by recursively splitting a list into two sublists, sorting each sublist, and then merging the two sorted sublists into one sorted list.

## How it Works

- **Divide**: The list is divided into two halves recursively until each half contains only one element.
- **Merge**: The sorted sublists are merged back together in ascending order to form the final sorted list.

### Functions

- `merge_sort<T: Ord + Clone>(arr: &[T]) -> Vec<T>`: Recursively sorts the input list by dividing it into two parts.
- `merge<T: Ord + Clone>(left: &[T], right: &[T]) -> Vec<T>`: Merges two sorted sublists into one sorted list.

### Example

Here's an example of how to use the merge sort algorithm to sort an array:

```rust
fn main() {
    let giant_array = [
        93, 84, 12, 56, 23, 78, 41, 91, 37, 65, 18, 87, 29, 48, 100, 32, 67, 53, 81, 97, 
        25, 74, 46, 17, 34, 62, 89, 21, 58, 13, 71, 39, 69, 43, 95, 27, 76, 49, 11, 36, 
        64, 82, 20, 55, 19, 72, 31, 60, 44, 92, 28, 77, 40, 14, 38, 66, 85, 22, 59, 16, 
        70, 33, 61, 47, 94, 26, 75, 42, 15, 35, 63, 83, 24, 57, 10, 73, 30, 68, 45, 96, 
        2, 79, 4, 98, 0, 7, 5
    ];

    println!("{:?}", merge_sort(&giant_array));
}
```

### Requirements

- **Rust Toolchain**: Ensure you have the Rust toolchain installed on your machine. You can install it from [rustup.rs](https://rustup.rs/).

### Running the Program

1. Clone this repository to your local machine.
2. Navigate to the project directory.
3. Compile and run the program using the command:

```sh
cargo run
```

### Expected Output

For the provided array, the sorted result will be:

```
[0, 2, 4, 5, 7, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 53, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 81, 82, 83, 84, 85, 87, 89, 91, 92, 93, 94, 95, 96, 97, 98, 100]
```

This program demonstrates how to use Rust's efficient memory management and generics to implement a classic sorting algorithm.
