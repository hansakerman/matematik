# Egna uppgifter

Mina egna uppgifter jag skapat för att läsa själv.

## Statistik

### Övning 1

Det finns 6 kulor, alla i olika färger. Inför varje dragning lägger du tillbaka kulorna. Du drar 2 kulor åt gången och antecknar färgerna. Hur många olika färgpar kan du få?

Ordningen spelar ingen roll: att dra en röd och sedan en gul räknas som samma färgpar som att dra en gul och sedan en röd.

**Lösning:**

Du använder binomialkoefficienten, "n över k", som anger på hur många sätt man kan välja $k$ saker bland $n$ när ordningen inte spelar roll:

$$\binom{n}{k} = \frac{n!}{k!\,(n-k)!}$$

Här är $n = 6$ (kulor) och $k = 2$ (dras):

$$\binom{6}{2} = \frac{6!}{2!\,(6-2)!} = \frac{6!}{2!\,4!} = \frac{6 \cdot 5}{2 \cdot 1} = \frac{30}{2} = 15$$

Det finns alltså **15** olika färgpar.

### Övning 2

Samma som övning 1 men nu är det med två tärningar.

**Lösning:**

Analogin med övning 1 håller inte helt. Kulorna är 6 olika föremål, så ett par kan aldrig bestå av samma kula två gånger. Tärningarna kan däremot visa samma ögontal (t.ex. två sexor), så kombinationer med upprepning är tillåtna.

Ordningen spelar fortfarande ingen roll (en 2:a och en 5:a är samma utfall som en 5:a och en 2:a). Antalet sätt att välja $k$ av $n$ med upprepning, utan hänsyn till ordning, är:

$$\binom{n+k-1}{k}$$

Här är $n = 6$ (ögontal) och $k = 2$ (tärningar):

$$\binom{6+2-1}{2} = \binom{7}{2} = \frac{7!}{2!\,5!} = \frac{7 \cdot 6}{2 \cdot 1} = 21$$

Kontroll: 15 par med olika ögontal (som i övning 1) plus 6 par med samma ögontal ger $15 + 6 = 21$.

Det finns alltså **21** olika kombinationer.
