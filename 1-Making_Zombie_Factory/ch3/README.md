# Chapter 3: State Variables & Integers

Now that we've got a shell for our contract, let's learn about how Solidity deals with variables.

State variables are permanently stored in contract storage. This means they're written to the Ethereum blockchain. Think of them like writing to a DB.

Example:

```bash
 contract Example {
  // This will be stored permanently in the blockchain
  uint myUnsignedInteger = 100;
}

```

In this example contract, we created a uint called myUnsignedInteger and set it equal to 100.

    Unsigned Integers: uint

The uint data type is an unsigned integer, meaning its value must be non-negative. There's also an int data type for signed integers.

    Note: In Solidity, uint is actually an alias for uint256, a 256-bit unsigned integer. You can declare uints with less bits — uint8, uint16, uint32, etc.. But in general you want to simply use uint except in specific cases, which we'll talk about in later lessons.
