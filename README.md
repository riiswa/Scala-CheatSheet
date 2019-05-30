
# Scala Cheat Sheet

- Author : Waris RADJI student at Université Paris XIII
- Source : https://www.amazon.fr/SCALA-Pas-%C3%A0-Gildas-M%C3%A9nier/dp/2340000092

<h1>Table of Contents<span class="tocSkip"></span></h1>
<div class="toc"><ul class="toc-item"><li><span><a href="#Scala-Cheat-Sheet" data-toc-modified-id="Scala-Cheat-Sheet-1">Scala Cheat Sheet</a></span><ul class="toc-item"><li><span><a href="#Scala-essentials" data-toc-modified-id="Scala-essentials-1.1">Scala essentials</a></span><ul class="toc-item"><li><span><a href="#Display-and-Strings" data-toc-modified-id="Display-and-Strings-1.1.1">Display and Strings</a></span><ul class="toc-item"><li><span><a href="#Blocks-and-expressions" data-toc-modified-id="Blocks-and-expressions-1.1.1.1">Blocks and expressions</a></span></li></ul></li><li><span><a href="#Method-definitions" data-toc-modified-id="Method-definitions-1.1.2">Method definitions</a></span></li><li><span><a href="#Conditional" data-toc-modified-id="Conditional-1.1.3">Conditional</a></span></li><li><span><a href="#Pattern-matching" data-toc-modified-id="Pattern-matching-1.1.4">Pattern matching</a></span></li><li><span><a href="#Exceptions" data-toc-modified-id="Exceptions-1.1.5">Exceptions</a></span></li><li><span><a href="#Parametric-type" data-toc-modified-id="Parametric-type-1.1.6">Parametric type</a></span></li></ul></li><li><span><a href="#Object-oriented-programming" data-toc-modified-id="Object-oriented-programming-1.2">Object oriented programming</a></span><ul class="toc-item"><li><span><a href="#General-hierarchy-of-classes-/-traits-/-objects" data-toc-modified-id="General-hierarchy-of-classes-/-traits-/-objects-1.2.1">General hierarchy of classes / traits / objects</a></span></li><li><span><a href="#object" data-toc-modified-id="object-1.2.2">object</a></span></li><li><span><a href="#class" data-toc-modified-id="class-1.2.3">class</a></span></li></ul></li><li><span><a href="#Arrays" data-toc-modified-id="Arrays-1.3">Arrays</a></span><ul class="toc-item"><li><span><a href="#Declaration-of-array" data-toc-modified-id="Declaration-of-array-1.3.1">Declaration of array</a></span></li><li><span><a href="#Access-to-the-elements" data-toc-modified-id="Access-to-the-elements-1.3.2">Access to the elements</a></span></li><li><span><a href="#Iteration-on-the-elements-of-an-array" data-toc-modified-id="Iteration-on-the-elements-of-an-array-1.3.3">Iteration on the elements of an array</a></span></li><li><span><a href="#Creating-an-array-by-transformation" data-toc-modified-id="Creating-an-array-by-transformation-1.3.4">Creating an array by transformation</a></span><ul class="toc-item"><li><span><a href="#for/yield" data-toc-modified-id="for/yield-1.3.4.1">for/yield</a></span></li><li><span><a href="#filter" data-toc-modified-id="filter-1.3.4.2">filter</a></span></li><li><span><a href="#map" data-toc-modified-id="map-1.3.4.3">map</a></span></li><li><span><a href="#sortWith" data-toc-modified-id="sortWith-1.3.4.4">sortWith</a></span></li><li><span><a href="#reduce" data-toc-modified-id="reduce-1.3.4.5">reduce</a></span></li></ul></li><li><span><a href="#Arrays-with-a-variable-size" data-toc-modified-id="Arrays-with-a-variable-size-1.3.5">Arrays with a variable size</a></span></li></ul></li><li><span><a href="#Main-collections" data-toc-modified-id="Main-collections-1.4">Main collections</a></span><ul class="toc-item"><li><span><a href="#Principles" data-toc-modified-id="Principles-1.4.1">Principles</a></span></li><li><span><a href="#Tuples" data-toc-modified-id="Tuples-1.4.2">Tuples</a></span></li><li><span><a href="#Map" data-toc-modified-id="Map-1.4.3">Map</a></span><ul class="toc-item"><li><span><a href="#Map-implementations" data-toc-modified-id="Map-implementations-1.4.3.1">Map implementations</a></span></li></ul></li><li><span><a href="#Option" data-toc-modified-id="Option-1.4.4">Option</a></span></li><li><span><a href="#Either" data-toc-modified-id="Either-1.4.5">Either</a></span></li><li><span><a href="#Lists" data-toc-modified-id="Lists-1.4.6">Lists</a></span></li><li><span><a href="#Set" data-toc-modified-id="Set-1.4.7">Set</a></span><ul class="toc-item"><li><span><a href="#Set-Implementations" data-toc-modified-id="Set-Implementations-1.4.7.1">Set Implementations</a></span></li></ul></li><li><span><a href="#Vector" data-toc-modified-id="Vector-1.4.8">Vector</a></span></li><li><span><a href="#Stack" data-toc-modified-id="Stack-1.4.9">Stack</a></span></li><li><span><a href="#Queue" data-toc-modified-id="Queue-1.4.10">Queue</a></span></li><li><span><a href="#Range" data-toc-modified-id="Range-1.4.11">Range</a></span></li><li><span><a href="#Streams" data-toc-modified-id="Streams-1.4.12">Streams</a></span></li></ul></li><li><span><a href="#Collections-in-detail" data-toc-modified-id="Collections-in-detail-1.5">Collections in detail</a></span><ul class="toc-item"><li><span><a href="#Traversable" data-toc-modified-id="Traversable-1.5.1">Traversable</a></span></li><li><span><a href="#Iterable" data-toc-modified-id="Iterable-1.5.2">Iterable</a></span></li><li><span><a href="#Seq" data-toc-modified-id="Seq-1.5.3">Seq</a></span></li><li><span><a href="#Usual-operations" data-toc-modified-id="Usual-operations-1.5.4">Usual operations</a></span><ul class="toc-item"><li><span><a href="#Add-/-remove-an-element" data-toc-modified-id="Add-/-remove-an-element-1.5.4.1">Add / remove an element</a></span></li><li><span><a href="#Update" data-toc-modified-id="Update-1.5.4.2">Update</a></span></li><li><span><a href="#Assemblist-operations" data-toc-modified-id="Assemblist-operations-1.5.4.3">Assemblist operations</a></span></li><li><span><a href="#Cast" data-toc-modified-id="Cast-1.5.4.4">Cast</a></span></li><li><span><a href="#Operations-of-Iterables" data-toc-modified-id="Operations-of-Iterables-1.5.4.5">Operations of Iterables</a></span></li><li><span><a href="#Selection-and-cutting" data-toc-modified-id="Selection-and-cutting-1.5.4.6">Selection and cutting</a></span></li><li><span><a href="#Transformation-of-a-collection" data-toc-modified-id="Transformation-of-a-collection-1.5.4.7">Transformation of a collection</a></span></li></ul></li></ul></li></ul></li></ul></div>

## Scala essentials


```Scala
var a = 5 // variable
var b: Int = 5 // variable with explicit typing
val zero = 0 // constant
```




    0



### Display and Strings


```Scala
val name = "joe"
"Hello " + name + " how are you ?"
// or
s"Hello $name how are you ?"
```




    Hello joe how are you ?




```Scala
s"2 + 2 = ${2+2}"
```




    2 + 2 = 4




```Scala
raw"\nature"// The "\n" is not escaped
```




    \nature




```Scala
printf("pi = %2.2f\n", 3.1415)
f"pi = ${3.1415}%2.2f" 
```

    pi = 3,14





    pi = 3,14




```Scala
"""1...
2...
3."""
// ou
"""1...
    |2...
    |3.""".stripMargin // stripMargin("#") to change the default value
```




    1...
    2...
    3.



#### Blocks and expressions


```Scala
{val a = 6; val b = 4; a + b}
```




    10




```Scala
def f: Int = {val a = 6; return a; val b = 7; a + b} // return interrupts the evaluation
```




    6




```Scala
scala.math.sin(3.14)
// or (when the function only takes one parameter)
scala.math.sin{3.14}
```




    0.0015926529164868282




```Scala
lazy val a = {println("Statement of a");1} // evaluate when the variable is called
val b = {println("Statement of b");2}
a+b
```

    Statement of b
    Statement of a





    3



### Method definitions


```Scala
def a = 1
```




    1




```Scala
def sum(v1: Int, v2: Int) = v1 + v2
def sum1(v1: Int, v2: Int): Int = v1 + v2 // to indicate the type of return
```




    sum: (v1: Int, v2: Int)Int
    sum1: (v1: Int, v2: Int)Int





```Scala
def zeroOrx(x: Int = 0) = x // parameter with default value
s"${zeroOrx()}, ${zeroOrx(100)}"
```




    0, 100




```Scala
def mean(x: Int*) = x.sum / x.size
mean(1, 2, 3, 4, 5)
```




    3




```Scala
// procedure (Unit): possibility to remove the "="
def unit() {println("Unit")}
```

    Unit





    null




```Scala
val flagColor: (String, String, String) => String = (c1, c2, c3) => {c1 + " " + c2 + " " + c3}
// ou
val flagColor1 = (c1: String, c2: String, c3: String) => {c1 + " " + c2 + " " + c3}
```




    <function3>



### Conditional


```Scala
if (scala.util.Random.nextFloat > 0.5) "win" else "loose"
```




    loose



### Pattern matching


```Scala
scala.util.Random.nextInt match {
    case 0 => println("zero")
    case a if a > 0 => println("positive")
    case a if a < 0 => println("negative")
    case _ => println("end")
}
```

    positive


### Exceptions


```Scala
throw new Exception("...")
```


    java.lang.Exception: ...
    
      ... 44 elided



```Scala
try {
    1 / 0 
} catch {
    case ex: ArithmeticException => ex.printStackTrace()
    case ex: Exception => ex.printStackTrace()
    case _ => println("Nothing")
}
```

    java.lang.ArithmeticException: / by zero
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.liftedTree1$1(<console>:91)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:90)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:101)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:103)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:105)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:107)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:109)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:111)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:113)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:115)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:117)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:119)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:121)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:123)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:125)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw$$iw.<init>(<console>:127)
    	at $line46.$read$$iw$$iw$$iw$$iw$$iw.<init>(<console>:129)
    	at $line46.$read$$iw$$iw$$iw$$iw.<init>(<console>:131)
    	at $line46.$read$$iw$$iw$$iw.<init>(<console>:133)
    	at $line46.$read$$iw$$iw.<init>(<console>:135)
    	at $line46.$read$$iw.<init>(<console>:137)
    	at $line46.$read.<init>(<console>:139)
    	at $line46.$read$.<init>(<console>:143)
    	at $line46.$read$.<clinit>(<console>)
    	at $line46.$eval$.$print$lzycompute(<console>:7)
    	at $line46.$eval$.$print(<console>:6)
    	at $line46.$eval.$print(<console>)
    	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
    	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
    	at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
    	at java.base/java.lang.reflect.Method.invoke(Method.java:566)
    	at scala.tools.nsc.interpreter.IMain$ReadEvalPrint.call(IMain.scala:793)
    	at scala.tools.nsc.interpreter.IMain$Request.loadAndRun(IMain.scala:1054)
    	at scala.tools.nsc.interpreter.IMain$WrappedRequest$$anonfun$loadAndRunReq$1.apply(IMain.scala:645)
    	at scala.tools.nsc.interpreter.IMain$WrappedRequest$$anonfun$loadAndRunReq$1.apply(IMain.scala:644)
    	at scala.reflect.internal.util.ScalaClassLoader$class.asContext(ScalaClassLoader.scala:31)
    	at scala.reflect.internal.util.AbstractFileClassLoader.asContext(AbstractFileClassLoader.scala:19)
    	at scala.tools.nsc.interpreter.IMain$WrappedRequest.loadAndRunReq(IMain.scala:644)
    	at scala.tools.nsc.interpreter.IMain.interpret(IMain.scala:576)
    	at scala.tools.nsc.interpreter.IMain.interpret(IMain.scala:572)
    	at com.twosigma.beakerx.scala.evaluator.ScalaEvaluatorGlue.evaluate(ScalaEvaluatorGlue.scala:121)
    	at com.twosigma.beakerx.scala.evaluator.ScalaCodeRunner.call(ScalaCodeRunner.java:46)
    	at com.twosigma.beakerx.scala.evaluator.ScalaCodeRunner.call(ScalaCodeRunner.java:29)
    	at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
    	at java.base/java.lang.Thread.run(Thread.java:834)





    ()



### Parametric type


```Scala
def hey[T](x: T) = "Hey " + x.toString
// equivalent to 
def hey1(x: Any) = "Hey " + x.toString
hey[String]("Joe") + " " + hey1(122)
```




    Hey Joe Hey 122




```Scala
import Ordering.Implicits._
```




    scala.math.Ordering$Implicits$@61d25c2b




```Scala
def greaterThan[T: Ordering](x: T, y: T): Boolean = x > y
moreThan(1, 3)
```


    <console>:95: error: not found: value moreThan
    
           moreThan(1, 3)
    
           ^



```Scala
type ArrInt = Array[Int] // type alias
```




    defined type alias ArrInt




 ## Object oriented programming

### General hierarchy of classes / traits / objects

<img src="https://scala-lang.org/files/archive/spec/2.12/public/images/classhierarchy.png">

### object


```Scala
object Test {
    def main(args: String*){
        println("Hello world!")
    }
}
```




    $line54.$read$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$$iw$Test$@3f9c19c3



### class


```Scala
class Money(startMoney: Int) {
    def this() = this(0) // builder
    private var contain: Int = 0
    def +=(money: Int) = contain += money
    def empty = {val solde = contain; contain = 0; solde}
    def howMany = contain
    override def toString = contain.toString
}
object Money {
    // method and static variables
    def foo = "bar"
}
```




    $line55.$read$$iw$$iw$Money$@797ce733




```Scala
val m = new Money()
m += 10
m.empty
```




    10




```Scala
Money.foo
```




    bar



## Arrays

### Declaration of array


```Scala
val ints = new Array[Int](30) // empty array
val ints2 = Array[Int](1, 2, 3, 4) // array with init values
```




    [1, 2, 3, 4]




```Scala
val matrix4x9 = Array.ofDim[Double](4, 9)
```




    [[0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]]



### Access to the elements


```Scala
ints2(3)
```




    4




```Scala
ints2(3) = 1000 
// or
ints2.update(3, 1000)
ints2(3)
```




    1000



### Iteration on the elements of an array


```Scala
val days = Array("Monday", "Tuesday", "Wednesday", "Thrusday", "Friday", "Saturday", "Sunday")
```




    [Monday, Tuesday, Wednesday, Thrusday, Friday, Saturday, Sunday]




```Scala
var i = 0
while(i < days.length){
    println(days(i))
    i += 1
}
```

    Monday
    Tuesday
    Wednesday
    Thrusday
    Friday
    Saturday
    Sunday





    null




```Scala
for (i <- 0 until days.length) println(days(i))
```

    Monday
    Tuesday
    Wednesday
    Thrusday
    Friday
    Saturday
    Sunday



```Scala
for (day <- days) println(day)
```

    Monday
    Tuesday
    Wednesday
    Thrusday
    Friday
    Saturday
    Sunday



```Scala
days foreach println
```

    Monday
    Tuesday
    Wednesday
    Thrusday
    Friday
    Saturday
    Sunday


### Creating an array by transformation

#### for/yield


```Scala
val daysToUpperCase = for(day <- days) yield day.toUpperCase
```




    [MONDAY, TUESDAY, WEDNESDAY, THRUSDAY, FRIDAY, SATURDAY, SUNDAY]




```Scala
val daysWithLetterE = for(day <- days if day.contains("e")) yield day
```




    [Tuesday, Wednesday]




```Scala
val ints = Array(1, 2, 3, 4)
val chars = Array('a', 'b', 'c', 'd')
for (int <- ints; char <- chars) yield int.toString + char.toString
```




    [1a, 1b, 1c, 1d, 2a, 2b, 2c, 2d, 3a, 3b, 3c, 3d, 4a, 4b, 4c, 4d]



#### filter


```Scala
Array(1, 2, 3, 4, 5).filter(x => x % 2 == 0)
```




    [2, 4]



#### map


```Scala
Array(1, 2, 3, 4, 5).map(x => x*x)
```




    [1, 4, 9, 16, 25]



#### sortWith


```Scala
Array(3, 6, 2, 0, 8, 5).sortWith((e1, e2) => e1 < e2)
```




    [0, 2, 3, 5, 6, 8]



#### reduce


```Scala
Array(1, 2, 3, 4, 5).reduce((e1, e2) => e1+e2) // équivalent à Array(1, 2, 3, 4, 5).sum
```




    15



### Arrays with a variable size


```Scala
import scala.collection.mutable.ArrayBuffer
```




    import scala.collection.mutable.ArrayBuffer





```Scala
val arr = ArrayBuffer[Int]()
```




    [[]]




```Scala
arr += 25
```




    [[25]]




```Scala
arr += (1, 2, 3, 4)
```




    [[25, 1, 2, 3, 4]]




```Scala
arr.insert(2, 5, 5)
arr
```




    [[25, 1, 5, 5, 2, 3, 4]]




```Scala
arr ++= Array(99, 99)
```




    [[25, 1, 5, 5, 2, 3, 4, 99, 99]]




```Scala
arr.remove(4)
```




    2



## Main collections

### Principles

- Lazy evaluation: Allows to delay the transformation operations and thus to calculate or store only if necessary.

- Parallelization support: Method calls do not change. They are just calling in parallel instead of calling them one after the other.

- Mutable: Write access.

- Immutable: No write access.

### Tuples

Storage of values


```Scala
val oneAndTwo = (1, 2)
val oneAndTwo1 = Tuple2(1, 2) // There are tuples that range from 1 element to 22
val oneAndTwo2 = 1 -> 2
```




    (1,2)




```Scala
s"${oneAndTwo._1}, ${oneAndTwo._2}"
```




    1, 2




```Scala
val (a, b, _, d) = (1, 2, 3, 4)  // "_" for a meaningless value
s"$a $b $d"
```




    1 2 4



### Map

Key-value couple


```Scala
val map = Map(("one", 1), ("two", 2))
val map1 = Map("one" -> 1, "two" -> 2)
```




```Scala
map("two")
```




    2




```Scala
map.getOrElse("three", -1)
```




    -1




```Scala
val mutableMap = scala.collection.mutable.Map[String, Int]()
mutableMap("three") = 3
mutableMap += (("one" -> 1), ("two" -> 2))
mutableMap -= "one"
mutableMap += "five" -> 5
```




    Map(three -> 3, five -> 5, two -> 2)




```Scala
val reverseMap = for((key, value) <- mutableMap) yield (value, key)
// or
mutableMap.map(element => (element._2, element._1))
```




    Map(2 -> two, 5 -> five, 3 -> three)




```Scala
s"keys: ${mutableMap.keys} values: ${mutableMap.values}"
```




    keys: Set(three, five, two) values: HashMap(3, 5, 2)




```Scala
mutableMap.partition(_._2 % 2 == 0) // cut a Map according to a predicate
```




    (Map(two -> 2),Map(three -> 3, five -> 5))



#### Map implementations

##### Immutable


```Scala
import scala.collection.immutable

immutable.HashMap[AnyVal, AnyVal]()
immutable.IntMap[AnyVal]()
immutable.ListMap[AnyVal, AnyVal]()
immutable.LongMap[AnyVal]()
immutable.SortedMap[Int, AnyVal]()
immutable.TreeMap[Int, AnyVal]()
```



##### Mutable


```Scala
import scala.collection.mutable

mutable.HashMap[AnyVal, AnyVal]() 
mutable.LinkedHashMap[AnyVal, AnyVal]() 
mutable.ListMap[AnyVal, AnyVal]() 
mutable.OpenHashMap[AnyVal, AnyVal]()
mutable.WeakHashMap[AnyVal, AnyVal]()
```




    Map()



### Option

Presence (Some) or not (None) of value


```Scala
val emptyOpt: Option[Int] = None
```




    None




```Scala
val fullOpt: Option[Int] = Some(42)
```




    Some(42)




```Scala
emptyOpt match {
    case Some(value) => println(value)
    case None => println("Empty")
}
```

    Empty



```Scala
fullOpt.get
```




    42




```Scala
emptyOpt.isEmpty
```




    true



### Either

Choice between 2 return values


```Scala
def divide(a: Double, b: Double): Either[String, Double] = {
    if (b==0.0) Left("Division by zero") else Right(a/b)
}
divide(4, 0)
```




    Left(Division by zero)




```Scala
divide(4, 2)
```




    Right(2.0)



### Lists

Object sequence defined in recursive ways


```Scala
val list = List(1, 2, 3, 4)
```




    [[1, 2, 3, 4]]




```Scala
list.head
```




    1




```Scala
list.tail
```




    [[2, 3, 4]]




```Scala
list.tail.tail.head
```




    3




```Scala
list.tail.tail.tail.tail
```




    [[]]




```Scala
Nil
```




    [[]]




```Scala
1 :: List(2, 3, 4)
```




    [[1, 2, 3, 4]]




```Scala
1 :: 2 :: 3 :: 4 :: Nil
```




    [[1, 2, 3, 4]]




```Scala
list(3)
```




    4




```Scala
def lCount(lst: List[Int], func: (Int) => Boolean): Int = {
    if (lst == Nil) 0 else
        (if (func(lst.head)) 1 else 0) + lCount(lst.tail, func)
}
lCount(List(1, 2, 3, 4), _ % 2 == 0)
```




    2



### Set

Non-ordered collection with each element present only once


```Scala
val set = Set(1, 2, 3, 4)
set + 3
```




    Set(1, 2, 3, 4)




```Scala
set contains 1
// or
set(1)
```




    true



#### Set Implementations

##### Immutable


```Scala
import scala.collection.immutable

immutable.BitSet()
immutable.HashSet[AnyVal]()
immutable.ListSet[AnyVal]()
immutable.TreeSet[Int]()
immutable.SortedSet[Int]()
```




    TreeSet()



##### Mutable


```Scala
import scala.collection.mutable

mutable.BitSet()
mutable.HashSet[AnyVal]()
mutable.LinkedHashSet[AnyVal]()
mutable.TreeSet[Int]()
```




    TreeSet()



### Vector

Collection with acceptable performance in access and update.


```Scala
val v = Vector(1, 2, 3, 4)
```




    [[1, 2, 3, 4]]




```Scala
v :+ 5 :+ 6
```




    [[1, 2, 3, 4, 5, 6]]




```Scala
v(1)
```




    2




```Scala
v updated(2, 10)
```




    [[1, 2, 10, 4]]




```Scala
0 +: v
```




    [[0, 1, 2, 3, 4]]



### Stack

LIFO


```Scala
val s = scala.collection.immutable.Stack[Int](1, 2, 3, 4)
```




    [[1, 2, 3, 4]]




```Scala
s push(29) push(98)
```




    [[98, 29, 1, 2, 3, 4]]




```Scala
s top
```




    1




```Scala
s pop // Remove the first element from the stack
```




    [[2, 3, 4]]



### Queue

FIFO


```Scala
val q = scala.collection.immutable.Queue[Int](1, 2, 3, 4)
```




    [[1, 2, 3, 4]]




```Scala
q enqueue(98) enqueue(76)
```




    [[1, 2, 3, 4, 98, 76]]




```Scala
q dequeue
```




    (1,Queue(2, 3, 4))



### Range


```Scala
1 to 10
```




    [[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]]




```Scala
1 until 10
```




    [[1, 2, 3, 4, 5, 6, 7, 8, 9]]




```Scala
0 to 100 by 5
```




    [[0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60, 65, 70, 75, 80, 85, 90, 95, 100]]



### Streams 

Lazy List, only the first occurrence is evaluated


```Scala
val s = 1 #:: 2 #:: 3 #:: Stream.empty
```




    [[1, 2, 3]]




```Scala
Stream(1, 2, 3)
```




    [[1, 2, 3]]




```Scala
def fibonacci(a: Int, b: Int): Stream[Int] = a #:: fibonacci(b, a + b)
fibonacci(0, 1).take(10).force
```




    [[0, 1, 1, 2, 3, 5, 8, 13, 21, 34]]



## Collections in detail

<img src="https://docs.scala-lang.org/resources/images/tour/collections-mutable-diagram.svg">

### Traversable

Traversables collections implement `foreach`, which allows the collection to be browsed by calling a function.


```Scala
'a' to 'z' foreach print
```

    abcdefghijklmnopqrstuvwxyz

### Iterable

Crossover collections implement `iterator`, which allows access to each element without modification.


```Scala
val ite = ('a' to 'z').iterator
while (ite.hasNext) print(ite.next)
```

    abcdefghijklmnopqrstuvwxyz




    null



### Seq

The Seq collections are ordered.


```Scala
val s = ('a' to 'z')
```




    [[a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z]]




```Scala
s(scala.util.Random.nextInt(25))
```




    q




```Scala
s.segmentLength(v => (v < 'd'), 1) // Length of the longest sequence according to a predicate and an index
```




    2




```Scala
s.prefixLength(v => (v < 'd')) // Length of the longest sequence according to a predicate from index 0
```




    3




```Scala
s.indexWhere(v => "hello world" contains v.toString) // first indice according to a predicate
```




    3




```Scala
s.lastIndexWhere(v => "hello world" contains v.toString) // last indice according to a predicate
```




    22




```Scala
s.indexOf('z')
```




    25




```Scala
s.startsWith(Seq('a', 'b'))
```




    true




```Scala
s.endsWith(Seq('y', 'z'))
```




    true




```Scala
s.reverse
```




    [[z, y, x, w, v, u, t, s, r, q, p, o, n, m, l, k, j, i, h, g, f, e, d, c, b, a]]




```Scala
s.indexOfSlice(Seq('k', 'l'))
```




    10



### Usual operations

#### Add / remove an element

| Operation                                     	| Description                                               	| Collection            	|
|-----------------------------------------------	|-----------------------------------------------------------	|-----------------------	|
| c + e ; c + (e1,..,en)	                          	| Add elements, return a new collection.  	| Map, Set              	|
| c += e ; c += (e1,..,en) ; c -= e ; c -= (e1,..,en) 	| Adds and removes elements by modifying the collection. 	| Mutable               	|
| c - e ; c - (e1,..,en)                          	| Retire des éléments, retourne une nouvelle collection.    	| ArrayBuffer, Map, Set 	|
| c :+ e ; e +: e                                 	| Remove items, return a new collection.                	| Seq                   	|
| e :: c                                        	| Add an element at the beginning.                             	| List                  	|
| e #:: c                                       	| Add an element at the beginning.                             	| Stream                	|

#### Update

| Operation               	| Description                                                 	| Collection               	|
|-------------------------	|-------------------------------------------------------------	|--------------------------	|
| c(k) = e ; c.update(k, e)	 	| Updates the item in the indexed collection k.              	| mutable.Map, mutable.Seq 	|
| c.updated(k, e)         	| New collection in which the element is updated. 	| Sauf Set.                	|

#### Assemblist operations

| Opération                 	| Description                       	| Collection            	|
|---------------------------	|-----------------------------------	|-----------------------	|
| c ++ c2                   	| Union.                            	| Iterable              	|
| c - c2                    	| c without the elements of c2           	| ArrayBuffer, Map, Set 	|
| c2 ++=: c                 	| Add c2 at the top of c           	| ArrayBuffer           	|
| c ++= c2 ; c -= c2        	| Rajoute c2 à c ou enlève c2 à c   	| Mutable               	|
| c diff c2                 	| Add c2 to c or remove c2 to c           	| Seq                   	|
| c ::: c2                  	| Union                             	| List                  	|
| c \| c2 ; c & c2 ; c &~ c2 	| Union, Intersection et Difference 	| Set                   	|

#### Cast


```Scala
Seq(1).toArray
Seq(1).toBuffer
Seq(1).toList
Seq((1, 2)).toMap
Seq(1).toStream
Seq(1).toString
Seq(1).toVector

Seq(1).toTraversable
Seq(1).toIndexedSeq
Seq(1).toIterable
Set(1).toSeq
Seq(1).toSet
```




    Set(1)




```Scala
val collec = 1 to 100 by 8
collec.to[List] // de manière générale
```




    [[1, 9, 17, 25, 33, 41, 49, 57, 65, 73, 81, 89, 97]]



#### Operations of Iterables


```Scala
val collec = (1 to 100 by 6) ++ Seq(4)
```




    [[1, 7, 13, 19, 25, 31, 37, 43, 49, 55, 61, 67, 73, 79, 85, 91, 97, 4]]




```Scala
collec.size
```




    18




```Scala
collec.count(_%2 == 0)
```




    1




```Scala
collec.isEmpty
```




    false




```Scala
collec.nonEmpty
```




    true




```Scala
collec.sameElements(collec)
```




    true




```Scala
collec.forall(_ > 0)
```




    true




```Scala
collec.exists(_ < 0)
```




    false




```Scala
collec.sum
```




    837




```Scala
collec.product
```




    -320583804




```Scala
collec.min
```




    1




```Scala
collec.max
```




    97



#### Selection and cutting


```Scala
val collec = (1 to 100 by 6) ++ Seq(4)
```




    [[1, 7, 13, 19, 25, 31, 37, 43, 49, 55, 61, 67, 73, 79, 85, 91, 97, 4]]




```Scala
collec.head
```




    1




```Scala
collec.last
```




    4




```Scala
collec.tail
```




    [[7, 13, 19, 25, 31, 37, 43, 49, 55, 61, 67, 73, 79, 85, 91, 97, 4]]




```Scala
collec.init
```




    [[1, 7, 13, 19, 25, 31, 37, 43, 49, 55, 61, 67, 73, 79, 85, 91, 97]]




```Scala
collec.take(5)
```




    [[1, 7, 13, 19, 25]]




```Scala
collec.drop(5)
```




    [[31, 37, 43, 49, 55, 61, 67, 73, 79, 85, 91, 97, 4]]




```Scala
collec.splitAt(5)
```




    (Vector(1, 7, 13, 19, 25),Vector(31, 37, 43, 49, 55, 61, 67, 73, 79, 85, 91, 97, 4))




```Scala
collec.takeRight(5)
```




    [[79, 85, 91, 97, 4]]




```Scala
collec.dropRight(5)
```




    [[1, 7, 13, 19, 25, 31, 37, 43, 49, 55, 61, 67, 73]]




```Scala
collec.takeWhile(_ < 30)
```




    [[1, 7, 13, 19, 25]]




```Scala
collec.dropWhile(_ < 30)
```




    [[31, 37, 43, 49, 55, 61, 67, 73, 79, 85, 91, 97, 4]]




```Scala
collec.span(_ < 30)
```




    (Vector(1, 7, 13, 19, 25),Vector(31, 37, 43, 49, 55, 61, 67, 73, 79, 85, 91, 97, 4))




```Scala
collec.filter(_ % 2 == 0)
```




    [[4]]




```Scala
collec.filterNot(_ % 2 == 0)
```




    [[1, 7, 13, 19, 25, 31, 37, 43, 49, 55, 61, 67, 73, 79, 85, 91, 97]]




```Scala
collec.partition(_ % 2 == 0)
```




    (Vector(4),Vector(1, 7, 13, 19, 25, 31, 37, 43, 49, 55, 61, 67, 73, 79, 85, 91, 97))




```Scala
collec.slice(3, 7)
```




    [[19, 25, 31, 37]]




```Scala
collec.mkString(";")
```




    1;7;13;19;25;31;37;43;49;55;61;67;73;79;85;91;97;4




```Scala
collec.mkString("[", ",", "]")
```




    [1,7,13,19,25,31,37,43,49,55,61,67,73,79,85,91,97,4]



#### Transformation of a collection

##### map, flatMap


```Scala
def range(n: Int) = 0 to n
```




    range: (n: Int)scala.collection.immutable.Range.Inclusive





```Scala
Seq(1, 2, 3, 4).map(range)
```




    [[Range(0, 1), Range(0, 1, 2), Range(0, 1, 2, 3), Range(0, 1, 2, 3, 4)]]




```Scala
Seq(1, 2, 3, 4).flatMap(range) // merges collections
```




    [[0, 1, 0, 1, 2, 0, 1, 2, 3, 0, 1, 2, 3, 4]]



##### reduceLeft, reduceRight


```Scala
(1 to 5).reduceLeft(_-_)
```




    -13




```Scala
(1 to 5).reduceRight(_-_)
```




    3



##### foldRight, foldLeft

Same thing as reduction but with an initial element.


```Scala
((1 to 4) ++ (1 to 6)).foldLeft(Set[Int]())(_+_)
```




    Set(5, 1, 6, 2, 3, 4)




```Scala
// number of occurrences
Seq(1, 2, 1, 1, 7, 7, 2, 9).foldLeft(Map[Int, Int]()) ((counter, e) => counter + (e -> (counter.getOrElse(e, 0) + 1)))
```



##### scanLeft, scanRight

Same as fold by saving the intermediate results in a collection


```Scala
Seq(1, 2, 4, 1, 3, 4).scanLeft(Set[Int]()) ((s, e) => s + e)
```




    [[Set(), Set(1), Set(1, 2), Set(1, 2, 4), Set(1, 2, 4), Set(1, 2, 4, 3), Set(1, 2, 4, 3)]]



##### zip, zipAll, zipWithIndex, unzip


```Scala
"abcde" zip 1.to(5)
```




    [[(a,1), (b,2), (c,3), (d,4), (e,5)]]




```Scala
"abcde".zipAll(1.to(2), "*", -1) // valeur par défaut à gauche et à droite
```




    [[(a,1), (b,2), (c,-1), (d,-1), (e,-1)]]




```Scala
"abcde" zipWithIndex
```




    [[(a,0), (b,1), (c,2), (d,3), (e,4)]]




```Scala
Seq((1, 2), (3, 4), (5, 6)) unzip
```




    (List(1, 3, 5),List(2, 4, 6))




```Scala

```
