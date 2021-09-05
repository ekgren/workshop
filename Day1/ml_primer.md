# Maskininlärning 

## Vad är Maskininlärning?

I korthet: Metoder som *lär* sig lösa problem från *data*.

Exempel: 
    - Bildigenkänning
    - Rekommendationssystem
    - Språkmodeller

## Vad är Maskininlärning?

Brukar delas upp i tre fält beroende på hur datan, problemet och hur dessa relaterar till varandra. 
- Övervakad inlärning
- Oövervakad inlärning
- Förstärkningsinlärning

### Övervakad inlärning

I korthet: Om man har tillgång till indata och önskad utdata, kan man bygga en modell som lär sig mappningen indata - utdata.

Exempel: 
    - Bildigenkänning med indata (bilder) och utdata (etiketter), i.e. etiketterade bilder.

Tar ofta formen av klassificering eller regression:

klassificering:
    Att givet data försöka mappa det till en av flera fördefinierade klasser. t.ex. sifferigenkänning: Mappa bild till symboler.

Regression:
    Att givet data försöka mappa det till en skalär, eller vektor. t.ex. mappa lägenhetsannonser till säljpris. 
    (Notera att klassificering ofta är enklare, då regression kräver antaganden om vad "närhet" är i den aktuella kontexten.)

### Oövervakad inlärning

I korthet: Om man har tillgång till data och vill finna struktur i datan så som den är. 

Exempel: 
    - Språkmodellering, där datan är text och modellen lär sig hur text "ser ut".

### Förstärkningsinlärning

I korthet: Om man har en agent som ska lära sig utföra handlingar i en miljö.

Exempel:
    - Spel-AI, där agenter lär sig vilka handlingar som ska utföras i vilka situationer för att vinna.

### Neurala Nätverk

En typ av maskininlärning inspirerad av neuroner. 

Formulera problemet som ett **optimeringsproblem**

Exempel: Bildigenkänning

#### Bildigenkänning med Neurala Nätverk

- Problem: Läs siffror ur bilder.
- Optimeringsproblem: Finn en funktion $f$ som givet indata i form av en bild, get utdata i form av en sannolikhetsdistribution över siffror. 
- Funktionen $f$ ska vara parameteriserd och differentierbar.
- Funktionen $f$ tränas och utvärderas på tillgänglig data, med förhoppningen att den ska generalisera till ny data. 

Detta är ett exempel på övervakad inlärning: Vi har indata (bilder) och utdata (siffror), och försöker finna en mappning mellan dem. 

#### Bildigenkänning med Neurala Nätverk

$f : X \times \Theta \rightarrow Y$

### Loss

I korthet tränas neurala nätverk genom att hitta en parameterisering som minimerar en "loss", eller felfunktion.

I fallet klassificering ges lossen ofta av cross entropy: ett mått på hur en prediktion (i form av en sannolikhetsdistribution) överenstämmer med verkligheten.

I fallet regression ges lossen ofta av ett avståndsmått mellan det predicerade värdet och verkligheten. 

### Backprop 

Neurala nätverk är parameteriserade och differentierbara med avseende på dess parametrar. Detta innebär att när man beräknat lossen,
kan beräkna gradienten.

### Optimering

Man kan finna parametrar som minimerar lossen genom att uppdatera parametrarna med gradienten. 

### Modeller


### Domäner
