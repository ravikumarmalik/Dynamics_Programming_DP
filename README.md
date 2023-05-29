# Dynamics_Programming_DP

DP is an optimization recursion.
Wherever we see a recursive solution that has repeated calls for same inputs, we can optimize it using Dynamic Programming.
The idea is to simply store the results of subproblems, so that we do not have to re-compute them when needed later.
This simple optimization reduces time complexities from exponential O(2^n) to polynomial O(n).

# How to identify DP?
i. Optimal Problem (Best Solution)

ii. Some choice is given (we can see multiple branches in recursion).

# Ways to DP
i. Memoization(Top down)

ii. Tabulation(Buttom-UP)


EX - 

With recursion:-
=================
public class Dp{

public static int fib(int n){

if (n == 0 || n == 1){ - O(2^n)

return n;

}

return f(n-1) + f(n-2);

}

public static void main(String[] str){

int n=5;

System.out.println(fib(n)); - 5

}

}

With dp:-
=================

public class Dp{

public static int fib(int n, int f[]){

if (n == 0 || n == 1){ O(n)

return n;

}

return f(n-1, f) + f(n-2, f);

}

public static void main(String[] str){

int f[] = new int [n+1];

int n=5;

System.out.println(fib(n,f)); - 5

}

}




