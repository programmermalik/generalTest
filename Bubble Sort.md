# Bubble Sort
int Min = 0;
            int Max = 1000;
            
            int[] bubble = new int[15]; 
            
            int L = bubble.Length;
            
            Random randNum = new Random();
            for (int i = 0; i < L; i++)
            {
                bubble[i] = randNum.Next(Min, Max);
            }
            
            for(int A = L-1; L > 0; L--){
                for(int B = 0; B < A; B++){
            
                    if(bubble[B] > bubble[B + 1]){
                        
                int temp;
                        
                temp = bubble[B];
                bubble[B] = bubble[B + 1];                      
                bubble[B + 1] = temp;
                
                    }
            
                }
            }
            
            /*
            Büyükten Küçüğe Yapacak İsek
            
            /////Array.Reverse(bubble);\\\\\
            
            Komutunu Kullanacağız.
            
            */
            
            foreach(var item in bubble){
            
                Console.WriteLine(item);
                
            }
