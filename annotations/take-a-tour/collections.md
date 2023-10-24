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
