# SORU 1 
# [16,21,11,8,12,22] -> Merge Sort
# Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.


# ÇÖZÜM :
    [16,21,11,8,12,22]
  [16,21,11] - [8,12,22]
 6 elemanlı olan sıramız ilk adımında 2 'ye bölünerek 3 elemanlı 2 dizeye ayrılmış oldu.
 
  [16,21]-[11] - [8,12]-[22]            
 3 elemanlı 2 dizemiz 2 ye bölünerek toplamda 4 dize olup, 2'si iki elemanlı ve diğer 2'si tek elemanlı şekilde kalmıştır.

  [16]-[21]-[11]-[8]-[12]-[22]         
  2 elemanlı olan iki dizemizde tekrar 2'ye bölünerek, tüm dizelerimizin tek elemanlı hale gelmesiyle bölünme sonlanmıştır.
  
  [16,21]-[11] - [8,12]-[22]          
  Birleşmeye başladığında ilk olarak son bölünme esnasındaki dizeyle kendi arasında başlar. Tek elemanlı dizeler tek olarak kalmış olur bu durumda.
  
  [11,16,21] - [8,12,22]                 
  Tek elemanlı dizemiz ile 2 elemanlı dizemiz kendi arasında sıralanarak, 2 adet 3 elemanlı dize şeklinde olmuştur.
  
  [8,11,12,16,21,22]                    
  Bu da dizemizin son birleşme halidir. Artık dizemiz küçükten büyüğe şeklinde sıralanmış haldedir.

  # SORU 2
  # Big-O gösterimini yazınız.

  # ÇÖZÜM :
  Her bölünme de logn şeklinde hareket edecektir.
  Birleşme esnasında ise her adımda birer kez birleşeceği için o(n) zamanını alır.
  Böylelikle algoritmamoz O(nlogn) şeklinde ifade edilmiş olur.
