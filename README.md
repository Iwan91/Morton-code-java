# Morton code for java
Usage:
```java
//range for (x,y,z) is (0,0,0) to (2097151,2097151,2097151) !!!
int x=100;
int y=200;
int z=2;

//return 64-bit unsigned long 
long mortonCode=MortonCode3D64BitsLookupTable.encode(100,200,2);

//return 3 element array
//xyz[0] -> our x
//xyz[1] -> our y
//xyz[2] -> our z
int[] xyz=MortonCode3D64BitsLookupTable.decode(mortonCode);

//get only x
int x2=MortonCode3D64BitsLookupTable.decodeX(mortonCode);

//get only y
int y2=MortonCode3D64BitsLookupTable.decodeY(mortonCode);

//get only z
int z2=MortonCode3D64BitsLookupTable.decodeY(mortonCode);
```

### More info about Morton code:
https://en.wikipedia.org/wiki/Z-order_curve
