---
source-git-commit: 58ccef353b492b1c2adfbb8c2471e1f92263e6e4
translation-type: tm+mt

---
# Instructies

**Opmerking: Deze pagina (of een willekeurige pagina readme.md) zal niet publiceren naar de klant die documentatie onder ogen ziet**

## Inhoudsopgave

+ `TOC.md` bij de wortel van de gebruikersgids verstrekt de organisatie van de onderwerpen die in de gids voor deze oplossing bevat zijn.
+ Elke gebruikersgids zal het hebben uniek `TOC.md`, waarin u alle pagina&#39;s/onderwerpen kunt tot zonodig opdracht geven.
+ De eerste pagina van alle gebruikershandleidingen is `overview.md`.

## Handboek

+ De inleiding tot de gebruikersgids wordt geroepen `overview.md`
+ Elk onderwerp in de gebruikersgids heeft het zijn eigen verschillende folder.
   + Als er een onderwerp in de gids genoemd *Implementatie* is, is de overeenkomstige folder `/implementation`
+ Alle afbeeldingselementen worden in de `/assets` hoofdmap van de gebruikershandleiding opgeslagen.
   + Alle afbeeldingen in de `/assets` map worden gelokaliseerd.
   + Afbeeldingen in de `/no-localize` directory worden niet gelokaliseerd (dat is een verrassing!). Dit kan worden gebruikt om er in lokale versies voor te zorgen dat specifieke elementen niet onnodig worden gereproduceerd.

## Metagegevens gebruikersgids Niveau

+ Metagegevens die de gebruikershandleiding beschrijven, worden opgeslagen in de `TOC.md`. Dit omvat:
   + product - naam van product/capaciteit.
   + cloud - cloud waartoe dit product behoort.
   + publiek - publiek of archetype waarop de gids is gericht.
   + gebruikershandleiding - naam van de gebruikershandleiding.

## Metagegevens paginaniveau

+ Metagegevens die nodig zijn om een document te beschrijven, worden opgeslagen als onderdeel van elke afzonderlijke pagina. Dit omvat:
   + titel - titel van de pagina.
   + beschrijving - beschrijving van de pagina.
   + tweede titel - tweede alternatieve titel.
   + seo-description - alternatieve titel voor SEO-doeleinden.
   + korte titel - (optioneel veld).
   + Met index - ja/nee - wordt de pagina geïndexeerd door het zoekplatform van Adobe.
   + vertalen - ja / nee - zal deze pagina worden gelokaliseerd .
   + versie - vooral gebruikt voor AEM en Campagne, om de versie van het product aan te duiden.
   + private-feature-pack - voornamelijk gebruikt voor AEM.
   + bèta - is dit product in bèta?
   + omleiding - kan worden gebruikt om een verwijzing naar een nieuwe pagina tot stand te brengen als dat wordt vereist.
   + doc-type: referentie (standaard) / problemen oplossen / ontwikkelaar / zelfstudie / kb / whitepaper.

## Meer informatie

Voor meer publicatieinstructies, stijlgidsen, steekproeven en andere middelen, gelieve te bezoeken de [Samenwerken Documentatie Repo](https://git.corp.adobe.com/AdobeDocs/collaborative-doc-instructions)
