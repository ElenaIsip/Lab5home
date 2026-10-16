#Домашняя работа Попова Елена бТИИ-262
# Задание для работы
# Написать программу вычисления значения функции двух переменных. Результат проверить на контрольном примере.
#<img width="859" height="82" alt="{087FD1FE-51B7-4F24-91C6-BC0B69B720EC}" src="https://github.com/user-attachments/assets/30cdc246-4238-426f-bfd4-9dc38e42613d" />
#Блок схема программы
<img width="370" height="525" alt="{D64F7444-AF0C-4C10-B191-B64B9232B955}" src="https://github.com/user-attachments/assets/faccbd0e-d2bd-497c-b091-08218382947b" />



#Реализация программы 
#define _USE_MATH_DEFINES
#include <stdio.h>
#include <locale.h>
#include <math.h>

int main(void)
{
    setlocale(LC_ALL, "RUS");

    double x, y, F;

   
    x = 1.9;
    y = -1.0;
    F = 2.33 * log(sqrt(1.0 + cos(x) * cos(x)))
        / (exp(y) + sin(x) * sin(x));
    printf("F(%.2f, %.2f) = %.6f\n", x, y, F);

   
    x = 1.6;
    y = -2.3e-6;
    F = 2.33 * log(sqrt(1.0 + cos(x) * cos(x)))
        / (exp(y) + sin(x) * sin(x));
    printf("F(%.2f, %.1e) = %.6e\n", x, y, F);

    return 0;
}
