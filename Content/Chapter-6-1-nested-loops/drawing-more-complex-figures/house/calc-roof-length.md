#### Изчисляване дължината на покрива

За да начертаем **покрива**, записваме колко ще е началният брой **звезди** в променлива **`stars`**:
* Ако **`n`** е **четно** число, ще са 2 броя.
* Ако е **нечетно**, ще е 1 брой.

![](/assets/chapter-6-images/09.House-03.png)

Изчисляваме дължината на **покрива**. Тя е равна на половината от **`n`**. Резултата записваме в променливата **`roofLength`**.

![](/assets/chapter-6-images/09.House-04.png)

Важно е да се отбележи че, когато **`n`** е нечетно число, дължината на покрива е по-голяма с един ред от тази на **основата**. В езика **C#**, когато два целочислени типа се делят и има остатък, то резултата ще е числото без остатъка.

Пример:

```csharp
int result = 3 / 2; // резултат 1
```

Ако искаме да закръглим нагоре, трябва да използваме метода **`Math.Ceiling(…)`**:
**`int result = (int)Math.Ceiling(3 / 2f);`**
В този пример делението не е от 2 целочислени числа. "`f`" след число показва, че даденото число е от тип **`float`** (число с плаваща запетая). Резултатът от **`3 / 2f`** е **`1.5f`**. **`Math.Ceiling(…)`** закръгля делението нагоре. В нашият случай **`1.5f`** ще стане 2. **`(int)`** се използва, за да може да трансформираме типа обратно в **`int`**.
