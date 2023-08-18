# Introduksjon til variabler, input og datatyper

_Under kan du lese om en del forklaringer og eksempler knyttet til oppgavene. Kan du noe eller alt av dette fra før kan du godt starte på oppgavene uten å lese noe. Det er kun oppgavene som leveres inn._

## Variabler

Variabler i programmering fungerer som bokser eller beholdere som holder på informasjon. Denne informasjonen kan være tekst (strenger), tall (heltall eller desimaltall), lister og mange andre datatyper. I Python kan du opprette en variabel ved å gi den et navn og deretter tildele den en verdi med et likhetstegn (`=`).

### Eksempler

Tilordning av et heltall til en variabel:

```Python
alder = 18
```

Tilordning av en streng til en variabel:

```Python
navn = "Ola"
```

Tilordning av et desimaltall (float) til en variabel:

```Python
hoyde = 1.75  # Høyde i meter
```

## Datatyper

I programmering refererer datatyper til de ulike typene verdier som en variabel kan holde. Python, som mange andre programmeringsspråk, har en rekke innebygde datatyper. Noen av de mest vanlige datatypene i Python er:

### Integers (heltall)

**Integers (heltall)**: Disse er positive eller negative hele tall, uten desimalpunkt. F.eks., 1, -5, 0, 1000.

#### Eksempel:

```Python
mitt_heltall = 10
```

### Float (desimaltall)

**Float (desimaltall)**: Disse er tall med et desimalpunkt. F.eks., 3.14, -0.01, 2.0.

#### Eksempel:

```Python
pi = 3.14
```

### String (tekst)

**String (strenger)**: Dette er sekvenser av karakterer, og de er definert ved å være innenfor enkle eller doble anførselstegn. F.eks., "Hei", 'Python', "1234".

#### Eksempel:

```Python
tekst = "Python er gøy!"
```

### Boolean

**Boolean (boolske verdier)**: Dette er enten True eller False. De brukes ofte i betingelser og logiske operasjoner.

#### Eksempel:

```Python
roboter_er_kult = True
```

### Lister

**Lister**: En samling av verdier som kan være av hvilken som helst datatype. De er definert ved å være innenfor firkantparanteser. F.eks., [1, 2, 3] eller ["a", "b", "c"].

#### Eksempel:

```Python
karakterer = [1, 2, 3, 4, 5, 6]
```

## Input

I Python, kan vi bruke den innebygde funksjonen `input()` for å hente informasjon fra brukeren. Når denne funksjonen blir kjørt, stopper programmet opp og venter på at brukeren skal skrive noe. Det brukeren skriver blir så returnert som en streng. Dette kan lagres i en variabel.

### Eksempel

Hente brukerens navn:

```Python
bruker_navn = input("Hva er navnet ditt? ")
print(f"Hei, {bruker_navn}!")
```

## Typekonvertering i Python

Ofte trenger vi å konvertere en verdi fra én datatype til en annen. Dette kalles typekonvertering eller typecasting. Python gir oss innebygde funksjoner for å gjøre dette.

### Eksempler

#### Fra Streng til Heltall eller Desimaltall:

For å konvertere en streng som inneholder tall til en `int` (heltall) eller `float` (desimaltall):

```Python
streng_til_int = int("123")
streng_til_float = float("123.45")
```

#### Fra Heltall eller Desimaltall til Streng:

```Python
int_til_streng = str(123)
float_til_streng = str(123.45)
```

#### Fra Heltall til Desimaltall og omvendt:

```Python
int_til_float = float(123)
float_til_int = int(123.45)  # Dette vil avrunde tallet ned
```

#### Fra andre datatyper til Boolske verdier (Boolean):

I Python vil nesten alle verdier evalueres til `True` når de konverteres til en boolsk verdi, unntatt noen "tomme" eller "null"-verdier som `0`, `""`, `[]`, og `None`, som alle vil bli `False`.

```Python
bool_av_int = bool(1) # Dette vil være True
bool_av_tom_streng = bool("") # Dette vil være False
```
