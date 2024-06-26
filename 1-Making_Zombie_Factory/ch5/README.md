# Chapter 5: Structs

Sometimes you need a more complex data type. For this, Solidity provides structs:

```bash
struct Person {
  uint age;
  string name;
}

```

Structs allow you to create more complicated data types that have multiple properties.

    Note that we just introduced a new type, string. Strings are used for arbitrary-length UTF-8 data. Ex. string greeting = "Hello world!"

In our app, we're going to want to create some zombies! And zombies will have multiple properties, so this is a perfect use case for a struct.

    1. Create a struct named Zombie.
    2. Our Zombie struct will have 2 properties: name (a string), and dna (a uint).
