# C# Dizi Uygulaması
C# ile 0-9 arasında rastgele 100 elemanlı bir dizi oluşur ve dizide bulunan elemanların kaç kere tekrarlandığını yazdır.

            int[] dizi = new int[100];
            Random rnd = new Random();
            for (int i = 0; i < 100; i++)
            {
                dizi[i] = rnd.Next(maxValue:10) ;

            }

            foreach (var sayi in dizi)
            {
                Console.WriteLine(sayi);
            }

            int[] adet = new int[10];
            for (int i = 0; i < 100; i++)
            {
                adet[dizi[i]]++;
            }

            for (int i = 0; i < adet.Length; i++)
            {
                Console.WriteLine(i + $"rakamından dizi içerisinde {0} adet bulunmaktadır", adet[i]); 

            }
