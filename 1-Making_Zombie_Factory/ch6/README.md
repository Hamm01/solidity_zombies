# Chapter 6: Arrays

When you want a collection of something, you can use an array. There are two types of arrays in Solidity: fixed arrays and dynamic arrays:

```bash
// Array with a fixed length of 2 elements:
uint[2] fixedArray;
// another fixed Array, can contain 5 strings:
string[5] stringArray;
// a dynamic Array - has no fixed size, can keep growing:
uint[] dynamicArray;

```

You can also create an array of structs. Using the previous chapter's Person struct:

```bash
Person[] people; // dynamic Array, we can keep adding to it

```

Remember that state variables are stored permanently in the blockchain? So creating a dynamic array of structs like this can be useful for storing structured data in your contract, kind of like a database.

Public Arrays
You can declare an array as public, and Solidity will automatically create a getter method for it. The syntax looks like:

```bash
Person[] public people;

```

Other contracts would then be able to read from, but not write to, this array. So this is a useful pattern for storing public data in your contract.

We're going to want to store an army of zombies in our app. And we're going to want to show off all our zombies to other apps, so we'll want it to be public. 1. Create a public array of Zombie structs, and name it zombies.
