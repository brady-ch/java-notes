# Primitive Types in Java
| Type | Size (bits) | Minimum | Maximum |
|---|---|---|---|
| [[Java Primitives#Boolean \| boolean]] | 1 | - | - |
| [[Java Primitives#Byte \| byte]] | 8 | -2<sup>7</sup>|2<sup>7</sup>-1|
| [[Java Primitives#Short\| short]] | 16 | -2<sup>16</sup>|2<sup>16</sup>-1|
| [[Java Primitives#Int\| int]] | 32 | -2<sup>32</sup>|2<sup>32</sup>-1|
| [[Java Primitives#Long\|long]] | 64 | -2<sup>64</sup>|2<sup>64</sup>-1|
| [[Java Primitives#Float\|float]] | 32 | -2<sup>-149</sup>|(2-2<sup>-23</sup>)·2<sup>127</sup>|
| [[Java Primitives#Double\|double]] | 64 | -2<sup>-1074</sup>|(2-2<sup>-52</sup>)·2<sup>1023</sup>|
| [[Java Primitives#Char\|char]] | 16 | 0 |2<sup>16</sup>-1|


### Considerations
#### Overflow

Overflow is a concern with Java
- Integer Overflow behavior
	- Integers overflow in a manner that you would expect from storing data using the [[Two's Compliment]] method. When there is enough added that the sign bit changes you will have an overflow, and it is represented that way in Java.
- Floating Point Overflow Behavior
	- Overflow will return infinity and Underflow return 0.0


#### Autoboxing
Wrapper classes exist for all primative types
TODO

### Boolean Type

#### Boolean (bit)
- 1 bit of memory
- Can only accept 1 or 0 which can also be expressed as true or false

### Integer Type
- Default value of 0 and decimal values are truncated
- The primitive types that are of the integer type are [[#Byte]], [[#Short]], [[#Int]], and [[#Long]].

#### Byte
- Integer type
- 8 bits of memory
- Default 0


#### Short
- Integer type
- 16 bits of memory


#### Int
 - Integer type
 - 32 bits of memory


#### Long
 - Integer type
 - 64 bits of memory
 - Need to put an L on the end of a number for it to be treated as a long as numbers are treated as an int by default


### Floating Point Types
#### Float
- Floating-point type
- After 6 decimal places it becomes less precise and more of an estimate
- Default 0.0
- Add an f to the end of a number to be explicit


#### Double
- Floating-point type
- has similar precision limitations to float
- Default 0.0
- Add an d to the end of a number to be explicit

### Char Type
#### Char
- A char takes up 16 bits, meaning that it’s capable of representing 65,536 different characters. Each character represented by Unicode has a numeric counterpart. Because of that, chars can be declared using either a literal character or an integer value.
- Default '/u0000'
- Can add unicode characters into a string 

