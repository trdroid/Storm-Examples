# Tuple

The nodes in a Storm Topology send data between one another in the form of *tuples*.

A *tuple* in Storm has the following properties

* It is an ordered list of values
* Each value in the list is assigned a name

### Dynamic Types

The types of the values in a *tuple* need not be declared and can be dynamic. 

### Serialization

Storm serializes the values of a *tuple* to send the *tuple* between nodes in a *topology*. 

**Primitive Types**

*Primitive Types* need no serialization as it is handled by Storm.

**Custom Types**

*Custom Types* will have to provide custom serializers so Storm can serialize the values of custom types to allow *tuples* to be sent between nodes.
In cases where custom serializers are not provided for custom types, Storm falls back to standard Java serialization.

### Named Values

Each value in a *tuple* is assigned a name, but

* A *tuple* is not represented using a *map* underneath the hoods
* A *tuple* is not a list of name-value pairs i.e. the names are not stored along with their values



