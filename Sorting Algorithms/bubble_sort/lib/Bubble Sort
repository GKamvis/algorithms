/*
Time Complexity-si O(n^2)
Space Complexity O(1)
çoxda faydalı deyil amma asandı deyə istifadə olunur, çoxda böyük olmayan -
 sıralamalardada istifadə oluna bilər.
 Rekursivdə yazila bilər amma yenədə effektivliyi dəyişməz.

 işləmə ardıcılığı belədir -->
 listə sıra ilə hər dəfə 2 element götürür (j və j+1 indeksli) yoxlama aparır 
 list[j] > list[j + 1]  doğrudursa şərt yerlərini dəyişir və dövr davam edir ..

(asc desc biz hansi sira ilə yoxlayiriqsa  list[j] > list[j + 1]: artan , list[j] < list[j + 1]: azalan sıra ilə düzür ) 
 hər halda  ilk dövrdə  uyğun olaraq ya ən böyüy ya ən kiçiyi ən sona köçürür.Texniki olaraq ən sondakı elemetlərri birinci dövrdən sonra yoxlamaq lazim deyil
 buna görədə biz ikinci for dövründə j < n - 1 - i  şərti daxilində yoxlama aparırıq,yəni n-1 listin max indeksini təyin edəcək 
(n - 1 )- i  buradada i dəyəri ona görə çıxılırkı onsuzda hər dəfə i vahid dövr iterasiya etdikdə ən sona ən (böyük / kiçik ) dəyəri köçürüb. Yoxlamaq lazim deyil.
*/

class BubbleSort {
  List? sort(List<int> list) {
    int n = list.length;
    bool swapped;

    for (int i = 0; i < n - 1; i++) {
      swapped = false;
      for (int j = 0; j < n - 1 - i; j++) {
        if (list[j] > list[j + 1]) {
          int temp = list[j + 1];
          list[j + 1] = list[j];
          list[j] = temp;
          swapped = true;
        }
      }
      if (swapped == false) break;
    }
    return list;
  }
}

void main() {
  BubbleSort BSort = BubbleSort();
  List<int> list = [1, 4, 2, 5, 0];
  print(BSort.sort(list));
}
