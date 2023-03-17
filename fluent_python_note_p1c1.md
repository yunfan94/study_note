Python Data Model

1. python collections.namedtuple

Arguments:
typename: provided class name for the namedtuple
field_names: a)An iterable of strings; b) A string with each field name separated by whitespace c) A string with each field name separated by commas

Creation:
can create a named tuple using keyword arguments

Using Optional Arguments:
rename
rename to True, then all the invalid field names are automatically replaced with positional names.
use case read csv files colnums name automatically transfer invalid name to `_index`
defaults
set defaults to an iterable of values. In this case, namedtuple() assigns the values in the defaults iterable to the rightmost fields:
module

additional Features of namedtuple Classes
 ._make() to create named tuple instances
 ._asdict() to convert existing named tuple instances into dictionaries.
._replace() takes keyword arguments of the form field=value and returns a new namedtuple instance updating the values of the selected fields

Exploring Additional namedtuple Attributes
._fields, you can use it to introspect your namedtuple classes and instances. You can also create new classes from existing ones:
._field_defaults, you can introspect namedtuple classes and instances to find out what fields provide default values


Use case
Using Field Names Instead of Indices
Returning Multiple Named Values From Functions
Reducing the Number of Arguments to Functions
Reading Tabular Data From Files and Databases
https://realpython.com/python-namedtuple/
