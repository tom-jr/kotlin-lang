# Basic Types
Caso não declarar o tipo da variável em kotlin sera necessário atribuir seu valor na declaração para que
o Kotlin infira automaticamente o type da variável.

Para declara em outro momento, podemos declarar a variável com o tipo e atribuir um valor depois.

```kotlin
fun main () {
    val name: String;
    name = "Tom";
    
    println("my name is $name");
}
```

## Tipos de variáveis em Kotlin
<div class="table__wrapper table__wrapper--wide table__wrapper--without-scroll"><table class="table__content table__content--wide" id="d8783548"><thead class="table__thead"><tr class="table__tr" id="90c9d824"><th class="table__th" id="667565b9"><p class="article__p"><b id="8c7b22cb" class="article__b">Category</b></p></th><th class="table__th" id="16a80615"><p class="article__p"><b id="e8507119" class="article__b">Basic types</b></p></th></tr></thead><tbody class="table__tbody"><tr class="table__tr" id="2a143c38"><td class="table__td" id="2f6fcf30"><p class="article__p child">Integers</p></td><td class="table__td" id="11729d7d"><p class="article__p child"><code class="code ">Byte</code>, <code class="code ">Short</code>, <code class="code ">Int</code>, <code class="code ">Long</code></p></td></tr><tr class="table__tr" id="27881322"><td class="table__td" id="713bc52f"><p class="article__p child">Unsigned integers</p></td><td class="table__td" id="4e9542af"><p class="article__p child"><code class="code ">UByte</code>, <code class="code ">UShort</code>, <code class="code ">UInt</code>, <code class="code ">ULong</code></p></td></tr><tr class="table__tr" id="70d72084"><td class="table__td" id="1a089878"><p class="article__p child">Floating-point numbers</p></td><td class="table__td" id="602b9141"><p class="article__p child"><code class="code ">Float</code>, <code class="code ">Double</code></p></td></tr><tr class="table__tr" id="822bb1a"><td class="table__td" id="289d203b"><p class="article__p child">Booleans</p></td><td class="table__td" id="3ec31814"><p class="article__p child"><code class="code ">Boolean</code></p></td></tr><tr class="table__tr" id="fdb43130"><td class="table__td" id="fe3b3a89"><p class="article__p child">Characters</p></td><td class="table__td" id="60bf13c1"><p class="article__p child"><code class="code ">Char</code></p></td></tr><tr class="table__tr" id="4343279b"><td class="table__td" id="51d930c0"><p class="article__p child">Strings</p></td><td class="table__td" id="fa337bb1"><p class="article__p child"><code class="code ">String</code></p></td></tr></tbody></table></div>

```kotlin
fun main() {
    val a: Int = 1000
    val b: String = "log message"
    val c: Double = 3.14
    val d: Long = 100_000_000_000_000
    val e: Boolean = false
    val f: Char = '\n'
}
```

