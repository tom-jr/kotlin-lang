# Collections

List, Set, Map
List: lista ordenadas que pode ter repetidos registros (Mutável ou imutável)

## List
```kotlin
fun main() {
    val myArray: List<String> = listOf("Luffy", "Sanji", "Nami") //imutável
    val myArrayMutable: MutableList<String> = mutableListOf("Nami", "Zoro", "Nico robe", "Chopper", "Zoro") //mutável

    val castArray: List<String> = myArrayMutable //cast lista mutável para imutável
    println(myArrayMutable)

    println(myArrayMutable.count()) // size do array
    println("contem Zoro ? ${"Zoro" in myArrayMutable}") //search in the array
    println(myArrayMutable[2]) // by indexArray
    println("Fist item from mutable array is ${myArrayMutable.first()} \nLast item from mutable list is ${myArrayMutable.last()}") // funcs last,first
    myArrayMutable.add("Buggy") //func add
    println(myArrayMutable)
    myArrayMutable.remove("Zoro") //func remove
    println(myArrayMutable)
}
```
## Set
Lista não ordenadas de itens de um mesmo tipo sem repetições
```kotlin
fun main() {
    val mySet: Set<String> = setOf("Nami", "Nico Robe", "Sakura")
    val mySetM: MutableSet<String> = mutableSetOf("Nami", "Nico Robe", "Sakura", "Nami", "Nico Robe", "Sakura")

    println(mySetM)
    mySetM.add("Ten Ten") //func add
    println(mySetM)
    mySetM.remove("Sakura") //func remove
    println(mySetM)


    println("Nico is in mySetM ? ${"Nico Robe" in mySetM}") //search func 

}
```

## Map
coleção de chave e valor com valores unicos

```kotlin
fun main() {
val myMap: Map<Int, String> = mapOf(1 to "Mokey D Ruffy", 2 to "Zoro", 3 to "Nami", 4 to "Ussop")
val myMapM: MutableMap<Int, String> = mutableMapOf(1 to "Mokey D Ruffy", 2 to "Zoro", 3 to "Nami", 4 to "Ussop", 5 to "Sanj", 6 to "Chopper")

println(myMapM)
println(myMapM[2]) // search by the key, returns key's value
println(myMapM.count()) // size of key's pair items
myMapM.put(7 , "Nico Robe")
println(myMapM) // func adiona novo par
myMapM.remove(1) // func remove by the key
println(myMapM)
println("contains key 2? ${myMapM.containsKey(2)}");
println(myMapM.values) // returns only values
println(myMapM.keys) //returns only keys
println(3 in myMapM.keys)
println("Nami" in myMapM.values)
}
```
