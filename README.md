# LoginUI-Android
 ```
1 - Məqsəd Burada Vievdakı  dataları  tutmaq və bu  sayədə Vievdaki dataları hər səfərində yeniden yaradamq yerinə içindəki dataları təkrar istifadə oluna biləcək hala gətirməkdir

```
```
2 -
    fun trycatch() {
        try {
            // some code that might throw an exception
        } catch (e: Exception) {
            // handle the exception here
        } finally {
            // optional finally block
        }
    }
```
```
3 - 
interface Component {
    fun operation(): String
}

class ConcreteComponent : Component {
    override fun operation() = "concrete "
}

abstract class Decorator(private val component: Component) : Component {
    override fun operation() = component.operation()
}

class ConcreteDecoratorFirst(component: Component) : Decorator(component) {
    override fun operation() = "${super.operation()} + concrete First "
}

class ConcreteDecoratorLast(component: Component) : Decorator(component) {
    override fun operation() = "${super.operation()} +  Last compnent "
}
```

```
4 -
fun main()
{
    val array = arrayOf(1, 2, 3, 1, 2)
    val uniqueArray = array.distinct()
    println(uniqueArray) // Output: [1, 2, 3]

}
```
```
5 - 
fun main(args: Array<String>) {
    val e: String? = "Salam"
    e?.let {
        println("Sagol")
    }
}
```

 7-  Object 
```
8   -  Sinif cagrildigi zaman ise  dusen  ilk method 
  a - class test(var a: Int )
    {}
  b - class test () {
      constructor(a: Int, b:Int)
  }
```

```
9 - 
bu battern alt class lar ozleri yeni  bir Obyekt  Yaradmaga imakan verir 
10 - 
interface Create {
    fun createType ()
}

class Kottec : Create {
    override fun createType() {
        println("Drawing Circle")
    }
}

class Villa : Create {
    override fun createType() {
        println("Drawing Square")
    }
}

class GenerateFactory  {
    fun getShape(type: String): Create? {
        return when (type) {
            "Circle" -> Kottec()
            "Square" -> Villa()
            else -> null
        }
    }
}
 ```

11 -  LiveData  datalarda deyisiklik oldugunda  update olunur ozu  numune desek meselen api den gelen deyerlerde eger ki deyiskilik olsa bu zaman onnan referans alan her yer de ki datalar deyisilib yeni gelen deterleri qebul edecek  
```
14  -  Singleton pattern - Static classlara yaranir 
object  Com {
}
15 - 

data class Home(var rooms: Int, var roof: String , var color : String  ) {
    class Builder() {
        var room = 0;
        var roofBuild : String = " ";
        var color   : String  = " ";
        fun setRooms(roomCount: Int): Builder {
            this.room= roomCount
            return this
        }

        fun setRoof(roof  : String): Builder {
            this.roofBuild = roof
            return this
        }
        
        fun build(): Home {
             return Home(room, roofBuild ,  color)
        }
    }
}
```


```
13 - fun maxNUm(array: IntArray): Int {
    array.sortDescending()
    return array[0] * array[1]
}
```
12 - MOdel - view Presenter 

6 - Liskov 



