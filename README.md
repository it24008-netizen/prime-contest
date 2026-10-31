# prime-contest
<img width="1763" height="811" alt="image" src="https://github.com/user-attachments/assets/8610405d-74a3-4290-b975-9826f9278aa4" />
## Prime checker##
~~~
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;
import java.lang.reflect.*;
import java.io.*;
import java.util.*;
import static java.lang.System.in;

class Prime {
    public void checkPrime(int... nums) {
        StringBuilder sb = new StringBuilder();
        for (int n : nums) {
            if (isPrime(n)) {
                sb.append(n).append(" ");
            }
        }
        System.out.println(sb.toString());
    }

    private boolean isPrime(int n) {
        if (n < 2) return false;
        for (int i = 2; (long) i * i <= n; i++) {
            if (n % i == 0) return false;
        }
        return true;
    }
}
public class Solution {
~~~
## java priliminary test##
~~~
import java.io.*;
import java.math.BigInteger;
import java.util.*;

public class Solution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        BigInteger n = new BigInteger(sc.nextLine().trim());
        System.out.println(n.isProbablePrime(100) ? "prime" : "not prime");
        sc.close();
    }
}
~~~



