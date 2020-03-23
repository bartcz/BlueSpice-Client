**Obsah**

[Úvod 5](#_Toc34845550)

[1 Rozhodovací problém 6](#_Toc34845551)

[2 Fullerova metoda (Fullerův trojúhelník) 11](#_Toc34845552)

[3 Saatyho metoda 15](#_Toc34845553)

[3.1 Analyticko-hierarchický proces 21](#_Toc34845554)

[Použitá literatura 22](#_Toc34845555)

[Seznam příloh 23](#_Toc34845556)

  
**Seznam tabulek**

[Tabulka 4: Vstupní data 7](#_Toc34845523)

[Tabulka 5: Hodnoty 8](#_Toc34845524)

[Tabulka 6: Kritéria 9](#_Toc34845525)

[Tabulka 7: Cíle 9](#_Toc34845526)

[Tabulka 8: Alternativy 10](#_Toc34845527)

[Tabulka 9: Fullerova metoda – Kriteriální tabulka 11](#_Toc34845528)

[Tabulka 10: Cena (Fullerova metoda) 11](#_Toc34845529)

[Tabulka 11: Procesor (Fullerova metoda) 12](#_Toc34845530)

[Tabulka 12: RAM (Fullerova metoda) 12](#_Toc34845531)

[Tabulka 13: Disk (Fullerova metoda) 12](#_Toc34845532)

[Tabulka 14: Grafika (Fullerova metoda) 13](#_Toc34845533)

[Tabulka 15: Hmotnost (Fullerova metoda) 13](#_Toc34845534)

[Tabulka 16: Výdrž (Fullerova metoda) 13](#_Toc34845535)

[Tabulka 17: Vyhodnocení (Fullerova metoda) 13](#_Toc34845536)

[Tabulka 18: Saatyho metoda – Jazykové deskriptory 15](#_Toc34845537)

[Tabulka 19: Saatyho metoda – Kriteriální tabulka 15](#_Toc34845538)

[Tabulka 20: Cena (Saatyho metoda) 16](#_Toc34845539)

[Tabulka 21: Procesor (Saatyho metoda) 16](#_Toc34845540)

[Tabulka 22: RAM (Saatyho metoda) 16](#_Toc34845541)

[Tabulka 23: Disk (Saatyho metoda) 17](#_Toc34845542)

[Tabulka 24: Grafika (Saatyho metoda) 18](#_Toc34845543)

[Tabulka 25: Hmotnost (Saatyho metoda) 18](#_Toc34845544)

[Tabulka 26: Výdrž (Saatyho metoda) 18](#_Toc34845545)

[Tabulka 27: Přehled vypočtených hodnot (Saatyho matice) 19](#_Toc34845546)

[Tabulka 28: Hodnoty RI pro počet m kriterií (podle Whartona) 19](#_Toc34845547)

[Tabulka 29: Vyhodnocení (Saatyho metoda) 20](#_Toc34845548)

[Tabulka 30: Analyticko-hierarchický proces – vyhodnocení 21](#_Toc34845549)

**Seznam ilustrací**

[Obrázek 1: Rozhodovací problém – systém 6](#_Toc34845557)

[Obrázek 2: Fullerova metoda - graf 14](#_Toc34845558)

[Obrázek 3: Matlab M-file pro výpočet vlastního čísla (Saatyho matice)
20](#_Toc34845559)

[Obrázek 4: Saatyho metoda - graf 21](#_Toc34845560)

Úvod

V rámci této práce se se budu zabývat dílčími úkoly na předmět Rozhodovací
procesy (KROP)

![](media/c7355405832b802374d888a7578a1cd5.png)

Rozhodovací problém

Obrázek 1: Rozhodovací problém – systém

Cílem je výběr vhodného notebooku pro studenta. Vstupními daty pro výběr jsou:
cena, procesor, RAM paměť, disk, grafika počítače (která má podíl na výkonu
počítače také, včetně podílu na výdrži), dále hmotnost a výdrž.

Na výběr máme ze 4. alternativ. Jedná se o skutečné produkty, prodávané eshopem
Alza.cz. Vstupní data jsou v Tabulka 1.

Tabulka 1: Vstupní data

|                |                                             | K1                 | K2                                   | K3                            | K4                              | K5                                 | K6                     | K7              |
|----------------|---------------------------------------------|--------------------|--------------------------------------|-------------------------------|---------------------------------|------------------------------------|------------------------|-----------------|
|                | **Notebook**                                | **Cena**           | **Procesor**                         | **RAM**                       | **Disk**                        | **Grafika**                        | **Hmotnost**           | **Výdrž (v h)** |
|                |                                             | **(v kč)**         |                                      |                               |                                 |                                    | **(v kg)**             |                 |
| **A1**         | Lenovo ThinkPad E580                        | 18 990             | Intel i5 /                           | 8 GB /                        | Hybrid -                        | Integrovaná -                      | 2,1                    | 9               |
| *(ntb1)*       | (*ntb1*)                                    |                    | 4 core                               | DDR 4 /                       | HDD / SSD -                     | Intel UHD                          |                        |                 |
|                |                                             |                    |                                      | 2400 Mhz                      | 1TB + 256 GB                    | Graphics 620                       |                        |                 |
| **A2**         | ASUS VivoBook 15 X542UF                     | 15 990             | Intel i7 /                           | 8 GB /                        | SSD -                           | Dedikovaná -                       | 2,3                    | 8               |
| *(ntb2)*       | (*ntb2*)                                    |                    | 4 core                               | DDR 4 /                       | 256 GB                          | NVIDIA                             |                        |                 |
|                |                                             |                    |                                      | 2133 Mhz                      |                                 | GeForce MX130                      |                        |                 |
| **A3**         | Acer Aspire 3 Obsidian Black                | 11 990             | AMD Quad Core Ryzen 5 2500U / 4 core | 8 GB / (Adata)                | SSD -                           | Integrovaná                        | 1,85                   | 8,5             |
| *(ntb3)*       | (ntb3)                                      |                    |                                      | DDR 4 /                       | 256 GB                          |                                    |                        |                 |
|                |                                             |                    |                                      | 2133 Mhz                      |                                 |                                    |                        |                 |
| **A4**         | HP Pavilion 15-cw1005nc Ceramic white       | 16 490             | AMD Ryzen 3 2300U / 4 core           | 8 GB /                        | Hybrid -                        | Dedikovaná -                       | 1,9                    | 9               |
| *(ntb4)*       | (ntb4)                                      |                    |                                      | DDR 4 /                       | HDD / SSD -                     | AMD Radeon RX Vega 6               |                        |                 |
|                |                                             |                    |                                      | 2400 Mhz                      | 1TB + 128 GB                    |                                    |                        |                 |

Tabulka 2: Hodnoty

|    |                        | **A1**                             | **A2**                          | **A3**                               | **A4**                                      |
|    |                        | *(ntb1)*                           | *(ntb2)*                        | *(ntb3)*                             | *(ntb4)*                                    |
|----|------------------------|------------------------------------|---------------------------------|--------------------------------------|---------------------------------------------|
|    | **Notebook**           | Lenovo ThinkPad E580               | ASUS VivoBook 15 X542UF         | Acer Aspire 3 Obsidian Black         | HP Pavilion 15-cw1005nc Ceramic white       |
|    |                        | (*ntb1*)                           | (*ntb2*)                        | (ntb3)                               | (ntb4)                                      |
| K1 | **Cena**               | 18 990                             | 15 990                          | 11 990                               | 16 490                                      |
|    | **(v kč)**             |                                    |                                 |                                      |                                             |
| K2 | **Procesor**           | Intel i5 /                         | Intel i7 /                      | AMD Quad Core Ryzen 5 2500U / 4 core | AMD Ryzen 3 2300U / 4 core                  |
|    |                        | 4 core                             | 4 core                          |                                      |                                             |
| K3 | **RAM**                | 8 GB /                             | 8 GB /                          | 8 GB / (Adata)                       | 8 GB /                                      |
|    |                        | DDR 4 /                            | DDR 4 /                         | DDR 4 /                              | DDR 4 /                                     |
|    |                        | 2400 Mhz                           | 2133 Mhz                        | 2133 Mhz                             | 2400 Mhz                                    |
| K4 | **Disk**               | Hybrid -                           | SSD -                           | SSD -                                | Hybrid -                                    |
|    |                        | HDD / SSD -                        | 256 GB                          | 256 GB                               | HDD / SSD -                                 |
|    |                        | 1TB + 256 GB                       |                                 |                                      | 1TB + 128 GB                                |
| K5 | **Grafika**            | Integrovaná -                      | Dedikovaná -                    | Integrovaná                          | Dedikovaná -                                |
|    |                        | Intel UHD                          | NVIDIA                          |                                      | AMD Radeon RX Vega 6                        |
|    |                        | Graphics 620                       | GeForce MX130                   |                                      |                                             |
| K6 | **Hmotnost**           | 2,1                                | 2,3                             | 1,85                                 | 1,9                                         |
|    | **(v kg)**             |                                    |                                 |                                      |                                             |
| K7 | **Výdrž (v h)**        | 9                                  | 8                               | 8,5                                  | 9                                           |

V Tabulka 3 nalezneme kritéria pro rozhodování. V Tabulka 4 jsou cíle
rozhodování.

Tabulka 3: Kritéria

| **Kritérium** |                                                         |
|---------------|---------------------------------------------------------|
| K1            | **Cena**                                                |
|               | (v Kč)                                                  |
| K2            | **Procesor**                                            |
|               | (výkon v GHz, počet jader, model a výrobce)             |
| K3            | **RAM**                                                 |
|               | (typ paměti, velikost v GB a výkon v MHz)               |
| K4            | **Disk**                                                |
|               | (typ disku, velikost disku)                             |
| K5            | **Grafika**                                             |
|               | (Integrovaná nebo dedikovaná)                           |
| K6            | **Hmotnost**                                            |
|               | (v kg)                                                  |
| K7            | **Výdrž**                                               |
|               | (v h)                                                   |

Tabulka 4: Cíle

| **Kritéria – cíle** |              |
|---------------------|--------------|
| K1                  | Minimalizace |
| K2                  | Maximalizace |
| K3                  | Maximalizace |
| K4                  | Maximalizace |
| K5                  | Maximalizace |
| K6                  | Minimalizace |
| K7                  | Maximalizace |

Tabulka 5: Alternativy

| **Alternativa** | **Model** | **URL**                                     |                                                    |
|-----------------|-----------|---------------------------------------------|----------------------------------------------------|
| A1              | *ntb1*    | Lenovo                                      | <https://www.alza.cz/lenovo-thinkpad-e580>         |
|                 |           | ThinkPad E580                               |                                                    |
| A2              | *ntb2*    | ASUS                                        | <https://www.alza.cz/asus-vivobook-15-f542uq>      |
|                 |           | VivoBook 15 X542UF                          |                                                    |
| A3              | *ntb3*    | Acer                                        | <https://www.alza.cz/acer-aspire-3-obsidian-black> |
|                 |           | Aspire 3 Obsidian Black                     |                                                    |
| A4              | *ntb4*    | HP Pavilion 15-cw1005nc Ceramic white       | <https://www.alza.cz/hp-pavilion-15-c?dq=5615204>  |
|                 |           | (ntb4)                                      |                                                    |

1.  Fullerova metoda (Fullerův trojúhelník)

Je metoda založená na zjišťování počtu preferencí pro každé kritérium vzhledem k
ostatním kritériím souboru.

Postupně se vyplňují políčka od horního levého rohu. Posuzuje se význam kritéria
K1 vzhledem ke všem ostatním kritériím v prvním řádku. Pokud je kritérium
důležitější než kritérium K2, zapíše se hodnota 1. Je-li tomu naopak, zapíše se
0.

Na závěr se stanoví pro každé kritérium počet preferencí fi\* jako součet
jedniček v jednotlivých řádcích uvažovaného kritéria.

Tabulka 6: Fullerova metoda – Kriteriální tabulka

![](media/cef066b5d1dc142c8e2d8159137548f0.png)

Pro každé kritérium byla vypracováno tabulka vztahů a důležitostí jednotlivých
alternativ.

Tabulka 7: Cena (Fullerova metoda)

|    |                 | A1        | A2        | A3        | A4        |                |             |                        |                 |
|----|-----------------|-----------|-----------|-----------|-----------|----------------|-------------|------------------------|-----------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **Preference** | **Váhy**    | **Preference**         | **Váhy**        |
|    |                 |           |           |           |           |                |             | **fi\***               | **wij**         |
| A1 | **ntb 1**       | **x**     | 0         | 0         | 0         | 0              | 0           | 1                      | 0,1             |
| A2 | **ntb 2**       | 1         | **x**     | 0         | 1         | 2              | 0,333333333 | 3                      | 0,3             |
| A3 | **ntb 3**       | 1         | 1         | **x**     | 1         | 3              | 0,5         | 4                      | 0,4             |
| A4 | **ntb 4**       | 1         | 0         | 0         | **x**     | 1              | 0,166666667 | 2                      | 0,2             |
|    |                 |           |           |           | *Suma*    | 6              | 1           | 10                     | 1               |

Tabulka 8: Procesor (Fullerova metoda)

|    |                 | A1        | A2        | A3        | A4        |                |             |                        |                 |
|----|-----------------|-----------|-----------|-----------|-----------|----------------|-------------|------------------------|-----------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **Preference** | **Váhy**    | **Preference**         | **Váhy**        |
|    |                 |           |           |           |           |                |             | **fi\***               | **wij**         |
| A1 | **ntb 1**       | **x**     | 0         | 1         | 1         | 2              | 0,333333333 | 3                      | 0,3             |
| A2 | **ntb 2**       | 1         | **x**     | 1         | 1         | 3              | 0,5         | 4                      | 0,4             |
| A3 | **ntb 3**       | 0         | 0         | **x**     | 0         | 0              | 0           | 1                      | 0,1             |
| A4 | **ntb 4**       | 0         | 0         | 1         | **x**     | 1              | 0,166666667 | 2                      | 0,2             |
|    |                 |           |           |           | *Suma*    | 6              | 1           | 10                     | 1               |

Tabulka 9: RAM (Fullerova metoda)

|    |                 | A1        | A2        | A3        | A4        |                |             |                        |                 |
|----|-----------------|-----------|-----------|-----------|-----------|----------------|-------------|------------------------|-----------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **Preference** | **Váhy**    | **Preference**         | **Váhy**        |
|    |                 |           |           |           |           |                |             | **fi\***               | **wij**         |
| A1 | **ntb 1**       | **x**     | 1         | 1         | 0,5       | 2,5            | 0,416666667 | 3,5                    | 0,35            |
| A2 | **ntb 2**       | 0         | **x**     | 0,5       | 0         | 0,5            | 0,083333333 | 1,5                    | 0,15            |
| A3 | **ntb 3**       | 0         | 0,5       | **x**     | 0         | 0,5            | 0,083333333 | 1,5                    | 0,15            |
| A4 | **ntb 4**       | 0,5       | 1         | 1         | **x**     | 2,5            | 0,416666667 | 3,5                    | 0,35            |
|    |                 |           |           |           | *Suma*    | 6              | 1           | 10                     | 1               |

Tabulka 10: Disk (Fullerova metoda)

|    |                 | A1        | A2        | A3        | A4        |                |             |                        |                 |
|----|-----------------|-----------|-----------|-----------|-----------|----------------|-------------|------------------------|-----------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **Preference** | **Váhy**    | **Preference**         | **Váhy**        |
|    |                 |           |           |           |           |                |             | **fi\***               | **wij**         |
| A1 | **ntb 1**       | **x**     | 1         | 1         | 0,5       | 2,5            | 0,416666667 | 3,5                    | 0,35            |
| A2 | **ntb 2**       | 0         | **x**     | 0,5       | 0         | 0,5            | 0,083333333 | 1,5                    | 0,15            |
| A3 | **ntb 3**       | 0         | 0,5       | **x**     | 0         | 0,5            | 0,083333333 | 1,5                    | 0,15            |
| A4 | **ntb 4**       | 0,5       | 1         | 1         | **x**     | 2,5            | 0,416666667 | 3,5                    | 0,35            |
|    |                 |           |           |           | *Suma*    | 6              | 1           | 10                     | 1               |

Tabulka 11: Grafika (Fullerova metoda)

|    |                 | A1        | A2        | A3        | A4        |                |             |                        |                 |
|----|-----------------|-----------|-----------|-----------|-----------|----------------|-------------|------------------------|-----------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **Preference** | **Váhy**    | **Preference**         | **Váhy**        |
|    |                 |           |           |           |           |                |             | **fi\***               | **wij**         |
| A1 | **ntb 1**       | **x**     | 0         | 1         | 0         | 1              | 0,166666667 | 2                      | 0,2             |
| A2 | **ntb 2**       | 1         | **x**     | 1         | 1         | 3              | 0,5         | 4                      | 0,4             |
| A3 | **ntb 3**       | 0         | 0         | **x**     | 0         | 0              | 0           | 1                      | 0,1             |
| A4 | **ntb 4**       | 1         | 0         | 1         | **x**     | 2              | 0,333333333 | 3                      | 0,3             |
|    |                 |           |           |           | *Suma*    | 6              | 1           | 10                     | 1               |

Tabulka 12: Hmotnost (Fullerova metoda)

|    |                 | A1        | A2        | A3        | A4        |                |             |                        |                 |
|----|-----------------|-----------|-----------|-----------|-----------|----------------|-------------|------------------------|-----------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **Preference** | **Váhy**    | **Preference**         | **Váhy**        |
|    |                 |           |           |           |           |                |             | **fi\***               | **wij**         |
| A1 | **ntb 1**       | **x**     | 1         | 0         | 0         | 1              | 0,166666667 | 2                      | 0,2             |
| A2 | **ntb 2**       | 0         | **x**     | 0         | 0         | 0              | 0           | 1                      | 0,1             |
| A3 | **ntb 3**       | 1         | 1         | **x**     | 1         | 3              | 0,5         | 4                      | 0,4             |
| A4 | **ntb 4**       | 1         | 1         | 0         | **x**     | 2              | 0,333333333 | 3                      | 0,3             |
|    |                 |           |           |           | *Suma*    | 6              | 1           | 10                     | 1               |

Tabulka 13: Výdrž (Fullerova metoda)

|    |                 | A1        | A2        | A3        | A4        |                |             |                        |                 |
|----|-----------------|-----------|-----------|-----------|-----------|----------------|-------------|------------------------|-----------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **Preference** | **Váhy**    | **Preference**         | **Váhy**        |
|    |                 |           |           |           |           |                |             | **fi\***               | **wij**         |
| A1 | **ntb 1**       | **x**     | 1         | 1         | 0,5       | 2,5            | 0,416666667 | 3,5                    | 0,35            |
| A2 | **ntb 2**       | 0         | **x**     | 0         | 0         | 0              | 0           | 1                      | 0,1             |
| A3 | **ntb 3**       | 0         | 1         | **x**     | 0         | 1              | 0,166666667 | 2                      | 0,2             |
| A4 | **ntb 4**       | 0,5       | 1         | 1         | **x**     | 2,5            | 0,416666667 | 3,5                    | 0,35            |
|    |                 |           |           |           | *Suma*    | 6              | 1           | 10                     | 1               |

Tabulka 14: Vyhodnocení (Fullerova metoda)

| **Alternativa**                            | **Hodnota** | **Pořadí** |
|--------------------------------------------|-------------|------------|
| A1 -Lenovo ThinkPad E580                   | 0,242857143 | **3**      |
| A2 - ASUS VivoBook 15 X542UF               | 0,2125      | **4**      |
| A3 - Acer Aspire 3 Obsidian Black          | 0,266071429 | **2**      |
| A4 - HP Pavilion 15-cw1005nc Ceramic white | 0,278571429 | **1**      |
| *Suma*                                     | 1           |            |

[CHART]

Obrázek 2: Fullerova metoda - graf

Pomocí Fullerovy metody byla vybrána jako nejlepší alternativa, podle námi
zvolených kritérií **alternativa 4 (HP Pavilion 15-cw1005nc Ceramic white)**.

1.  Saatyho metoda

Slouží k určení vah kritérií pomocí expertního hodnocení. Na rozdíl od metody
párového srovnávání se však kromě směru preference dvojic kritérií určuje také
velikost této preference, která se vyjadřuje určitým počtem bodů ze zvolené
bodové stupnice.

Pro ohodnocení párových porovnání kritérií je použita 9-ti bodová stupnice, viz
Tabulka 15.

Na základě toho, kolikrát je kritérium významnější než, přiřazujeme prvkům
matice intenzit preferencí S čísla od 1 do 9, jejichž význam je uveden v Tabulce
1.1. Pro jemnější rozlišení preferencí dvojic kritérií se používají hodnoty 2,
4, 6, 8.

Tabulka 15: Saatyho metoda – Jazykové deskriptory

| Počet bodů | Deskriptor                                            |
|------------|-------------------------------------------------------|
| 1          | Kritéria jsou stejně významná                         |
| 3          | První kritérium je slabě významnější než druhé        |
| 5          | První kritérium je dosti významnější než druhé        |
| 7          | První kritérium je prokazatelně významnější než druhé |
| 9          | První kritérium je absolutně významnější než druhé    |

Tabulka 16: Saatyho metoda – Kriteriální tabulka

![](media/e6a65ffbf1b7bd56dede8d8f98d6dcd1.png)

Na základě kriteriální tabulky jsem následně vypracoval jednotlivé porovnání
alternativ k jednotlivým kritériím. Konzistence všech Saatyho matic byla menší
než 0,1 a jsou tedy sestaveny v pořádku a jsou konzistentní.

Tabulka 17: Cena (Saatyho metoda)

|    |                 | A1        | A2        | A3        | A4        |             |                         |
|----|-----------------|-----------|-----------|-----------|-----------|-------------|-------------------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **GEOMEAN** | **Norm.**               |
|    |                 |           |           |           |           |             | **váha**                |
|    |                 |           |           |           |           |             | **wj**                  |
| A1 | **ntb1**        | **1**     | 1/3       | 1/4       | 1/2       | 0,451801002 | 0,092129947             |
| A2 | **ntb2**        | 3         | **1**     | 1/3       | 3         | 1,316074013 | 0,268369986             |
| A3 | **ntb3**        | 4         | 3         | **1**     | 3         | 2,449489743 | 0,499492826             |
| A4 | **ntb4**        | 2         | 1/3       | 1/3       | **1**     | 0,686589048 | 0,140007242             |
|    |                 |           |           |           | *Suma*    | 4,903953806 | 1                       |

Tabulka 18: Procesor (Saatyho metoda)

|    |                 | A1        | A2        | A3        | A4        |             |                         |
|----|-----------------|-----------|-----------|-----------|-----------|-------------|-------------------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **GEOMEAN** | **Norm.**               |
|    |                 |           |           |           |           |             | **váha**                |
|    |                 |           |           |           |           |             | **wj**                  |
| A1 | **ntb1**        | **1**     | 1/3       | 2         | 2         | 1,074569932 | 0,224622374             |
| A2 | **ntb2**        | 3         | **1**     | 4         | 3         | 2,449489743 | 0,512028286             |
| A3 | **ntb3**        | 1/2       | 1/4       | **1**     | 1/2       | 0,5         | 0,104517336             |
| A4 | **ntb4**        | 1/2       | 1/3       | 2         | **1**     | 0,759835686 | 0,158832004             |
|    |                 |           |           |           | *Suma*    | 4,78389536  | 1                       |

Tabulka 19: RAM (Saatyho metoda)

|    |                 | A1        | A2        | A3        | A4        |             |                         |
|----|-----------------|-----------|-----------|-----------|-----------|-------------|-------------------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **GEOMEAN** | **Norm.**               |
|    |                 |           |           |           |           |             | **váha**                |
|    |                 |           |           |           |           |             | **wj**                  |
| A1 | **ntb 1**       | **1**     | 2         | 2         | 1         | 1,414213562 | 0,333333333             |
| A2 | **ntb 2**       | 1/2       | **1**     | 1         | 1/2       | 0,707106781 | 0,166666667             |
| A3 | **ntb 3**       | 1/2       | 1         | **1**     | 1/2       | 0,707106781 | 0,166666667             |
| A4 | **ntb 4**       | 1         | 2         | 2         | **1**     | 1,414213562 | 0,333333333             |
|    |                 |           |           |           | *Suma*    | 4,242640687 | 1                       |

Tabulka 20: Disk (Saatyho metoda)

|    |                 | A1        | A2        | A3        | A4        |             |                         |
|----|-----------------|-----------|-----------|-----------|-----------|-------------|-------------------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **GEOMEAN** | **Norm.**               |
|    |                 |           |           |           |           |             | **váha**                |
|    |                 |           |           |           |           |             | **wj**                  |
| A1 | **ntb 1**       | **1**     | 2         | 2         | 1         | 1,414213562 | 0,333333333             |
| A2 | **ntb 2**       | 1/2       | **1**     | 1         | 1/2       | 0,707106781 | 0,166666667             |
| A3 | **ntb 3**       | 1/2       | 1         | **1**     | 1/2       | 0,707106781 | 0,166666667             |
| A4 | **ntb 4**       | 1         | 2         | 2         | **1**     | 1,414213562 | 0,333333333             |
|    |                 |           |           |           | *Suma*    | 4,242640687 | 1                       |

Tabulka 21: Grafika (Saatyho metoda)

|    |                 | A1        | A2        | A3        | A4        |             |                         |
|----|-----------------|-----------|-----------|-----------|-----------|-------------|-------------------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **GEOMEAN** | **Norm.**               |
|    |                 |           |           |           |           |             | **váha**                |
|    |                 |           |           |           |           |             | **wj**                  |
| A1 | **ntb 1**       | **1**     | 1/3       | 2         | 1/3       | 0,686589048 | 0,142794575             |
| A2 | **ntb 2**       | 3         | **1**     | 4         | 2         | 2,213363839 | 0,460328272             |
| A3 | **ntb 3**       | 1/2       | 1/4       | **1**     | 1/3       | 0,451801002 | 0,093964115             |
| A4 | **ntb 4**       | 3         | 1/2       | 3         | **1**     | 1,456475315 | 0,302913038             |
|    |                 |           |           |           | *Suma*    | 4,808229204 | 1                       |

Tabulka 22: Hmotnost (Saatyho metoda)

|    |                 | A1        | A2        | A3        | A4        |             |                         |
|----|-----------------|-----------|-----------|-----------|-----------|-------------|-------------------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **GEOMEAN** | **Norm.**               |
|    |                 |           |           |           |           |             | **váha**                |
|    |                 |           |           |           |           |             | **wj**                  |
| A1 | **ntb 1**       | **1**     | 2         | 1/2       | 1/2       | 0,840896415 | 0,195262146             |
| A2 | **ntb 2**       | 1/2       | **1**     | 1/2       | 1/2       | 0,594603558 | 0,138071187             |
| A3 | **ntb 3**       | 2         | 2         | **1**     | 2         | 1,681792831 | 0,390524292             |
| A4 | **ntb 4**       | 2         | 2         | 1/2       | **1**     | 1,189207115 | 0,276142375             |
|    |                 |           |           |           | *Suma*    | 4,306499918 | 1                       |

Tabulka 23: Výdrž (Saatyho metoda)

|    |                 | A1        | A2        | A3        | A4        |             |                         |
|----|-----------------|-----------|-----------|-----------|-----------|-------------|-------------------------|
|    | **Alternativa** | **ntb 1** | **ntb 2** | **ntb 3** | **ntb 4** | **GEOMEAN** | **Norm.**               |
|    |                 |           |           |           |           |             | **váha**                |
|    |                 |           |           |           |           |             | **wj**                  |
| A1 | **ntb 1**       | **1**     | 2         | 1         | 1         | 1,189207115 | 0,283277811             |
| A2 | **ntb 2**       | 1/2       | **1**     | 1/2       | 1/2       | 0,594603558 | 0,141638905             |
| A3 | **ntb 3**       | 1         | 2         | **1**     | 1/2       | 1           | 0,238207296             |
| A4 | **ntb 4**       | 1         | 2         | 2         | **1**     | 1,414213562 | 0,336875988             |
|    |                 |           |           |           | *Suma*    | 4,198024235 | 1                       |

Tabulka 24: Přehled vypočtených hodnot (Saatyho matice)

|    |               | λmax   | CI       | CR          | m | RI   |
|----|---------------|--------|----------|-------------|---|------|
| KT | Krit. tabulka | 7,5805 | 0,09675  | 0,073295455 | 7 | 1,32 |
| S1 | Cena          | 4,1596 | 0,0532   | 0,059111111 | 4 | 0,9  |
| S2 | Procesor      | 4,0813 | 0,0271   | 0,030111111 | 4 | 0,9  |
| S3 | RAM           | 4      | 0        | 0           | 4 | 0,9  |
| S4 | Disk          | 4      | 0        | 0           | 4 | 0,9  |
| S5 | Grafika       | 4,0813 | 0,0271   | 0,030111111 | 4 | 0,9  |
| S6 | Hmotnost      | 4,1213 | 0,040433 | 0,044925926 | 4 | 0,9  |
| S7 | Výdrž         | 4,0606 | 0,0202   | 0,022444444 | 4 | 0,9  |

Konzistence všech Saatyho matic byla menší než 0,1 a jsou v pořádku.

-   λmax - Maximální vlastní číslo matice S

-   CI - Index konzistence

-   CR - Konzistenční poměr

-   m – proměnná

-   RI – náhodný konzistenční index

Tabulka 25: Hodnoty RI pro počet m kriterií (podle Whartona)

| **Proměnné** | **Hodnoty** |     |      |      |      |      |      |      |      |
|--------------|-------------|-----|------|------|------|------|------|------|------|
| *m*          | 3           | 4   | 5    | 6    | 7    | 8    | 9    | 10   | 11   |
| **RI**       | 0,58        | 0,9 | 1,12 | 1,24 | 1,32 | 1,41 | 1,45 | 1,49 | 1,51 |

*Zdroj: Křupka Jiří, materiály moodle*

![Obsah obrázku snímek obrazovky Popis byl vytvořen automaticky](media/40a95186e61f95e0447bca2b3549c796.png)

Obrázek 3: Matlab M-file pro výpočet vlastního čísla (Saatyho matice)

Tabulka 26: Vyhodnocení (Saatyho metoda)

| **Alternativa**                            | **Hodnota** | **Pořadí** |
|--------------------------------------------|-------------|------------|
| A1 -Lenovo ThinkPad E580                   | 0,191216    | 4          |
| A2 - ASUS VivoBook 15 X542UF               | 0,230841    | 3          |
| A3 - Acer Aspire 3 Obsidian Black          | 0,342526    | 1          |
| A4 - HP Pavilion 15-cw1005nc Ceramic white | 0,235416    | 2          |
| *Suma*                                     | 1           |            |

[CHART]

Obrázek 4: Saatyho metoda - graf

Nejlepší alternativou je podle námi zvolených kritérií **alternativa 3 - A3 -
Acer Aspire 3 Obsidian Black.**

1.  Analyticko-hierarchický proces

Metoda AHP (Analytic Hierarchy Process) poskytuje rámec pro přípravu účinných
rozhodnutí ve složitých rozhodovacích situacích, pomáhá zjednodušit a zrychlit
přirozený proces rozhodování. Při řešení rozhodovacích problémů je třeba brát v
úvahu všechny prvky, které ovlivňují výsledek analýzy, vazby mezi nimi a
intenzitu s jakou na sebe vzájemně působí.

Tabulka 27: Analyticko-hierarchický proces – vyhodnocení

![](media/f4f9517dd6e9c9bde4f43480adf958e8.png)

Nejlepší alternativou je podle námi zvolených **kritérií alternativa 3 - A3 -
Acer Aspire 3 Obsidian Black.**

Použitá literatura

1.  KŘUPKA, J. et al. *Rozhodovací procesy* [online]. Pardubice: Univerzita
    Pardubice Fakulta ekonomicko-správní, 2012. ISBN 978-80-7395-478-9.

2.  FOTR, Jiří a Lenka ŠVECOVÁ. *Manažerské rozhodování: postupy, metody a
    nástroje*. 2., přeprac. vyd. Praha: Ekopress, 2010. ISBN 9788086929590.

3.  KŘUPKA, Jiří. *Moodle FES – Rozhodovací procesy* [online]. Pardubice:
    Univerzita Pardubice Fakulta ekonomicko-správní.

4.  <https://www.alza.cz/lenovo-thinkpad-e580?dq=5285006>

5.  <https://www.alza.cz/asus-vivobook-15-f542uq?dq=5315934>

6.  <https://www.alza.cz/acer-aspire-3-obsidian-black?dq=5477326>

7.  <https://www.alza.cz/hp-pavilion-15-c?dq=5615204>

    Seznam příloh

Příloha A Excel soubor s výpočty

Příloha B MATLAB M-File s výpočty vlastního čísla

Příloha C Alternativy pro rozhodování – Výběr vhodného notebooku pro studenta

**Příloha C**

**Alternativa 1**

![](media/d120a1a8773c154956388c2d8980597a.png)

**Alternativa 2**

![](media/3b94c292d3ee072b008155a1eeccc402.png)

**Alternativa 3**

![](media/21101463de424d928de697fb9a1f918b.png)

**Alternativa 4**

![Obsah obrázku snímek obrazovky Popis byl vytvořen automaticky](media/1dd2c22b9ee4818882a39e042e55d612.png)
