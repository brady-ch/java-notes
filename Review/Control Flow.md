# Control Flow
## if statements
```java
if(condition){
// things to do if condition is true
}

// The following is shorthand and bad practice however it is still valid
if(condition)
// things to do if condition is true, however it only works on the line directly below the if statemnt

// if then else
if(condition){
doThings();
} else if(otherCondition){ // run this statement if the previous didn't run, you can chain more after this if needed
doOtherThings();
} else { // If no other condition is satisfied run this code block
doDifferentThings();
}
```

## switch statements
```java
switch(value){
	case: 1:
		huh();
		break;
	case: 2;
		huhkay();
		break;
	default:
		huhkayhuhkay();
}
```
## Loops
### for statement (loop)
```java
for(int i = 0; i < y; i++){
huhkay();
}

for(int i = initialValue; condition; ThingToDoWhenRestartingTheLoop){
huhkay();
}

for(statement1; statement2; statement3){
huhkay();
}
// statement1 is excecuted once and only once before the code block
// statement2 defined the condition for excecuting the code block
// statement3 is excecuted every time after the code block has been executed
```
### for-each loop
```java
// iterates over the all elements in an array
String[] huhkay = {"huh", "kay", "huhkay"};
for(String element : huhkay){
System.out.println(element);
}
```

### while statement (loop)
```java
while(condition){
huhkay();
}
```
### do-while statement (loop)
```java
// differs from a normal while loop because it will always run at least once
do {
huhkay();
} while(condition)
```
## Branching Statements
### break
- breaks out of the current code block when inside of a switch statement or a loop
### continue
- continues onto the next iteration/cycle of the loop, breaks one iteration.
### return
- will return the value and end the method