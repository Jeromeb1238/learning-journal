## Objects:
- Objects represent things.  They consist of
    - properties, which are like variables
    - methods, which are like functions
- Properties and methods have a Key and a Value
    - The Key is the name of a property and method
    - The Value of a Property can be a string, Boolean, array, or another object
    - The Value of a Method is always a function

Ways to create Objects
- Literal Notation:
```javascript
var hotel = {
name: 'Quay',
rooms: 40,
booked: 25,
checkAvailability: function() {
  return this.rooms - this.booked;
  }
 };
- Note the this in `this.rooms` 'This' refers to this hotel because it is contained within the Object
```
   - Accessing an Object `var hotelName = hotel.name;` or `var roomsFree = hotel.checkavailability();`
   - Create an Object using Constructor Notation
```javascript
var hotel = new Object();

Note two items: first this method uses `new` and `Object`  `new` is a js keyword and `Object();`
the constructor function.  Also not capitalized 'O' in Object, used to denote Constructor Notation
```
- To **add** or change **value** of items to a new Object use the Object name and assign a Key and Value:
```javascript
hotel.name = 'Quay';
hotel.rooms = 40;
hotel.booked = 25;
hotel.checkAvaiolability = function() {
return this.rooms - this.booked;
};

Note: again this refers to \this object, and capitalized first letter of Object name
```
- Creating **many** Objects using Constructor Notation:
```javascript
function Hotel(name, rooms, booked) {
this.name = name;
this.rooms = rooms;
this.booked = booked;
this.checkAvailability = function () {
return this.rooms - this.booked;
};

Note: again this is referencing \this Object's name and capitalized first letter of Object Name
```
- You create an **Instance** of an Object Construction by using the keyword 'new' followed by the Object name.  For ex.
```javascript
var quayHotel = new Hotel('Quay', 40, 25);
```
   
