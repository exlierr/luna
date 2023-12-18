**Hello World**
```
// inside Main.luna
.print("Hello, World!");
```

Luna is a purely object oriented language so the above is treated like and can alternatively be programmed like this here.

```
// inside Main.luna
global class Main
{
  constructor Main() -> Main {}

  global static function main(args: Array<String>) -> void
  {
    .print("Hello, World!");
  }

}
```

#
#
#

**Simple Inheritance**
```
// inside Car.luna
global constructor Vehicle() -> Vehicle {}
global constructor Car() extends Vehicle -> Car {}
```

The above is treated and can alternatively be programmed like this.

```
global class Vehicle
{
  global constructor Vehicle() -> Vehicle {}
}

global class Car extends Vehicle
{
  global constructor Car() -> Car {}
}
```
