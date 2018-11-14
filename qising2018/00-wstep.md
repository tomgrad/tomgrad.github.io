---
theme: league
transition: concave
css: custom.css
revealjs-url: ../reveal.js
---

#
## Fizyka Ogólna
### dr inż. Tomasz Gradowski
#### Wykład dla kierunku Informatyka oraz Automatyka i Robotyka, Wydział Elektroniki i Technik Informacyjnych

## Kontakt

**dr inż. Tomasz Gradowski**

- `tomasz.gradowski@pw.edu.pl`
- `http://if.pw.edu.pl/~tomgrad`
- terminy konsultacji na stronie www
- Gmach Fizyki PW, pokój 6
- *tel:* `022 234 7958`

## Regulamin

*pełna treść regulaminu na stronie WWW*

- wykład 30h, ćwiczenia 30h
- punktacja: 25 p. (ćwiczenia) + 25 p. (egzamin) = 50 p.
- warunek dopuszczenia do egzaminu: ­13 p. z ćwiczeń
- egzamin: pisemny (test wielokrotnego wyboru)
- do 25.5 p. ocena niedostateczna, dalej pół oceny co 5 p.
- kolokwium poprawkowe na koniec semestru (ew. początek
sesji)

#
## Plan wykładu
### Mechanika
- Opis ruchu. Układy odniesienia.
- Opis ruchu układu fizycznego. Rodzaje sił. Zasady dynamiki Newtona. Równania ruchu.
- Zasady zachowania a symetria w fizyce. Zasady zachowania pędu i momentu pędu. Siły zachowawcze. Zasada zachowania energii. 
- Ruch drgający. Rezonans układów drgających. Wpływ nieliniowości układu na własności ruchu (ruch regularny i chaotyczny, przyczynowość równań ruchu, rezonans nieliniowy). 
- Ruch falowy. Równania ruchu falowego.

##
### Elektrodynamika
- Pole elektryczne. Prawo Coulomba. Natężenie i potencjał pola elektrycznego.
- Prawo Gaussa. Równanie Poissona. Pole elektryczne w dielektryku (zjawisko polaryzacji dielektrycznej).
- Pole magnetyczne. Siła Lorentza. Prawo Ampere’a dla prądów stałych i dla prądów zmiennych. 
- Prawo indukcji Faradaya. Indukcyjność. Niejednoznaczność potencjału skalarnego dla pola magnetycznego potencjał wektorowy. Prawo Biote’a-Savarta. 
- Równania Maxwella (postać różniczkowa i całkowa,
interpretacja). Równania materiałowe. Rozwiązanie równań Maxwella dla próżni. Fale elektromagnetyczne.

#

## Literatura

### Podręczniki

- *W.Bogusz, J.Garbarczyk, F.Krok*, Podstawy Fizyki, 
<br/>Oficyna Wydawnicza Politechniki Warszawskiej, Warszawa 1997.

- *I.W.Sawieliew*, Wykłady z fizyki, t.1 Mechanika i fizyka, cząsteczkowa t.2 Elektryczność i magnetyzm, fale, optyka. 
<br/>Wyd. Naukowe PWN, Warszawa 1994.

### Zbiory zadań

- *K.Blankiewicz, M.Igalson*, Zbiór zadań rachunkowych z fizyki
- *A.Hennel, W.Szuszkiewicz*, Zadania i problemy z fizyki, tom 1 i 2

# Czym jest fizyka?

## W.Bogusz, J.Garbarczyk, F.Krok
*Podstawy Fizyki*

> Fizyka jest najbardziej podstawową nauką przyrodniczą, zajmującą się badaniem fundamentalnych i uniwersalnych własności materii oraz zjawisk w otaczającym nas świecie. Nazwa fizyka pochodzi od greckiego słowa physis, czyli przyroda. Fizyka jest ścisłą i ilościową nauką empiryczną. Posługuje się ona wielkościami fizycznymi, które można ująć ilościowo, a wyniki badań przedstawia w postaci liczb i praw wyrażonych matematycznie.

## I.W.Sawieliew
*Wykłady z fizyki*

> Fizyka jest nauką o najogólniejszych własnościach i formach ruchu materii. Klasyczne określenie materii sformułował W.I.Lenin w ksiażce “Materializm a empiriokrytycyzm”: 

> Materia jest filozoficzną kategorią służącą do oznaczenia obiektywnej rzeczywistości, która dana jest człowiekowi we wrażeniach, którą nasze wrażenia kopiują, fotografują, odzwierciedlają, a która istnieje niezależnie od nich. 

---

> W przytoczonym tekście istotne są dwa spostrzeżenia: 1) materia istnieje obiektywnie, tzn. niezależnie od czyjejkolwiek świadomości i wrażeń, oraz 2) materia jest kopiowana, odzwierciedlana przez nasze wrażenia, a więc jest poznawalna. Z przyjętego określenia fizyki wynika, że skupia ona wiedzę o najogólniejszych
własnościach i zjawiskach świata zewnętrznego.

## Sam Edwards
*University of Cambridge (1928-2015)*

> Physics is what physicists do.

## R. Sinatra, P. Deville, M. Szell, D. Wang, A.-L. Barabasi
*A century of physics, Nature Physics 11, 797 (2015)*

> In this era of interdisciplinary science, of biological physics, network science and econophysics, defining physics as the science of the properties of matter and energy is increasingly outdated and inaccurate. We are therefore prompted to ask anew: what is physics? 

---

> When two engineers accidentally discover cosmic microwave background radiation, is that physics or engineering? When a physicist uncovers the structure of DNA, is that biology or physics? Is the interdisciplinary role of physics something new - a potential fad - or has it always been an integral part of the field? Is physics dying or thriving, becoming more insular or more interdisciplinary?

#
##
### Rzędy wielkości - rozmiar

| obiekty            | rozmiar [m] |
| ------------------ | ----------- |
| kwarki             | $10^{-18}$  |
| elektrony, protony | $10^{−15}$  |
| jądra atomów       | $10^{−14}$  |
| atomy              | $10^{−10}$  |
| wirusy             | $10^{−7}$   |
| człowiek           | $10^0$      |
| Ziemia             | $10^7$      |
| Słońce             | $10^{10}$   |
| Galaktyka          | $10^{22}$   |
| obs. Wszechświat   | $10^{26}$   |


##
### Rzędy wielkości - czas

| zjawiska                              | czas [s]   |
| ------------------------------------- | ---------- |
| niektóre cząstki elem.                | $10^{−23}$ |
| czas życia człowieka                  | $10^{9}$   |
| wiek Wszechświata                     | $10^{17}$  |
| okres rozpadu niektórych pierw. prom. | $10^{24}$  |

#
## Oddziaływania fundamentalne

| rodzaj             | natężenie wzg. | zasięg [m] | źródła    |
| ------------------ | -------------- | ---------- | --------- |
| silne              | $1$            | $10^{−15}$ | nukleony  |
| elektromagnetyczne | $10^{−2}$      | ∞          | ładunki   |
| słabe              | $10^{−5}$      | $10^{−18}$ | cz. elem. |
| grawitacyjne       | $10^{−38}$     | ∞          | masy      |

## 
### Oddziaływanie grawitacyjne

Prawo powszechnego ciążenia Newtona:

> $F = G \frac{m_1 m_2}{r^2}$

$G = 6.67 \times 10^{-11} \frac{kg \cdot m}{s^2}$ - stała grawitacji

## 
### Oddziaływanie elektromagnetyczne

Bozon cechowania: **foton**

Prawo Coulomba:

> $F = \frac{1}{4 \pi \varepsilon_0} \frac{Q_1 Q_2}{r^2}$

## 
### Oddziaływanie silne (jądrowe)
Bozon cechowania: **gluon**

- Odpowiedzialne za wiązanie nukleonów w jądra atomowe.

- Silne przyciąganie przewyższa elektrostatyczne odpychanie
między protonami.

## 
### Oddziaływanie słabe

Bozony cechowania: **$W_+$, $W_-$, $Z$**

Odpowiedzialne za rozpad nietrwałych cz. element.
(rozpad $\beta$). 

Przykłady: 

- rozpad swobodnego neutronu (czas życia rzędu $10^3 s$)

$n^0 \rightarrow p^+ + e^- + \tilde \nu_e$

- Rozpad mionu (czas życia $2.2 \times 10^{-6} s$ ):

$\mu_- \rightarrow e^- + \nu_\mu + \tilde \nu_e$

$\mu_+ \rightarrow e^+ + \tilde \nu_\mu +  \nu_e$


#
## Wielkości fizyczne

- **skalary** - wyrażane za pomocą jednej liczby ($m$ - masa, $W$ - praca, $\varphi$ - potencjał elektryczny)
  
- **wektory** - wyrażane przez $n$ uporządkowanych liczb tzw. współrzędnych lub składowych ($\vec v$ - prędkość, $\vec E$ - natężenie pola elektrycznego)

- **tensory** - wyrażane przez macierze ($\hat \mu_r$ - przenikalność magnetyczna, $\hat I$ - moment bezwładności)
