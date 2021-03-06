# complex@0.0.1

### Задание
Написать программу, выполняющую арифмитические операции и функции ввода/вывода над комплексными числами. Программа должна содержать следующую структуру:
```
struct complex_t {
  float real;
  float imag;
  
  complex_t();
  
  complex_t add( complex_t other ) const;
  complex_t sub( complex_t other ) const;
  complex_t mul( complex_t other ) const;
  complex_t div( complex_t other ) const;
  
  std::istream & read( std::istream & stream );
  std::ostream & write( std::ostream & stream );
};
```

### Входные данные
Во входных данных заданы строки, следующего формата:
```
(r1, i1) op (r2, i2) 
```

### Выходные данные
Результат арифмитической операции или строка `An error has occured while reading input data`, сведетельствующая о возникновении ошибки ввода.

### Примеры
#### входные данные
```
(3, 4) + (1, 2)
```
#### выходные данные
```
(4, 6)
```
#### входные данные
```
(3, 4) - (1, 2)
```
#### выходные данные
```
(2, 2)
```
#### входные данные
```
(3, 4) * (1, 2)
```
#### выходные данные
```
(-5, 10)
```
#### входные данные
```
(3, 4) / (1, 2)
```
#### выходные данные
```
(2.2, -0.4)
```
#### входные данные
```
(3, 4) + (1, )
```
#### выходные данные
```
An error has occured while reading input data
```
