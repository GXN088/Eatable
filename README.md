# Eatable
Имплементируй интерфейс Eatable только для классов, объекты которых могут быть съедобными, из этого списка:
Apple — яблоко
Carrot — морковь
Fire — огонь
Fish — рыба
Stone — камень


Псевдокод для задачи "Съедобное — несъедобное":

```
// Интерфейс Eatable - маркерный интерфейс для съедобных объектов
interface Eatable {
    // Пустой интерфейс, служит только для маркировки
}

// Класс Apple - съедобный
class Apple implements Eatable {
    // Реализация Apple
}

// Класс Carrot - съедобный
class Carrot implements Eatable {
    // Реализация Carrot
}

// Класс Fish - съедобный
class Fish implements Eatable {
    // Реализация Fish
}

// Класс Fire - несъедобный (не implements Eatable)
class Fire {
    // Реализация Fire
}

// Класс Stone - несъедобный (не implements Eatable)
class Stone {
    // Реализация Stone
}
```

Ключевые моменты:

· Интерфейс Eatable используется как маркер (пустой интерфейс)
· Классы Apple, Carrot, Fish помечены как съедобные через implements Eatable
· Классы Fire и Stone не реализуют интерфейс Eatable, поэтому считаются несъедобными
· Такая структура позволяет в дальнейшем проверять объекты на съедобность через instanceof Eatable
