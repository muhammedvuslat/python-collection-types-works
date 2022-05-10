# python-collection-types-works
**String** **Metodları** 
  kalın metin

## Changing metod = Değiştirme yöntemleri

# Upper metodu, karakterleri büyük harfe çevirir.
sentence2 = " I live and work in, Virginia"
sentence2 = sentence2.upper()
print(sentence2)

# Lower metodu, karakterleri küçük harfe çevirir.
sentence3 = " I live and work in, Virginia"
sentence3 = sentence3.lower()
print(sentence3)

# Title metodu, karakter dizisindeki her kelimenin baş harfini küçük harfe çevirir.
sentence4 = " I live and work in, Virginia"
sentence4 = sentence4.lower()
print(sentence3)

# Capitalize, karakter dizisindeki sadece ilk kelimenin baş harfini büyük harfe çevirir.
sentence5 = "merhaba"
sentence5 = sentence5.capitalize()
print(sentence5)

# Replace metodu karakter güncellemesi için kullanılır. 
sentece6 = "My name is vuslat"
sentece6 = sentece6.replace("vuslat", "mehmet")
sentence1 = "0yayı 0yala"
sentence1 = sentence1.replace("0", "o") # o harfi yerine 0 sıfır rakamı kullanılmış
print(sentece6, sentence1)

# Bu metot eğer harf küçük ise büyük harfe çevirir eğer büyükse küçük harfe çevirir.
sentece7 = "MeRhAbA bU gÜzEl"
sentece7 = sentece7.swapcase()
sentece8 = "ESKİSİ gibi"
sentece8 = sentece8.swapcase()
print(sentece7, sentece8)



#Editing a String = Dize düzenleme


# string.strip() metodu başından ve sonundan olan boşlukları ve escape sequenceleri sıfırlar
space_string = "       listen first   "
print(space_string.strip())


space_string = "\n       listen first   \t"
print(space_string.strip())

# string.rstrip() metodu sağdan olan boşlukları ve escape sequenceleri sıfırlar sıfırlar
space_string = "\n       listen first   "
print(space_string.rstrip())


# string.lstrip() metodu soldan olan boşlukları ve escape sequenceleri sıfırlar sıfırlar
space_string = "       listen first   \t"
print(space_string.lstrip())


# Örnekler
# strip metodu baştan ve sondan "i" "iy" "yi" "y" kobinasyonlarını dener ve uyanları kaldıdır
source_string = "interopebiliyt"
source2_string = "imteropebiliy"
print(source_string.strip("yi"))
print(source2_string.strip("yim")) # Harf sayısı farketmeksizin bütün kombinasyonları dener

# örnek
text = 'tyou can learn almost everything in pre-classz'
text = text.strip("tz").upper()
print(text)

# --örnek--
# burada f döndürme kullanılmıştır
#    123456789
f = "ın good wee trust"
f1 = f[:9]
f2 = f[-7:]
print(f1+f2)

# --örnek--
# burada replace kullanılmıştır
text1 = 'ın good wee trust'
print(text1.replace('ee', 'e'))

#**COLLECTİON TYPES** 

## List

### Creating a List = Liste oluşturma

list.()

[ ] 

# [] her çeşit veriyi alır


# list() 1- İçeriye iterable veriyi alır 
# 2. İterable veriyi elemanlara ayırıyor 
# 3. Baştan sona kadar virgül koyar
# 4. İterable elemanlarının sonunda listenin elemanı halie getiriyor


list("clarusway") # list fonsiyonunu elemanlarına ayırdı ve ----> [] listeye aktardı


a = [1, 2, 3, 4]
list(a)

list_1 = ['h', 'a', 'p', 'p', 'y']
world = "happy"
list_2 = list(world)
print(list_1)
print(list_2)

list(1234) # hata vericek iterable olmadığı için 

string_1 = "I quit smoking" #boşluklar da dahil elemanlarına ayırdı 
new_list_1 = list(string_1)
print(new_list_1)

new_list_2 = [string_1] # İçerisine ne yazılırsa elemanlar o olur
print(new_list_2)


mixed_list = [11, 'Joseph', False, 3.14, None, [1, 2, 3]]
             #int,  str,    bool,   float, noe type, list,
             #Bir listeninin bileşenleri farklı çeşitler barındırabilir 
print(mixed_list)

my_list = ['Joseph', 'Clarusway', 2020] 
new_list1 = list(my_list)
new_list2 = [my_list] # my listi manuel olarak [] parantezinin içerisine koydu 

print(new_list1) # my listin list fonsiyonu
print(len(new_list1)) # len fonsiyonu saydırdığı için new listi sayarak 3 cevabını verir
print(new_list2) 
print(len(new_list2))

mesela = [[1,2,4],False, "ali", 11, ["veli", ["deli"]]]
len(mesela)

len([[[" "]]])









### Basic Operations with Lists=Listelerle Temel İşlemler

.append()

.pop()

.insert()

# Boş liste örnekleri
[]
list()  


# .append() listenin sonun eleman ekler
listem = []

# ÖRNEK
listem.append(11) # listem ekleme yapacak 
# her çalıştırmada ekleme yapcaktır

# ÖRNEK
listem.append(True)
listem

# ÖRNEK
listem.append("merhaba")
listem

# ÖRNEK
listem.append(3.14)
listem

# ÖRNEK
# -1 elemanı döndğrecek yani sol taraf tan yazılan indexi silecek
listem.pop() # son elemanı return remove edecek

# ÖRNEK
listem # son elemanı sildi

# ÖRNEK
listem.pop(1) # 1. indexi sildi ve bunu sildiğinin çıktı verdi

# ÖRNEK
listem # Çıktıda silinen değeri düşüp son kalan stringi bize çıktı verdi

# ÖRNEK
bir_list = []
bir_list.append(6666)
bir_list.append("multiverse")
bir_list.append([0])

print(bir_list)

# .insert hangi indexe eleman eklemek istiyorsanız oraya ekleme yapar
# belirtilen index konumu ne ise atamayı sağlayacaktır

iki_list = ["ahmet", "deli", 22]
          #    0       1     2   

iki_list.insert(2, "sezer") # iki defa çalıştığından dolayı iki defa sezer yazmış oldu
iki_list



