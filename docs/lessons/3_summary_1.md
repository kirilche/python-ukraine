---
tags:
  - Прості Типи
  - Рядки
---

# Уроки 1 та 2, підсумки.

## Ціль

Повторити та **система**тизувати знання, про які йдеться в початкових уроках.

## Засоби

Довідкова література, google, stackoverflow

## Перша програма

- Перша програма пишеться для того, щоб перевірити процес запуску коду на виконання
- Сам код першої програми роблять максимально простим
- Пайтон — чи не єдина мова, у якої найпростіша програма займає 1 простий рядок

## Функція print()

`print()` це функція яка виводить на екран те, що ми помістимо в круглі дужки.  
Наприклад:

- числовий літерал `5` або `123_456_789_000` або `3.14159265359`
- рядковий літерал `"Ukraine"`, `'Вистоїмо'` `"2025р"`
- числова змінна `e = 2,71828`
- рядкова змінна `s = "My name is "`
- будь–яка кількість цих або інших типів через кому `,`
- нічого
- f–рядок, спеціальний шаблон, що містить змінні або вирази `f"Два в степені 7 буде {2**7}"`

## f–рядок

Спеціальний тип рядків — f–рядок використовується, щоб поєднувати відомі та невідомі (змінні) значення.
Невідомі значення можуть бути отримані з різних джерел:

- від ОС (Операційної Системи),
- від користувача,
- від генератора випадкових чисел,
- з БД (Бази Даних) тощо  

???+ tip "Константи"
    Окремим випадком невідомих значень є константи. Константи вводять для того, щоб не міняти багато рядків коду.  
    Якщо наприклад зміниться параметр, який міняється доволі рідко.

## Змінні та присвоєння

- Пайтон робить процес створення змінних простим
- [Декларація та Визначення](2.md#declare-vs-definition) — терміни які треба знати
- Перший значить — заявити змінну (declare)
- Другий значить — надати значення (define)
- В мові Пайтон декларація відбувається в момент визначення (неявно)
- Тобто коли ви присвоюєте перше значення в цей самий момент змінна і виникає
- ==Присвоєння== — це коли ліворуч пишеться ==ім'я змінної==, потім знак `=` а за ним праворуч ==вираз або літерал==, значення, яке ми запишемо у змінну.

## input()

- Функція `input()` друкує запрошення до вводу та зчитує рядок з клавіатури. Завершенням вводу є ++enter++
- `input()` повертає рядок, а значить
    1. ліворуч від `input()` має стояти якась змінна та `=`
    2. `input()` має бути в дужках іншої функції, бути параметром

## int()

- `int()` в дужках (на вході) може мати рядок, що схожий на ціле число `-123` або `1_000_000`
- `int()` може викликати помилку або повернути ціле число, а значить
    1. ліворуч від `int()` має стояти якась змінна та `=`
    2. `int()` має бути в дужках іншої функції, бути параметром

## Композиція функцій

=== "Без композиції"
    ```py title="Трішки простіше, але не так математично" linenums="1"
    age_str = input("Введіть свій вік: ")
    age_int = int(age_str)
    ```
=== "Використання композиції"
    ```py title="Компактно та елегантно" linenums="1"
    # int() — зовнішня функція input() — внутрішня  
    age = int(input("Введіть свій вік: "))
    ```

Ці 2 програми абсолютно ідентичні за ефектом, але виглядають трішки по–різному
