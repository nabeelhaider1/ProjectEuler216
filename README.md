# ProjectEuler216
Project
import java.math.BigInteger;

public class e216 {
    public static void main (String[] args) {
        long n, t;
        int p = 0;

        for (n=2; n<=50000000; n++) {
           t = (2*n*n)-1;
           BigInteger bt = BigInteger.valueOf(t);
           if(bt.isProbablePrime(20))
              p++;
        }
        System.out.print(p);
    }
}
