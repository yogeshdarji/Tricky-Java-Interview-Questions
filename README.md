# Tricky-Java-Interview-Questions
This repository contains all the important and tricky java questions which I have faced during interviews over the years

**Q) Can you overload a main method in java?** <br />
A)Yes, you can overload a main method

**Q) What is the output of the following?**

```
String s = "Hello, how are you doing ?";
System.out.println(s.substring(5, 3));
```
  
  A) `java.lang.StringIndexOutOfBoundsException: String index out of range: -2`

 **Q) What is the output of the following?**
 
 ```
 String s = "ONE"+1+2+"TWO"+"THREE"+3+4;
 System.out.println(s);
 ```
 A ) `ONE12TWOTHREE34`
 
 **Q) What is the output of following?**
 ``` fff
 int i = 10++11--12++13--14++15;
 System.out.println(i);
 ```
 A) 75.Beacuse 10+11+12+13+14+15 = 75, all these are unary operators.
 
  **Q) What is the difference between HashMap and Concurrent HashMap?**
  
  A) Below are the difference between HashMap and ConcurrentHashMap:
- ConcurrentHashMap was made to make HashMap thread-safe and synchronized.   
- HashMap can be synchronized by wrapping it on Collections.synchornizedMap(HashMap) which will return a collection which is almost equivalent to Hashtable, where every modification operation on Map is locked on Map object while in case of ConcurrentHashMap, thread-safety is achieved by dividing whole Map into different partition based upon Concurrency level and only locking particular portion instead of locking the whole Map

 **Q) How to set the java initial heap size and maximum heap size?**
  
  A) `java -Xms1g` - to set intial Java heap size
     `java -Xmx6g` - to set maximum Java heap size
  
