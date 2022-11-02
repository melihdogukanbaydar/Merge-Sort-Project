# [16,21,11,8,12,22] -> Merge Sort

## 1. Yukaridaki Dizinin Merge Sort Türüne Göre Aşamalarını Yazınız
----------------
Başlangıçta dizimizi ikiye bölüyoruz. Bölünen dizileri tekrar bölüyoruz. Tek eleman kalana kadar devam ediyoruz.

Diziyi ikiye bölerek yeniden yazıyoruz.  [16,21,11,8,12,22]->

[16,21,11]  <-------------------------> [8,12,22] ->

Sol ve sağdaki diziyi  bir kez daha bölüyoruz.->

[16,21] <---> [11] <-------------------> [8,12] <---> [22]->

Tek eleman kalana kadar bir kez daha bölüyoruz.

[16] <-> [21] <-> [11] <-------------> [8] <-> [12] <-> [22]

İkili ikili sıralayarak birleştiriyoruz.->

[16,21] <--->[11] <---------------->  [8,12] <---> [22]

Tekrar ikili ikili sıralayrak birleştiriyoruz.->

[11,16,21] <----------------------------> [8,12,22]

Son sıralayarak birleştirmede dizimizi elde ediyoruz.

[8,11,12,16,21,22]

## 2. Big O Gösterimini yazınız
-----------------------

Recursive bir fonksiyon olduğu için sürekli kendini çağırarak diziyi hep ikiye bölmektedir. Her bölünmüş dizi elemanı için Merge işlemi, dizinin uzunluğu olan n işlem kadardır.
Yani O(n*logn) -> O(6log6)

