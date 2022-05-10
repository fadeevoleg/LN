# LN (Длинная арифметика) #

Программа, позволяющая выполнять арифметические операции над целыми числами произвольной точности в десятичной системе. 

Входной файл должен содержать выражение в обратной польской записи, каждое число и знак операции располагаются на отдельной строке. 

Выходной файл содержит состояние стека на момент завершения программы.


## Струтура проекта: ##

### LN - класс, выполняющий арифметические операции: 
  * сложение ('+') 
  * вычитание ('-')
  * умножение ('*')
  * деление ('/')
  * остаток от деления ('%')
  * квадратный корень ('~')
  * унарный минус ('_')

**операции сравнения**:

  * меньше, меньше или равно ('<', '<=')
  * больше, больше или равно ('>', '>=')
  * равно, неравно ('==', '!=') 
  
**Конструкторы класса:**
* конструктор копирования,
* конструктор перемещения,
* из long long со значением по умолчанию: 0,
* из строки символов C (const char \*),
* из строки std::string\_view.

**Также реализованы операции:**
* присваивания
* перемещения
* преобразования типа в: long long (с генерацией исключения в случае, когда значение не умещается), bool (неравенство нулю);
* создания из литерала произвольной длины с суффиксом \_ln (пример: LN x; x = 123\_ln;).
### MyVector - аналог <std::vector> на С++ ###
