# craftinginterpreters
Coding along with [craftinginterpreters.com](http://craftinginterpreters.com) tutorial.

Implements an interpreter for the "Lox" programming language

```
// Your first Lox program!
print "Hello, world!";

true;  // Not false.
false; // Not *not* false.

1234;  // An integer.
12.34; // A decimal number.

"I am a string";

nil

add + me;
subtract - me;
multiply * me;
divide / me;

-negateMe;

less < than;
lessThan <= orEqual;
greater > than;
greaterThan >= orEqual;

1 == 2;         // false.
"cat" != "dog"; // true.
123 == "123"; // false.

!true;  // false.
!false; // true;

true and false; // false.
true and true;  // true.

false or false; // false.
true or false;  // true.

var average = (min + max) / 2;

{
  print "One statement";
  print "Two statements.";
}

var breakfast = "bagels";
print breakfast; // "bagels".
breakfast = "beignets";
print breakfast; // "beignets".

if (condition) {
  print "yes";
} else {
  print "no";
}

var a = 1;
while (a < 10) {
  print a;
  a = a + 1;
}

for (var a = 1; a < 10; a = a + 1) {
  print a;
}

makeBreakfast(bacon, eggs, toast);
makeBreakfast();

fun printSum(a, b) {
  print a + b;
}

fun outerFunction() {
  fun localFunction() {
    print "I'm local!";
  }

  localFunction();
}

fun returnFunction() {
  var outside = "outside";

  fun inner() {
    print outside;
  }

  return inner;
}

var fn = returnFunction();
fn();

class Breakfast {
  cook() {
    print "Eggs a-fryin'!";
  }

  serve(who) {
    print "Enjoy your breakfast, " + who + ".";
  }
}

// Store it in variables.
var someVariable = Breakfast;

// Pass it to functions.
someFunction(Breakfast);

var breakfast = Breakfast();
print breakfast; // "Breakfast instance".

breakfast.meat = "sausage";
breakfast.bread = "sourdough";

class Breakfast {
  init(meat, bread) {
    this.meat = meat;
    this.bread = bread;
  }

  // ...
}

var baconAndToast = Breakfast("bacon", "toast");
baconAndToast.serve("Dear Reader");

class Brunch < Breakfast {
  init(meat, bread, drink) {
    super.init(meat, bread);
    this.drink = drink;
  }
}
```
