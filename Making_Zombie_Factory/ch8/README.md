# Chapter 8: Working With Structs and Arrays

## Creating New Structs

Remember our Person struct in the previous example?

```bash
struct Person {
  uint age;
  string name;
}

Person[] public people;
```

Now we're going to learn how to create new Persons and add them to our people array.

```bash
// create a New Person:
Person satoshi = Person(172, "Satoshi");

// Add that person to the Array:
people.push(satoshi);
```

We can also combine these together and do them in one line of code to keep things clean:

```bash
people.push(Person(16, "Himanish"));
```

Note that array.push() adds something to the end of the array, so the elements are in the order we added them. See the following example:

```bash
uint[] numbers;
numbers.push(5);
numbers.push(10);
numbers.push(15);
// numbers is now equal to [5, 10, 15]
```

Let's make our createZombie function do something!

    1. Fill in the function body so it creates a new Zombie, and adds it to the zombies array. The name and dna for the new Zombie should come from the function arguments.
    2. Let's do it in one line of code to keep things clean.
