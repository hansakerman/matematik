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

Två tärningar ger två olika ögontal (som i övning 1, där de två dragna kulorna har olika färger):

$$\binom{6}{2} = 15$$

Om båda tärningarna även får visa samma ögontal (t.ex. två sexor) tillkommer 6 par, totalt $15 + 6 = 21$. Det kan också skrivas som $\binom{6+2-1}{2} = \binom{7}{2} = 21$.
