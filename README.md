# NVE Hydro Calculator Pro v4

En kalkulator for å beregne hva som skjer hvis en dam brister.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-4.0-green.svg)

## Hva er dette?

Når en dam brister, strømmer store mengder vann ut på kort tid. Dette kan føre til flom nedstrøms som truer liv og eiendom. For å planlegge sikkerhet og beredskap trenger ingeniører å vite:

- **Hvor mye vann** strømmer ut?
- **Hvor raskt** utvikler bruddet seg?
- **Hvor stort** blir hullet i dammen?

Denne kalkulatoren svarer på disse spørsmålene ved hjelp av anerkjente formler fra NVE (Norges vassdrags- og energidirektorat) og internasjonal forskning.

## Hvem er dette for?

- Damsikkerhetsansvarlige
- Hydrologer og sivilingeniører
- Kommunal beredskap
- Studenter innen vannressurser

## Hovedfunksjoner

### 🌊 Bruddberegning
Beregner hvor stort hullet i dammen blir og hvor mye vann som renner ut per sekund.

### 📊 Tidssimulering
Viser hvordan vannstanden og vannføringen endrer seg minutt for minutt gjennom hele bruddhendelsen.

### 🔄 Scenariosammenligning
Lag flere "hva hvis"-scenarioer og sammenlign resultatene side om side.

### 📁 Eksport
Last ned resultatene som Excel-regneark, Word-rapport eller datafil (JSON).

## Slik fungerer det

### Input - hva du må vite om dammen

| Du trenger | Eksempel | Forklaring |
|------------|----------|------------|
| Vannvolum | 2.5 Mm³ | Hvor mye vann magasinet holder |
| Damhøyde | 15 m | Høyden fra bunn til topp av dammen |
| Damkote | 850 moh. | Hvor høyt damkronen ligger over havet |

### Output - hva kalkulatoren forteller deg

| Du får vite | Eksempel | Forklaring |
|-------------|----------|------------|
| Bruddbredde | 45 m | Hvor bredt hullet i dammen blir |
| Bruddutviklingstid | 1.2 timer | Hvor lang tid det tar før bruddet er ferdig utviklet |
| Maksimal vannføring | 850 m³/s | Den største vannmengden som strømmer ut per sekund |

## Tekniske detaljer

### Bruddform

Kalkulatoren antar at bruddet får en **trapesform** - bredere i toppen enn i bunnen. Dette er realistisk for fyllingsdammer der vannet graver seg nedover og utover samtidig.

```
    ←───── Toppbredde ─────→
    \                      /
     \                    /
      \                  /
       ←─ Bunnbredde ─→
```

### Flomløp (spillway)

Mange dammer har et flomløp - en kontrollert "nødutgang" for vann ved høy vannstand. Kalkulatoren kan ta hensyn til dette, inkludert om flomløpet er delvis blokkert av drivgods (trær, is, etc.).

### Formler

Beregningene bygger på:
- **Froehlich (1995)** - Internasjonal standard for bruddparametere
- **NVE Veileder 2/2022** - Norske retningslinjer for damsikkerhet
- **Overløpslikninger** - Fysikk for vannstrømning over kanter

## Kom i gang

### Bruk direkte i nettleser
1. Last ned `NVE-Hydro-Calculator-Pro-v4.html`
2. Åpne filen i Chrome, Firefox eller Edge
3. Fyll inn verdiene for din dam
4. Klikk "Beregn"

Ingen installasjon nødvendig!

## Begrensninger

- Beregningene er forenklede estimater, ikke eksakte forutsigelser
- Forutsetter fyllingsdammer (jord/stein), ikke betongdammer
- Tar ikke hensyn til terreng nedstrøms
- Bør brukes sammen med faglig skjønn

## Eksempel

**Scenario:** Liten fyllingsdam i fjellet

| Parameter | Verdi |
|-----------|-------|
| Vannvolum | 0.5 Mm³ |
| Damhøyde | 8 m |
| Bruddtype | Overtopping |

**Resultat:**
- Bruddbredde: ~20 m
- Bruddutviklingstid: ~0.5 timer
- Maks vannføring: ~150 m³/s

## Lisens

MIT License - Fri bruk, også kommersielt.

## Referanser

- [NVE - Damsikkerhet](https://www.nve.no/energi/tilsyn/damsikkerhet/)
- Froehlich, D.C. (1995) - "Peak Outflow from Breached Embankment Dam"
- NVE Veileder 2/2022

## Tilbakemelding

Fant du en feil? Har du forslag til forbedringer? Opprett en [issue](../../issues) eller send en pull request.

Disclaimer: Kunstig intelligens er brukt til opprettelse av programmet, og denne teksten.
