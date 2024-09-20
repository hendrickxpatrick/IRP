# Account Compromised Playbook

[[_TOC_]]

## Scope
Dit draaiboek beschrijft de stappen die moeten worden genomen wanneer accounts zijn gecompromitteerd. Natuurlijk moeten we ook de hosts waar deze accounts zijn gebruikt, herstellen. 

## 1. Voorbereiding

<details>
<summary>Expand/Colapse</summary>

- Maak en onderhoud een lijst van:
    - alle domeinen die eigendom zijn van het bedrijf.
        - Dit kan voorkomen dat je acties onderneemt tegen onze eigen domeinen.
    - alle mensen die domeinen kunnen registreren.
- Maak e-mailsjablonen:
    - om alle medewerkers te informeren over lopende phishingcampagnes tegen de organisatie.
    - om hostingbedrijven te contacteren voor het neerhalen van domein(en).
    - om derden te informeren om actie te ondernemen tegen phishing op hun infrastructuur (Microsoft, Fedex, Apple, enz.).
- Zorg ervoor dat:
    - Mail anti-malware/anti-spam/anti-phish oplossingen aanwezig zijn.
    - Gebruikers weten hoe ze phishing kunnen melden.
    - Detectie bestaat voor Office-documenten die processen starten.
        - PowerShell
        - CMD
        - WMI
        - MSHTA
        - Etc.
- Voer een oefening uit om ervoor te zorgen dat alle aspecten van het draaiboek werken:
    - Na publicatie.
    - Minstens één keer per jaar.
    - Test/Valideer:
        - Interne contact- en escalatiepaden.
- Beoordeel dreigingsinformatie voor:
    - bedreigingen voor de organisatie,
    - merken en de sector,
    - gemeenschappelijke patronen,
    - nieuw ontwikkelende risico's en kwetsbaarheden.
- Zorg voor de juiste toegang tot alle benodigde documentatie en informatie, inclusief toegang buiten kantooruren, voor de volgende:
    - IR Draaiboeken.
    - Netwerkarchitectuurdiagram.
    - Gegevensstroom.
    - Identificeer en verkrijg de diensten van een derde partij Cyber Forensic provider.
- Definieer dreigings- en risicofactoren en waarschuwingspatronen binnen de beveiligingsinformatie- en gebeurtenisbeheer (SIEM) oplossing van de organisatie.

### Train Medewerkers
- Voer regelmatig bewustwordingscampagnes uit om de informatiebeveiligingsrisico's voor medewerkers te benadrukken, waaronder:
    - Phishing-aanvallen en kwaadaardige e-mails;
    - Ransomware;
    - Het melden van een vermoedelijk cyberincident.
### Toegang tot en voorziening van tools

### Tool1
(../Products/TOOL.md)

### Tool2
(../Products/TOOL.md)

### Lijst van activa
- Er moet een lijst van activa en eigenaren bestaan en beschikbaar zijn voor de volgende:
    - Klantenactiva
    - Eigenaren
    - Contacten
    - Vooraf geautoriseerde acties
- Bedrijfsactiva (inclusief alle filialen en bedrijfseenheden)
    - Eigenaren
    - Contacten
    - Beheerders
- Vooraf geautoriseerde acties
    - Type activa-inventaris die nodig is:
    - Eindpunten
    - Servers
    - Netwerkapparatuur
    - Beveiligingsapparaten
    - Netwerkbereiken
        - Publiek
        - Privé
        - VPN / Out of Band
            - Medewerkers
            - Partners
            - Klanten
</details>

## 2. Detecteren
<details>
<summary>Expand/Colapse</summary>

### Workflow
<details open>
<summary>Expand/Colapse</summary>

![AccountCompromised Workflow](Workflows/AccountCompromised-Workflow-Detect.png)

</details>

### Identify Threat Indicators
<details open>
<summary>Expand/Colapse</summary>

#### Alerts
Waarschuwingen worden gegenereerd door verschillende systemen die eigendom zijn van het Security/SOC-team. De belangrijkste bronnen voor waarschuwingen zijn:
    - Tickets
    - SIEM
    - Anti-Virus / EDR
    - Rapporten
    - DNS
    - Fouten van mailservers

#### Meldingen
Meldingen komen van externe bronnen, meestal via e-mail, Teams of telefoon. De belangrijkste bronnen voor meldingen zijn:

- Gebruikers (intern)
- Ontvangers van e-mails (extern)
- Derden
- ISP
- Mailproviders

</details>

### Indentify Risks Factors
<details open>
<summary>Expand/Colapse</summary>

#### Algemeen
- Diefstal van inloggegevens
- Malwarelevering
- Criminele activiteiten
- Chantage / Losgeld

#### Bedrijfsspecifiek
- Financiële verliezen
    - Verlies van contract
    - Contract niet verlengd
    - Lagere bieding aan onze klanten
    - Boetes
        - Regelgeving

</details>

### Data Colletion
Deze sectie beschrijft de informatie die moet worden verzameld en gedocumenteerd over het incident. Er zijn veel bronnen om je te helpen met die fase Er is een externe koppeling verwijderd om uw privacy te beschermen..[here](../Tools/README.md)
<details open>
<summary>Expand/Colapse</summary>
Domeinen
- Reputatie
- Registrar
- Eigenaar
- IP
- Meerstaps / Doorverwijzing
- Technologieën van de site 
- WordPress
- Joomla
- Aangepaste pagina (inloggegevens phish)

IP
- Reputatie
- Eigenaar
- Geolocatie
- Andere domeinen op dat IP

</detials>

### Categoriseren
<details open>
<summary>Expand/Colapse</summary>

Determine type of 


</details>

### Triage 
<details open>
<summary>Expand/Colapse</summary>

Bepaal
- Impact
- Van
- Financieel
- Gegevensverlies
- Omvang (Aantal mensen)

</details>
</details>
</details>

## 3. Analyze
<details open>
<summary>Expand/Colapse</summary>

### Workflow
<details open>
<summary>Expand/Colapse</summary>

![AccountCompromised Workflow](Workflows/AccountCompromised-Workflow-Analyze.png)

</details>

### AA1. Verify
<details open>
<summary>Expand/Colapse</summary>

In conjonction with a senior member of the SOC  
- Double check previous data
- Rule out False Positive

</details>

### AA2. List Compromised Credentials
<details open>
<summary>Expand/Colapse</summary>

In the Compromised Assets TAB of the Event Log list:   
- Compromised accounts
- Compromised machines
- Compromised domains

</details>

### AA3. Level of Access / Priviledges
<details open>
<summary>Expand/Colapse</summary>

In conjonction with a senior member of the SOC  
- Double check previous data
- Rule out False Positive

</details>

### Update Scope
<details open>
<summary>Expand/Colapse</summary>

- Update lists of
    - affected endpoints
    - affected Company Entities
    - affected clients

</details>

### Scope Validation
<details open>
<summary>Expand/Colapse</summary>

Have all the machines been identified? 
If you find futher traces of phishing or new IOCs go back through this step.  

When you are done identifying all compromised:  
- Hosts

And investigated all:  
- URLs
- Domains
- IP
- Ports
- Files
- Hash

Go to the next phase <Contain/Eradicate>

</details>

</details>


## 4. Contain / Eradicate
<details open>
<summary>Expand/Colapse</summary>

### Workflow
<details open>
<summary>Expand/Colapse</summary>

![AccountCompromised Workflow](Workflows/AccountCompromised-Workflow-Contain_Eradicate.png)

</details>

### Block
<details open>
<summary>Expand/Colapse</summary>

- Update FW, Proxy, etc. rules
- Blackhole DNS
- Submit to Partners
    - AV/EDR Vendor
    - Web Filter Vendor
    - etc.

</details>

### Validate User's Actions
<details open>
<summary>Expand/Colapse</summary>



</details>

### Malware Infection?
<details open>
<summary>Expand/Colapse</summary>

If there was malicious attachments that were openned we need to assume the endpoint(s) was/were infected by a malware.  
Please continue to the [Malware Playbook](../IRP-Malware/README.md)  

</details>


### Close Monitoring
<details open>
<summary>Expand/Colapse</summary>

- Monitor for 
    - Related incoming messages
    - Internet connections to IOC
    - New files that matches hashes identified

</details>


### All Affected Endpoints Contained?
<details open>
<summary>Expand/Colapse</summary>

If all affected endpoints have been contained, you can go to the next phase, otherwise continue bellow.  

</details>

### New IOC Discovered?
<details open>
<summary>Expand/Colapse</summary>

If there was new IOC discovered, go back to the [Analyze Phase](README.md#3-analyze)
</details>
</details>

## 5. Recover
<details open>
<summary>Expand/Colapse</summary>

### Workflow
<details open>
<summary>Expand/Colapse</summary>

![AccountCompromised Workflow](Workflows/AccountCompromised-Workflow-Recover.png)

</details>

### Update Defenses
<details open>
<summary>Expand/Colapse</summary>

Determine which of the following rules needs to be removed and which needs to stay in the following list:  
- Firewall Rules
- EDR 
    - ban hashes
    - ban domains
    - Containment
- Proxy Block

</details>

### All Affected Endpoints Recovered?
<details open>
<summary>Expand/Colapse</summary>

If all affected endpoints have been contained, you can go to the next phase, otherwise continue bellow.  

</details>

### Validate Countermeasures
<details open>
<summary>Expand/Colapse</summary>

Determine if legitimate elements are blocked by:  
- Proxy
- Firewall
- EDR

If so, go back to [Update Defenses](README.md#update-defenses)
Otherwise go to the next phase <Post Incident>

</details>
</details>

## 6. Post Incident
<details>
<summary>Expand/Colapse</summary>

### Workflow
<details open>
<summary>Expand/Colapse</summary>

![AccountCompromised Workflow](Workflows/AccountCompromised-Workflow-Post_Incident.png)

</details>

### Incident Review
<details open>
<summary>Expand/Colapse</summary>

- What worked
- What didn't work

</details>

### Update Mode of Operations
<details open>
<summary>Expand/Colapse</summary>

Update the following documents as requiered:  
- Policies
- Processes
- Procedures
- Playbooks
- Runbooks

Update Detetion Rules in:  
- SIEM
- Anti-Spam
- Malware Gataway
- EDR
- Other security solution

</details>

### Review Defensive Posture
<details open>
<summary>Expand/Colapse</summary>

- Schedule review of newly introduced rules in6 months
- Are the following still applicatble
    - Firewall Rules
    - Proxy Rules for C2
    - AV / EDR custom Signatures
    - IPS Signatures

</details>

### User Awareness Training
<details open>
<summary>Expand/Colapse</summary>


</details>

</details>

# References

This Playbook was built using the following references:  
https://www.dfir.training/index.php?option=com_jreviews&format=ajax&url=media/download&m=14tt1&1600804844570  
https://www.gov.scot/publications/cyber-resilience-incident-management/  
https://github.com/certsocietegenerale/IRM/tree/master/EN  
https://www.incidentresponse.com/playbooks/  
https://ayehu.com/cyber-security-incident-response-automation/top-5-cyber-security-incident-response-playbooks/  
https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf  
