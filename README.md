# Finai_contor_1 - имя репозитория
 Создадим файл C#

## Текст задачи

*Задача*. Написать программу, которая из имеюшегося массива строк формирует массив из строк,
длина которых меньше либо равна 3 символа. Первоначальный массив можно ввести с клавиатуры,
либо задать на старте выполнение алгоритма. При решении не рекомендуется пользоваться 
коллекциями, лучше обойтись исключительно массивами.

![Блок-схема](blok_shema.jpg)

[Блок схема](https://dropmefiles.com/WFdDn)

``` c#
Console.WriteLine("Введите длинну массива ");
int size = Convert.ToInt32(Console.ReadLine());
string[]? array = new string[size];
Console.WriteLine("Введите слова масива");
for (int i = 0; i < size; i++)
{
    array[i] = Console.ReadLine();

}
bool tmp = false;
Console.WriteLine("Результат: ");
for (int i = 0; i < array.Length; i++)
{
    if (array[i].Length < 3) 
        {
            Console.WriteLine(array[i]);
            tmp = true;
        }
    
}
if (tmp == false)   Console.WriteLine("Все слова больше трёх символов=) ");
```