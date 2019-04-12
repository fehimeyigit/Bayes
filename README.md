# Bayes

Olasılık teorileri arasında en popüler ve yaygın kullanılan teoridir. Olasılıkla ilgili daha önceden bilgi sahibi değilseniz olasılık yazımda bu konuyla ilgili temel kuralları açıklamaya çalıştım o yazıyı da okumanızı öneririm.

Bayes teoremi, 18. yüzyıl İngiliz matematikçisi Thomas Bayes’in adını verdiği koşullu olasılığı belirlemek için kullanılan matematiksel bir formüldür.


P(A|B) = B olayı gerçekleştiğinde A olayının gerçekleşme olasılığı
P(A) = A olayının gerçekleşme olasılığı
P(B|A) = A olayı gerçekleştiğinde B olayının gerçekleşme olasılığı
P(B) = B olayının gerçekleşme olasılığı

Şimdi bu formülün nasıl çıkarıldığına bakalım. Koşullu olasılık kuralını kullanacağız. Buna göre:

P(A|B) = P(A∩B) / P(B)

Formülünü kullanıyorduk. Aynı şekilde :

P(B|A) = P(B∩A) / P(A)

P(A∩B) = P(B∩A)

Yukarıdaki iki denklemi birleştirirsek.

P(A|B).P(B)=P(B|A).P(A) buradan Bayes kuralını çıkarabiliriz.

P(A|B) = P(B|A) . P(A) / P(B)

Şimdi bu kuralı kullanarak bir örnek yapalım.


E: Kusurlu cıvata
A: Cıvata A makinesinde yapıldı.
B: Cıvata B makinesinde yapıldı.
C: Cıvata C makinesinde yapıldı.
O halde,

P(A)=0.30, P(E/A)=0.01,
P(B)=0.30, P(E/B)=0.03,
P(C)=0.40, P(E/C)=0.02 dir. 

P(A∩E)=P(A).P(E/A)=(0.30).(0.01)=0.003
P(B∩E)=P(B).P(E/B)=(0.30).(0.03)=0.009
P(C∩E)=P(C).P(E/C)=(0.40).(0.02)=0.008 olur.
Bayes teoremini kullanarak P(A/E) olasılığı aşağıdaki gibi bulunur.

 P(A/E) =  P(A∩E) /((A∩E)+(B∩E)+(C∩E))
∩

  = 0.003/(0.003+ 0.009+0.008)
  =3/20
  
Benzer şekilde

P(B/E)=0.009/0.020 
    =9/20

P(C/E)=0.008/0.020 
       =8/20

elde edilir. 
