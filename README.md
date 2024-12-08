# CALCULATE-POWER
public class CalcularePow {
    public CalcularePow() {
    }

    public static int calculatepow(int x, int n) {
        if (n == 0) {
            return 1;
        } else if (x == 0) {
            return 0;
        } else {
            int Pow1 = calculatepow(x, n - 1);
            int Pow2 = n * Pow1;
            return Pow2;
        }
    }

    public static void main(String[] args) {
        int n = 5;
        int x = 2;
        int ans = calculatepow(n, x);
        System.out.println(ans);
    }
}
