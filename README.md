**Hello World**
```ts
// inside Main.luna
.print("Hello, World!");
```

Luna is a purely object oriented language.

#
#
#

**Simple Inheritance**
```ts
// inside Vehicle.luna
class Vehicle; // this is implicit and can be removed if desired.

location: Location = new Location();

Vehicle() {} // constructor

getLocation() -> Location { return this.location; }
setLocation(location: Location) { this.location = location; }
```

```ts
// inside Car.luna
class Vehicle; // this is implicit and can be removed if desired.
extends Vehicle;

Car() {}

@Override
getLocation() -> Array<Integer> { return [super.location.getX(), super.location.getY(), super.location.getZ()]; }
```
