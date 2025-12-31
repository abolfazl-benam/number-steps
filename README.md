# مثلث اعداد تراز راست | Right-Aligned Number Triangle

یک برنامه ساده و آموزشی به زبان **C** که از کاربر یک عدد دریافت می‌کند و یک مثلث از اعداد را به صورت تراز راست چاپ می‌کند.

## پیش‌نمایش خروجی (برای n=6)
          1 
        1 2 
      1 2 3 
    1 2 3 4 
  1 2 3 4 5 
1 2 3 4 5 6

## نحوه کامپایل و اجرا
gcc main.c -o triangle
./triangle
سپس عدد دلخواه خود را وارد کنید.
مثال ورودی و خروجی

ورودی:
5
خروجی:
        1
      1 2 
    1 2 3 
  1 2 3 4 
1 2 3 4 5
## مناسب برای

- دانشجویان رشته کامپیوتر در ترم‌های اول
- تمرین حلقه‌های تودرتو (nested loops)
- یادگیری الگوهای چاپی (pattern printing)
- مصاحبه‌های برنامه‌نویسی مقدماتی

## تکنولوژی استفاده شده

- زبان برنامه‌نویسی C
- کامپایلر GCC


 English Version
# Right-Aligned Number Triangle
A simple and educational C program that takes an integer input from the user and prints a right-aligned triangle of numbers.
## Output Preview (for n=6)
          1 
        1 2 
      1 2 3 
    1 2 3 4 
  1 2 3 4 5 
1 2 3 4 5 6
## Source Code (main.c)

#include <stdio.h>

int main()
{
    int n, i, j;
    scanf("%d", &n);
    
    for (i = 1; i <= n; i++)
    {
        for (j = 0; j < n - i; j++)
            printf("  ");
            
        for (j = 1; j <= i; j++)
            printf("%d ", j);
            
        printf("\n");
    }
    
    return 0;
}

## How to Compile and Run
gcc main.c -o triangle
./triangle

## Suitable For

- Beginner programming students
- Practicing nested loops
- Learning pattern printing problems
- Basic coding interviews

Made with ❤️ by [abolfazl-benam]