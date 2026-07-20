# Bijlage 3: Versiehistorie

Hieronder staan de wijzigingen die in deze versie zijn doorgevoerd.

## Catalogus als geheel

De catalogus is omgezet naar het ReSpec-formaat. Hierdoor is de documentstructuur op een aantal punten aangepast en gestandaardiseerd naar de Geonovum-werkwijze:

- ReSpec opmaak met op de voorpagina Geonovum-logo.

- Documenthistorie is conform ReSpec opgenomen in deze bijlage.

- De standaard ReSpec-onderdelen [Samenvatting](#abstract) en [Status van dit document](#sotd) zijn toegevoegd. Deze zijn, zoals gebruikelijk in ReSpec, ongenummerd aanwezig in de inhoudsopgave.

- [Hoofdstuk 1 Inleiding](#inleiding) is één-op-één overgenomen in het gelijknamige onderdeel.

- [Hoofdstuk 2 Informatiemodel op hoofdlijnen](#informatiemodel-op-hoofdlijnen) is overgenomen in het gelijknamige onderdeel. Hieraan is het stukje inleidende tekst uit het oude hoofdstuk 3 ‘Informatiemodel in detail’ toegevoegd als [par. 2.3](#informatiemodel-in-detail), ter inleiding op het nieuwe onderdeel 3 ‘Gegevensdefinitie’.

- Het nieuwe [hoofdstuk 3 Gegevensdefinitie](#cat) is een samenvoeging van de oude hoofdstukken ‘3 Informatiemodel in detail’, ‘4 Objecttypen’ en ‘3 Attribuut- en relatiesoorten’. Dit is conform de Geonovum-werkwijze.

- Hoofdstuk ‘6 Waardenlijsten’ keert terug in het nieuwe [hoofdstuk 4 Inhoud van de waardelijsten](#lis). Hierbij worden eerst de referentielijsten getoond, vervolgens de enumeraties. Vanwege de manier waarop de catalogus wordt gegenereerd, is de ‘Waardenlijsten-view’ verplaatst naar [par. 3.15 Waardelijsten view - overzicht](#EAID_8279DB6D_9353_4fcc_A31C_787591A2C257). De referentielijsten zijn ook opgenomen als [par. 3.18 Referentielijsten](#referentielijsten). Daar worden zowel metagegevens (niet in onderdeel 4) en de structuur (ook in onderdeel 4) opgesomd. Een lijst met enumeraties en hun omschrijvingen is opgenomen in [par. 3.21 Enumeraties](#enumeraties).

- Hoofdstuk ‘7 Gestructureerde datatypen’ is opgenomen in [par. 3.20 Gestructureerde datatypen](#gestructureerde-datatypen).

- Bijlage 1: Overzicht views met ‘kern-objecttypen’ is één-op-éen overgenomen in [Bijlage 1: Overzicht met ‘kern-objecttypen'](#bijlage-1-overzicht-met-kern-objecttypen).

- Bijlage 2: Gerefereerde bronnen is één-op-éen overgenomen in [Bijlage 2: Gerefereerde bronnen](#bijlage-2-gerefereerde-bronnen). De diverse open punten (gemarkeerd met “[…]”) worden in een toekomstige versie opgelost.

- Conform ReSpec sluit de catalogus af met een [Lijst met figuren](#tof) en [Referenties](#references).

** Overige wijzigingen

## In paragraaf 3.22 Attribuut- en relatiesoort details

- Inconsistenties in relatieklassen (veldnamen en lege velden) zijn gecorrigeerd en afgestemd op de ReSpec-structuur.

- Als een objecttype meerdere relaties had met dezelfde naam, dan is deze naam uitgebreid om de namen van de relaties per objecttype uniek te maken. Bijv. de relatie tussen ‘Bevinding’ en ‘Specifiek voorschrift’ met de relatienaam ‘betreft’ heeft nu de relatienaam ‘betreft specifiek voorschrift’ gekregen.

- Waar mogelijk zijn opgenomen URL’s die niet als hyperlink functioneerden, nu als werkende hyperlink opgenomen.

- Als op een attribuutsoort een waardelijst van toepassing is, hetzij een enumeratie of hetzij een referentielijst, dan is het metagegeven ‘Patroon’ nu consequent ingevuld met ‘[waardelijst]’.

- In de gevallen waar in versie 1.0.0 het metagegeven ‘Patroon’ aanvullende informatie bevatte, is die informatie verplaatst naar het metagegeven ‘Toelichting’.

- De termen ‘waardelijst’ en ‘waardenlijst’ kwamen beide voor. Nu wordt alleen nog maar de term ‘waardelijst’ gebruikt (conform de naamgeving in het gehanteerde metamodel voor informatiemodellering, MIM).

- Tenslotte zijn de volgende wijzigingen doorgevoerd:

| **Github issue**                                        | **Soort wijziging**                  | **Wijziging**                                                                           |
|-------------------------------------------------------- | ------------------------------------ | --------------------------------------------------------------------------------------- |
|[11](https://github.com/Geonovum/vth-cim-flo/issues/11)  | Waardelijst benoemd                  | Bij de attribuutsoort Land van het objecttype Adres buitenland (par. 3.22.2.1.4) is toegevoegd dat hiervoor als waardelijst gebruikt wordt: Tabel 34 Landentabel van de Rijksdienst voor Identiteitsgegevens (Rv­IG).|
|[12](https://github.com/Geonovum/vth-cim-flo/issues/12)  | Diagram aangepast                    | Bij de attribuutsoort Regeltekstidentificatie van het objecttype Algemeen verbindend voorschrift (par. 3.22.1.6.1) is het metagegeven 'Patroon' gewijzigd van 'wId: [bevoegd_gezag]\_[versienummer]\__[prefix]\__)[element_ref](_[nummer]' naar 'wId: [bevoegd_gezag]\_[versienummer]\__[eId]'.|
|[49](https://github.com/Geonovum/vth-cim-flo/issues/49)  | Diagram aangepast                    | Bij de relatiesoort Activiteituitvoering wordt gedaan door betrokkene (par. 3.22.1.4.12) is de 'indicatie kardinaliteit bron' gewijzigd van 0..1 naar 0..*. Dit betekent dat de activiteituitvoering niet wordt gedaan door maximaal één betrokkene, maar dat dit meerdere betrokkenen kunnen zijn. |
