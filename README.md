# dynamic_programming
* A general walk through in understanding dynamic programming in general.

### What is Dynamic programming.
* Dynamic Programming is mainly an optimization over plain recursion.
  Wherever we see a recursive solution that has repeated calls for same
  inputs, we can optimize it using Dynamic Programming. The idea is to
  simply store the results of subproblems, so that we do not have to re-compute
  them when needed later.
  * an example:
  ~~~
  --> Fibonacci Numbers

  int fib(int n)

    if (n <= 1)
        return n;
    else
        return fib(n - 1) + fib(n - 2); --> building it recursively

    --> building it in a more Dynamic way (linear)

    f[0] = 0;
    f[1] = 1;

    for (i = 2; i <= n; i++)

        f[i] = f[i - 1] + f[i - 2];

    reurn f[n];
  ~~~
