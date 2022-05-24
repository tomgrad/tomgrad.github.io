---
title: Atom wodoru
---

# Atom wodoru
<!-- c -->
- kwantowy opis atomu wodoru został bardzo dobrze **potwierdzony eksperymentalnie**
- opis słuszny również dla innych wodoropodobnych atomów ($Z-1$ krotnie zjonizowanych, czyli z jednym elektronem)
- ponieważ **potencjał** jest **coulombowski**, wystarczy rozważyć położenie elektronu względem jądra
- problem jest **stacjonarny** (równanie Schrödingera niezależne od czasu)
- opis wymaga rozwiązania równania Schrödingera w 3 wymiarach
- ze względu na symetrię problemu potrzebujemy operatora Laplace'a ($\nabla^2$) w układzie **współrzędnych sferycznych**

<!-- c| -->

### równanie Schrödingera

$\frac{-\hbar^2 }{2m} \nabla ^2 \Psi + V(r) \Psi = E\Psi$


### funkcja falowa

$\Psi = \Psi(r, \vartheta, \varphi)$

### potencjał

$V(r) = - \frac{Ze^2}{4 \pi \varepsilon_0} \frac{1}{r}$ 

- $Z$ - liczba atomowa (liczba protonów w jądrze)
- $e$ - ładunek elektronu

<!-- c. -->
----

<!-- c -->
- laplasjan we współrzędnych sferycznych
- używamy metody **rozdzielenia zmiennych**
- postulowaną postać $\Psi$ wstawiamy do równania Schrödingera
- otrzymane równanie mnożymy stronami przez $- \frac{2mr^2 \sin^2\vartheta}{\hbar^2 R \Theta \Phi }$

<!-- c| -->

$\nabla ^2 ={\frac {1}{r^{2}}}{\frac {\partial }{\partial r}}\left(r^{2}{\frac {\partial}{\partial r}}\right)+
{\frac {1}{r^{2}\sin \vartheta }}{\frac {\partial }{\partial \vartheta }}\left(\sin \vartheta {\frac {\partial}{\partial \vartheta }}\right)+
{\frac {1}{r^{2}\sin ^{2}\vartheta }}{\frac {\partial ^{2}}{\partial \varphi ^{2}}}$

<br/>

$\Psi(r, \vartheta, \varphi) = R(r) \Theta(\vartheta) \Phi(\varphi)$

<!-- c. -->

<br/>

$\frac{-\hbar^2 }{2m} \left[
\Theta\Phi \frac{1}{r^2} \frac{\partial}{\partial r} \left( r^2 \frac{\partial R}{\partial r} \right)+
\frac{R\Phi}{r^2\sin\vartheta} \frac{\partial}{\partial \vartheta} \left( \sin\vartheta \frac{\partial \Theta}{\partial \vartheta}\right) + 
\frac{R \Theta}{r^2 \sin^2\vartheta} \frac{\partial^2\Phi}{\partial \varphi^2}
\right] + V(r)R\Theta\Phi = E R \Theta \Phi$

----

$\frac{1}{\Phi} \frac{d^2\Phi}{d\varphi^2} = 
\frac{\sin^2 \vartheta}{R} \frac{d}{dr} \left( r^2 \frac{dR}{dr}\right) - 
\frac{\sin\vartheta}{\Theta} \frac{d}{d\vartheta} \left( \sin \vartheta \frac{d\Theta}{d\vartheta}\right) -
\frac{2mr^2 \sin^2 \vartheta}{\hbar^2} [E-V(r)]
$

<!-- c -->

- Lewa strona zależy wyłącznie od $\varphi$, prawa wyłącznie od $r$ i $\vartheta$.
- Muszą więc być równe stałej.
- Przyrównujemy obie strony do $-m_l^2$.

<!-- c| -->

$\frac{d^2 \Phi}{d \varphi^2} = -m_l^2\Phi$

$\Phi(\varphi) = \Phi_{m_l} (\varphi) = A e^{im_l\varphi}$

$\Phi(0) = \Phi(2\pi) \Rightarrow m_l=0, \pm 1, \pm 2, \ldots$

<!-- c. -->

Po wstawieniu $\Psi$ otrzymujemy:

$\frac{1}{R} \frac{d}{dr} \left( r^2 \frac{dR}{dr}\right) + \frac{2mr^2}{\hbar^2} \left[ E-V(r) \right] = 
\frac{m_l^2}{\sin^2\vartheta} - \frac{1}{\Theta \sin\vartheta} \frac{d}{d\vartheta} \left( \sin\vartheta \frac{d\Theta}{d\vartheta} \right)$

<br>

Lewa strona zależy wyłącznie od $r$, prawa od $\vartheta$, przyrównujemy więc obie strony do $l(l+1)$.

<br>

**Uwaga:** na tym etapie wielkości $m_l$ i $l(l+1)$ to po prostu pewne stałe. Ich interpretacja pojawi się później.

----

## Równanie azymutalne

$- \frac{1}{\sin\vartheta} \frac{d}{d\vartheta} \left( \sin\vartheta \frac{d\Theta}{d\vartheta} \right) + \frac{m_l^2 \Theta}{\sin^2\vartheta} = l(l+1)\Theta$

## Równanie radialne

$
\frac{1}{r^2} \frac{d}{dr} \left( r^2 \frac{dR}{dr}\right) + 
\frac{2m}{\hbar^2} \left[ E-V(r) \right]R = l(l+1)\frac{R}{r^2}
$

---

## Rozwiązanie równania azymualnego

<!-- c -->
- równanie znane jest w teorii funkcji specjalnych
- rozwiązaniami są [**stowarzyszone wielomiany Legendre'a**](https://en.wikipedia.org/wiki/Associated_Legendre_polynomials)

$\Theta(\vartheta) = \Theta_{l,m_l}(\vartheta) \propto P_{l,m_l}(\cos \vartheta)$

<!-- c| -->

$
l \geq | m_l |
$

$l=0, 1, 2, \ldots$

$m_l = 0, \pm 1, \pm 2, \ldots, \pm l$

- stany odpowiadające danemu $l$ są $(2l+1)$-krotnie **zdegenerowane**
<!-- c. -->

<br>

### Degeneracja

- istnienie więcej niż jednej funkcji własnej o tej samej wartości własnej
- wiele stanów kwantowych ma tę samą energię.

----

## Część kątowa funkcji falowej

<!-- c -->

$Y(\vartheta, \varphi) = \Theta(\vartheta) \Phi(\varphi)$

$Y_{l, m_l}(\vartheta, \varphi) = N_{l, m_l} \cdot
P_{l, m_l}(\cos\vartheta) \cdot e^{i m_l \varphi}
$

- $P_{l, m_l}$ - stowarzyszone wielomiany Legendre'a 
- $N_{l, m_l}$ -  stała normująca

<!-- c| -->

- funkcja kulista, harmonika sferyczna
- numerowana dwoma indeksami: $l$ i $m_l$
- ta sama funkcja jest funkcją własną operatora $\hat {L^2}$ (kwadratu momentu pędu)
- stąd będzie wynikać fizyczna interpretacja indeksów $l$ i $m_l$

<!-- c. -->

----

## Normalizacja

Stałą $N_{l, m_l}$ wyznaczamy normalizując funkcję sferyczną:

$
\int\limits_o^\pi d\vartheta \int\limits_o^{2\pi} d\varphi \left|Y_{l, m_l}(\vartheta, \varphi)\right |^2 \sin \vartheta =1
$

Stąd otrzymujemy:

$N_{l, m_l} = (-1)^{m_l} 
\sqrt{\frac{2l+1}{4\pi} \frac{(l-|m_l|)!}{(l+|m_l|)!}}$

Kilka pierwszych [funkcji kulistych](https://en.wikipedia.org/wiki/Table_of_spherical_harmonics):

<!-- e -->
& Y_{0,0}(\vartheta,\varphi) &=& {1 \over \sqrt { 4\pi }} \\
& Y_{1,0}(\vartheta,\varphi) &=& {\sqrt {3 \over 4\pi }} \cdot \cos \vartheta \\
& Y_{1,\pm 1}(\vartheta,\varphi) &=& {\sqrt {3 \over 8\pi }} \cdot \sin \vartheta \cdot e^{\pm i \varphi}\\
<!-- e. -->

----

## Rozwiązanie równania radialnego

<!-- c -->

- w rozwiązaniu pojawiają się [stowarzyszone wielomiany Laguerre'a](https://en.wikipedia.org/wiki/Laguerre_polynomials) $L_n^{\alpha}$

$
R_{n, l}(r) = N_{n, l} \cdot e^{\rho \over 2} \cdot \rho^l \cdot L_{n+l}^{2l+1}(\rho)
$

<!-- c| -->

- podstawienie: $\rho = \frac{Zr}{2\pi\varepsilon_0 n a_0}$
- $a_0 = \frac{\hbar^2}{me^2}$ - [promień Bohra](https://en.wikipedia.org/wiki/Bohr_radius)
- $N_{n, l}$ - stała normująca

<!-- c. -->

<br><br>

### Normalizacja

$\int\limits_0^\infty = R_{nl}^\star R_{nl} r^2 dr = 1$

$N_{n, l} = - \sqrt{\left( \frac{2Z}{n a_0}\right)^3 \frac{1}{(4\pi\varepsilon_0)^3}\frac{(n-l-1)!}{2n[(n+1)!]^3}}$


---

## Interpretacja funkcji falowej

$\Psi_{n, l, m_l}(r, \vartheta, \varphi) = R_{n, l}(r) \cdot Y_{l, m_l}(\vartheta, \varphi)$

<!-- c -->

- $R_{n, l}(r)$ - część radialna
- $Y_{l, m_l}(\vartheta, \varphi)$ - część kątowa

<!-- c| -->

### Liczby kwantowe

- $n=1, 2, 3, \ldots$
- $l=0, 1, 2, \ldots, n-1$
- $m_l = -l, \ldots, 0, \ldots, l$

<!-- c. -->

<!-- $\int |\Psi_{n, l, m_l}(r, \vartheta, \varphi)|^2 dV = \int\limits_0^\infty dr  \int\limits_o^\pi d\vartheta \int\limits_o^{2\pi} d\varphi~ r^2 \sin \vartheta \left|R_{n, l}(r) Y_{l, m_l}(\vartheta, \varphi)\right |^2  =1$ -->

<br>

- kwadrat modułu funkcji falowej - gęstość prawdopodobieństwa znalezienia układu fizycznego w pewnym obszarze
- $e \Psi^\star \Psi$ - gęstość ładunku elektrycznego odpowiadającego elektronowi
- elektron nie jest zlokalizowany
- elektron jest chmurą elektryczną, której kształt i gęstość wynika z postaci $\Psi_{nlm_l}$

----

## Liczby kwantowe

<!-- c21 -->
### $n=1, 2, 3, \ldots$

- główna liczba kwantowa
- określa tzw. powłokę (poziom energetyczny) na której jest elektron
- $E_n = - \frac{m}{2\hbar^2} \left( \frac{e^2}{4\pi\varepsilon_0} \right)^2 {1 \over n^2}$
- $n=1$ - stan podstawowy



### $l = 0, \ldots, n-1$

- poboczna liczba kwantowa
- określa kwadrat momentu pędu
- $L^2 = l(l+1) \hbar^2$

### $m_l=-l, \ldots, l$

- magnetyczna liczba kwantowa
- określa składową momentu pędu w wyróżnionym kierunku ($z$)
- $L_z = m \hbar$

<!-- c| -->
![](moment.png)

<!-- c. -->

----

## Część radialna

<!-- c -->

- $R_{10}$ ($n=1$, $l=0$)
- tzw. orbital *s*
- maksimum prawdopodobieństwa dla odległości równej $a_0=0.529 Å$ (promień Bohra)


![](R10.png)

[Źródło](https://demonstrations.wolfram.com/HydrogenAtomRadialFunctions/)

<!-- c| -->

- $R_{20}$ ($n=2$, $l=0$) - orbital *s*

![](R20.png)

- $R_{21}$ ($n=2$, $l=1$) - orbital *p*

![](R21.png)
<!-- c. -->

----
<!-- c -->

Nazwy orbitali dla kolejnych wartości $l$:

- *s*  $(l=0)$
- *p*  $(l=1)$
- *d*  $(l=2)$
- *f*  $(l=3)$

<br><br>

- $R_{31}$

![](R31.png)

<!-- c| -->
- $R_{30}$
  
![](R30.png)

- $R_{32}$

![](R32.png)
<!-- c. -->

----

<!-- c -->
- $R_{40}$

![](R40.png)

- $R_{42}$

![](R42.png)
<!-- c| -->
- $R_{41}$

![](R41.png)

- $R_{43}$

![](R43.png)
<!-- c. -->


----

<!-- c12 -->

## Część kątowa

- a) $\Theta_{00} = {1 \over \sqrt 2}$
- b) $\Theta_{10} = \sqrt {3 \over 2} \cos \vartheta$
- c) $\Theta_{1\pm 1} = {\sqrt 3 \over 2} \sin \vartheta $
- d) $\Theta_{20} = \sqrt {5 \over 8} (3\cos^2 \vartheta-1)$
- e) $\Theta_{2 \pm 1} = {\sqrt 15 \over 2} \sin \vartheta \cos \vartheta$
- f) $\Theta_{2 \pm 2} = {\sqrt 15 \over 4} \sin^2 \vartheta$

<!-- c| -->
![](ptheta_a.png)<!-- w30% -->
![](ptheta_b.png)<!-- w30% -->
![](ptheta_c.png)<!-- w30% -->

![](ptheta_d.png)<!-- w30% -->
![](ptheta_e.png)<!-- w30% -->
![](ptheta_f.png)<!-- w30% -->
<!-- c. -->

---

<!-- c12 -->
## Orbitale atomowe

- z nałożenia radialnych i kątowych gęstości prawdopodobieństwa powstają rozkłady przestrzenne gęstości prawdopodobieństwa znalezienia elektronu
- są to tzw. orbitale atomowe
- [symulacje](https://falstad.com/qmatom/)
<!-- c| -->
![](Atomic-orbital-clouds_spdf_m0.png)<!-- w80% -->
<!-- c. -->

----

<!-- c -->
## Układ okresowy

![](Simple_Periodic_Table_Chart-blocks.svg)
<!-- c| -->
- **okres** - liczba powłok, na których są elektrony
- **grupa** (wg. starej konwencji 1-8 oznaczała liczbę elektronów na ostatniej powłoce, tzw. walencyjnej)
- **liczba atomowa** (porządkowa) *Z* - liczba protonów w jądrze
- każdy kolejny atom ma o 1 proton i 1 elektron więcej
- na *n*-tej powłoce może zmieścić się $2n^2$ elektronów
  - $n^2$, bo $l=0 \ldots n-1$ i $2l+1$ wartośc $m_l$ dla każdego $l$
  - ... i wszystko razy *2*, bo 2 możliwe wartości **spinu**
  - kolejne powłoki nazywamy $K$, $L$, $M$, $N$, $O$, $P$, $Q$

<!-- c. -->

----

## Przykłady

<!-- c -->

### miedź (*Cu*)

- 4. okres
- *Z=29* elektronów niezjonizowanego atomu
  - powłoka *K* - 2 elektrony na orbitalu *s*
  - powłoka *L* - 2 el. na orbitalu *s*, 6 na *p*
  - powłoka *M* - 2 na *s*, 6 na *p*, 10 na *d*
  - powłoka *N* - 1 elektron na powłoce *s*
- taką konfigurację zapisujemy następująco:

$1s^2 2s^2 p^6 3s^2 p^6 d^{10} 4s^1$

<!-- c| -->

### neon (*Ne*)

- 2. okres
- *Z=10*
- $1s^2 2s^2 p^6$

### srebro (*Ag*)

- 5. okres
- *Z=47*
- $1s^2 2s^2 p^6 3s^2 p^6 d^{10} 4s^2 p^6 d^{10} 5s^1$

<!-- c. -->

----

## Spin

- elektron posiada własny (spinowy) moment pędu (spin) i związany z nim moment magnetyczny
- spin jest przestrzennie skwantowany, względem zewnętrznego pola magnetycznego ma **tylko 2 dozwolone ustawienia**
- nie istnieje operator spinowego momentu pędu w postaci różniczkowej. Odpowiedni operator znany jest tylko w postaci macierzowej.
  
<br><br>

<!-- c -->

### Doświadczenie Sterna-Gerlacha

<video width="75%" controls>
  <source src="https://upload.wikimedia.org/wikipedia/commons/9/9e/Quantum_spin_and_the_Stern-Gerlach_experiment.ogv" type="video/ogg">
Your browser does not support the video tag.
</video>

<!-- c| -->
Atom srebra posiada na najwyższej orbicie jeden niesparowany elektron, którego spin może być zwrócony w górę lub w dół. Niejednorodne pole magnetyczne odchyla kierunek ruchu atomów w wiązce w zależności od zwrotu spinu.
<!-- c. -->