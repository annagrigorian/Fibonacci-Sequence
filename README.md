## Fibonacci-Sequence

Program gets Fibonacci Sequnce of specific count of elements
using a function named Fibonacci which has the following signature

~~~csharp
static IEnumerable<int> Fibonacci(int n)
~~~

Specify the range of the sequence you can by giving an integer argument to the function.
~~~csharp
var sequence = Fibonacci(8);
foreach (var item in sequence)
{
    Console.Write(item + "  ");
}
~~~

The output is as follows
~~~csharp
1  1  2  3  5  8  13  21
~~~

Getting the sequence you can manipulate with it (e.g. selecting odd numbers).
sdk
~~~csharp
var subsequence = from c in sequence
                  where c % 2 == 1
                  select c;
~~~

We have the following output
~~~csharp
1  1  3  5  13  21
~~~

You can find more information about Fibonacci sequence and it's usages [here](https://www.mathsisfun.com/numbers/fibonacci-sequence.html)
 
