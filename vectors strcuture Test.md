## 1. Vectors:
   - Definition: Vectors are resizable arrays, similar to lists in other programming languages. They can store elements of the same data type.
   - Declaration:
     ```rust
     let mut my_vector: Vec<i32> = Vec::new();
     ```
   - Initialization with Values:
     ```rust
     let my_vector = vec![1, 2, 3, 4, 5];
     ```
   - Access Methods:
     - Indexing: Access individual elements using their index. Indexing starts from 0 for the first element.
       ```rust
       let my_vector = vec![1, 2, 3, 4, 5];
       println!("{}", my_vector[0]);  // Output: 1
       ```
     - Mutable Access: Elements of a mutable vector can be modified directly.
       ```rust
       let mut my_vector = vec![1, 2, 3, 4, 5];
       my_vector[2] = 10;
       println!("{:?}", my_vector);  // Output: [1, 2, 10, 4, 5]
       ```
   - Vector Methods: Rust provides many built-in methods to manipulate vectors such as `push()`, `pop()`, `insert()`, `remove()`, `sort()`, `reverse()`, etc.
     ```rust
     let mut my_vector = vec![1, 2, 3, 4, 5];
     my_vector.push(6);  // Adds 6 to the end of the vector
     my_vector.insert(2, 7);  // Inserts 7 at index 2
     my_vector.pop();  // Removes and returns the last element
     my_vector.remove(3);  // Removes the element at index 3
     my_vector.sort();  // Sorts the vector in ascending order
     ```
   - Vector Iteration: Iterate over the elements of a vector using various methods like `for` loops, iterators, etc.
     ```rust
     let my_vector = vec![1, 2, 3, 4, 5];
     for num in my_vector.iter() {
         println!("{}", num);
     }
     ```
   - Vector Length: Get the length of a vector using the `len()` method.
     ```rust
     let my_vector = vec![1, 2, 3, 4, 5];
     println!("{}", my_vector.len());  // Output: 5
     ```
   - Vector Slicing: Extract a portion of the vector using slicing notation.
     ```rust
     let my_vector = vec![1, 2, 3, 4, 5];
     let slice = &my_vector[1..3];
     println!("{:?}", slice);  // Output: [2, 3]
     ```
   - List Comprehensions: Rust doesn't have list comprehensions like Python, but you can achieve similar functionality using iterators and closures.
   - Nested Vectors: Vectors can contain other vectors, enabling the creation of nested data structures.
     ```rust
     let nested_vector = vec![vec![1, 2, 3], vec![4, 5, 6], vec![7, 8, 9]];
     println!("{}", nested_vector[1][0]);  // Output: 4
     ```
   - Vector Operations: Rust supports various operations on vectors such as concatenation (`extend()`), repetition (`repeat()`), and membership (`contains()`).
     ```rust
     let mut vector1 = vec![1, 2, 3];
     let vector2 = vec![4, 5, 6];
     vector1.extend(vector2);  // Concatenates vector2 to vector1
     println!("{:?}", vector1);  // Output: [1, 2, 3, 4, 5, 6]
     ```
   - Cloning Vectors: Create a separate copy of a vector using the `clone()` method.
     ```rust
     let original_vector = vec![1, 2, 3];
     let cloned_vector = original_vector.clone();
     ```
