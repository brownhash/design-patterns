# Problem

Suppose there is a Duck simulator, that animates various kinds of ducks. 
You start implementing it by creating a `class Duck` and with methods like 
`display()`, `fly()`, `quack()`, `swim()` etc..

Now implementing ducks with the above class, 
`class MallardDuck extends Duck` & `class RubberDuck extends Duck`. 
**Something just went really wrong here**.

By doing so, you just gave a rubber duck the ability to fly and quack instead of squeak.

## Wrong Solution

Now you can think of overriding the fly & quack methods 
while implementing the Duck classes. But now consider the case of 
decoy wooden ducks, that aren't supposed to quack and fly.

**Too much duplicate code?**

## Solution

You use interface to define the behaviors that are expected to change. 
And later use these interfaces to extend more behaviors 
by not disturbing the constant behaviors like the `swim()` method.

Follow the [duck](./duck) package.
