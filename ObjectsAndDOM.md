## Objects:
- Objects represent things.  They consist of
    - properties, which are like variables
    - methods, which are like functions
- Properties and methods have a Key and a Value
    - The Key is the name of a property and method
    - The Value of a Property can be a string, Boolean, array, or another object
    - The Value of a Method is always a function
- Ways to create Objects
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
