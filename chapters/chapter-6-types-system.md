# Система типов

Для работы со значением *null* есть специальные инструменты:  
- Оператор безопасного вызова `?.`
- Оператор “Элвис” `?:`
- Утверждение, что значение не равно *null* - `!!`
- Функция `let`

Оператор `as?` позволяет привести значения к типу и обрабатывать случаи, когда оно имеет несовместимы тип

Типы, пришедшие из *Java*, интерпретируются в *Kotlin* как платформенные типы, что позволяет работать с ними как к типам с поддержкой и без поддержки *null*

Типы, представляющие обычные числа (например, `Int`), выглядят и функционируют как рядовые классы, но обычно компилируются в простые типы *Java*

Простые типы с поддержкой *null* (такие как `Int?`) соответствуют оберткам простых типов в *Java* (`Integer`)

Тип `Any` - это супертип всех других типов и аналог типа `Object` в *Java*. А тип `Unit` - аналог `void`

Тип `Nothing` используется в качестве типа возвращаемого значения для функций, которые обычном в режиме не завершаются

Для представления коллекций *Kotlin* использует стандартные классы *Java*, но делит их на доступные только для чтения и для чтения/записи.

При наследовании *Java*-классов и реализации *Java*-интерфейсов в *Kotlin* нужно обращать пристальное внимание на возможность изменения и допустимость значения *null*

Класс `Array` в *Kotlin* выглядит как обычный обобщенный класс, но компилируется в *Java*-массив

Массивы простых типов представлены специальными классами, такими как `IntArray`.
