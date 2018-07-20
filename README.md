# FibonacciRecursiveAlgorithm

 static void Main(string[] args)
        {
            Console.WriteLine("enter the number of terms: ");
            int n = Convert.ToInt32(Console.ReadLine());

            Console.WriteLine("Fibonacci series:");
            for (int i = 1; i <= n; i++)
            {
                int result = Fibo(i);
                Console.Write(result + " ");

            }
            Console.ReadKey();
        }
        
        public static int Fibo(int n)
        {
            if (n < 2)
            {
                return n;
            }

            else
            {
                return Fibo(n - 1) + Fibo(n - 2);
            }

        }
