## Experiment 7 – Create an Application to Demonstrate HashMap Collection Object  

<H3>ENTER YOUR NAME: PAGADALA MITHUN KALYAN</H3>  
<H3>ENTER YOUR REGISTER NO: 212223040142</H3>  
<H3>EX.NO.5</H3>  
<H3>DATE: 30/10/2025</H3>  

<H1 ALIGN =CENTER> Demonstrating HashMap Collection in Rust </H1>  

## AIM:  
To create a Rust application that demonstrates the use of the HashMap collection object.  

## EQUIPMENTS REQUIRED:  
- Hardware – PCs  
- Software – Visual Studio Code (Version 1.104.0)  
- Rust Installation  

## RELATED THEORETICAL CONCEPT:  

*HashMap in Rust:*  
A HashMap is a collection that stores data as key-value pairs. Keys are unique, and values can be retrieved efficiently using their associated keys.  

*Key Features of HashMap:*  
- Stores data as key-value pairs.  
- Keys must be unique, values can be duplicated.  
- Provides `.insert()` for insertion and `.get()` for retrieval.  
- Useful for fast lookups and mappings.  

## ALGORITHM:  
STEP 1: Start the program. <BR>  
STEP 2: Import `std::collections::HashMap`. <BR>  
STEP 3: Define the `main` function. <BR>  
STEP 4: Create a new HashMap to store key-value pairs. <BR>  
STEP 5: Insert values into the map using `.insert(key, value)`. <BR>  
STEP 6: Iterate and print the key-value pairs. <BR>  
STEP 7: Access values using `.get(key)` and display them. <BR>  
STEP 8: End the program. <BR>  

## PROGRAM:  

// Rust program to demonstrate HashMap Collection

use std::collections::HashMap;

fn main() {
    // Step 4: Create a new HashMap
    let mut student_scores = HashMap::new();

    // Step 5: Insert values into the map
    student_scores.insert(String::from("Alice"), 85);
    student_scores.insert(String::from("Bob"), 90);
    student_scores.insert(String::from("Charlie"), 78);
    student_scores.insert(String::from("Diana"), 92);

    // Step 6: Iterate and print key-value pairs
    println!("Student Scores:");
    for (name, score) in &student_scores {
        println!("{}: {}", name, score);
    }

    // Step 7: Access values using .get()
    println!("\nAccessing specific student's score:");
    let student_name = "Bob";
    match student_scores.get(student_name) {
        Some(score) => println!("{}'s score is {}", student_name, score),
        None => println!("{} not found", student_name),
    }

    // Demonstrating overwriting an existing value
    student_scores.insert(String::from("Alice"), 95);
    println!("\nUpdated Scores after modifying Alice's score:");
    for (name, score) in &student_scores {
        println!("{}: {}", name, score);
    }
}


## OUTPUT:

<img width="1346" height="1000" alt="image" src="https://github.com/user-attachments/assets/416c912f-00f2-46fe-8f3a-bea353e9d3a9" />

<img width="542" height="316" alt="image" src="https://github.com/user-attachments/assets/f30a52ae-905b-41e0-8a6c-5d8a2a4259bf" />


## RESULT:

Thus, the Rust program to demonstrate the HashMap Collection Object was successfully implemented and executed.
