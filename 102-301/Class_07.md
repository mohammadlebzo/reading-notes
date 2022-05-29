# HTML & CSS
## Tables
Tables represent information in a grid format.

### Table Structure:
- `<table>` *tag*: used to create the table.
- `<tr>` *tag*: used to indicate the start of a row.
- `<td>` *tag*: used to represent a cell.
- `<th>` *tag*: used to represent the heading for a column or a row

**ex**:

```
<table>
    <tr>
        <th></th>
        <th>9am</th>
        <th>10am</th>
        <th>11am</th>
        <th>12am</th>
    </tr>
    <tr>
        <th>Monday</th>
        <td colspan="2">Geography</td>
        <td>Math</td>
        <td>Art</td>
    </tr>
    <tr>
        <th>Tuesday</th>
        <td colspan="3">Gym</td>
        <td>Home Ec</td>
    </tr>
</table>
```

### Long Tables:
Used to distinguish between the main content of the table and the first and last rows. There are three elements that help with that:

- `<thead>` *tag*: it represent the heading.
- `<tbody>` *tag*: it represent the body.
- `<tfoot>` *tag*: it represent the footer.

# JavaScript
## Objects
**Objects** group together a set of variables and functions to create a model of a something you would recognize from the real world.

Inside **objects**, variables are called **properties** and functions are called **methods**. 

### Creating an Object: Literal Notation:

**ex**:

```
let hotle =     >> Object
{
    name: 'Quay',      >> 
    rooms: 40,         >>
    booked: 25,        >>   Properties
    gym: true,         >>

    roomTyps:['twin', 'double', 'suite'],   >>
    checkAvailability: function()           >>
    {                                       >>  Method
        return this.rooms - this.booked;    >>
    }                                       >>
};
```

### Accessing an object:
There are two notations for accessing objects:
- **Dot Notation**. **ex**: `let hotelName = hotle.name;`
- **Bracket Notation**. **ex**: `let hotelName = hotle['name'];`

### Creating an Object: Constructor Notation:

```
let hotle = new Object();    >> Object

    hotel.name: 'Quay',      >> 
    hotel.rooms: 40,         >>
    hotel.booked: 25,        >>   Properties
    hotel.gym: true,         >>

    hotel.roomTyps:['twin', 'double', 'suite'],   >>
    checkAvailability: function()                 >>
    {                                             >>  Method
        return this.rooms - this.booked;          >>
    }                                             >>
```

### Creating Many Object: Constructor Notation:

```
function Hotel(name, rooms, booked)
{
    this.name: 'Quay',      >> 
    this.rooms: 40,         >>
    this.booked: 25,        >>   Properties
    this.gym: true,         >>

    this.roomTyps:['twin', 'double', 'suite'],   >>
    checkAvailability: function()                >>
    {                                            >>  Method
        return this.rooms - this.booked;         >>
    }                                            >>
}
let parkHotel = new Hotel('Park', 120, 77, false);
```

### Groups of built-in objects:
- **Browser Object Model(BOM)**: creates a model of the browser tab or window.
![BOM](https://static.javatpoint.com/images/javascript/bom.jpg)

- **Document Object Model(DOM)**:creates a model of the current webpage.
[read more](https://mohammadlebzo.github.io/reading-notes/Class_07)

- **Global JavaScript Objects**: they are a group of individual objects that relate to different parts of the JavaScript language.

Objects that represent basic data types:
- **String**: works with string values.
- **Number**: works with numeric values.
- **Boolean**: works with boolean values.

Objects that help deal with real-world concepts:
- **Date**: represent and handle dates.
- **Math**: works with numbers and calculations.
- **Regex**: for matching patterns within strings of text.

### Creating instances of objects:

**ex**:

```
let today = new Date();
```
