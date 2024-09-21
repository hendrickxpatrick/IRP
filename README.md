# Table of Content
[[_TOC_]]

# IR Playbooks
Dit repository bevat alle Incident Response Playbooks en Workflows van het SOC van het bedrijf.

Elke map bevat een Playbook dat is onderverdeeld in 6 secties volgens [NIST - 800.61 r2](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf)

## 1- Voorbereiding

Deze sectie moet de volgende informatie bevatten:
- Lijst van ALLE activa
- Servers
- Eindpunten (+kritieke)
- Netwerken
- Applicaties
- Werknemers
- Beveiligingsproducten
- Baselines
- Communicatieplan
- Welke beveiligingsevenementen
- Drempels
- Hoe toegang te krijgen tot beveiligingstools
- Hoe toegang te verlenen
- Playbooks maken
- Oefeningen plannen
- Table Top
- Hands On

## 2- Detectie en Analyse
Deze sectie moet de volgende informatie bevatten:
- Geïsoleerde getroffen systemen
- Patch Threat Entry Point
- Vooraf gedefinieerde drempel
- Voor klanten
- Voor interne systemen
- Voor escalaties
- Vooraf geautoriseerde acties
- Per klanten
- Per omgeving
- Prod
- QA
- Internet Facing
- Hoe de dreiging op alle getroffen systemen te verwijderen
- Systemen operationeel krijgen
- Herbouwen en hervatten van de service
  
## 3- Containment, Eradication en Herstel
Deze sectie moet de volgende informatie bevatten:
- Geïsoleerde getroffen systemen
- Patch Threat Entry Point
- Vooraf gedefinieerde drempel
- Voor klanten
- Voor interne systemen
- Voor escalaties
- Vooraf geautoriseerde acties
- Per klanten
- Per omgeving
- Prod
- QA
- Internet Facing
- Hoe de dreiging op alle getroffen systemen te verwijderen
- Systemen operationeel krijgen
- Herbouwen en hervatten van de service

## 4- Post-Incident Activiteit
- Lessen geleerd
- Nieuwe detectie
- Nieuwe verharding
- Nieuw patchbeheer
- enz.
 
# Directory Structuren
## Klanten
- Contacten
    - Namen
    - Telefoonnummer
    - E-mail
- Escalatiepunt
    - Kantooruren
    - Buiten kantooruren
- Accountmanager
- Vooraf goedgekeurde acties en drempel
- Blackout / Brownout schema

## Producten
Deze map bevat informatie over de verschillende "commerciële" producten die we gebruiken tijdens een incident. Bijvoorbeeld:

- JIRA
- Microsoft ATP
- Fortigate
- enz.

## IRP-*
Dit zijn de individuele mappen die de Playbooks zelf bevatten. Binnen elke directory moet er een PDF-map zijn waar een PDF-versie beschikbaar is (en automatisch gegenereerd) voor auditors en klanten die deze willen zien.
