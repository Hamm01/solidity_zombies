# Chapter 12: SafeMath Part 4

Great, now we can implement SafeMath on all the types of uints we used in our DApp!

Let's fix all those potential issues in ZombieAttack. (There was also one zombies[_zombieId].level++; that needed to be fixed in ZombieHelper, but we've taken care of that one for you so we don't take an extra chapter to do so 😉).

1. implement SafeMath methods on all the ++ increments in ZombieAttack. We've left comments in the code to make them easy to find.
