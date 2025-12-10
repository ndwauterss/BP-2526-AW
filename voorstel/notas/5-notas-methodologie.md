# Fase 5. Methodologie

- **Werktitel onderzoeksvoorstel:** Optimalisatie van Azure Functions: van Dedicated Plan naar Premium plan of hosting op Azure Container Apps
- **Student 1:** Wauters, Andy, TIAO
- **URL Github repo:** <https://github.com/HoGentTIN/paper-research-methods-nl-24-25-rmwauters>

## Plan van aanpak

- **Fase 1: Requirementsanalyse**
    - **Doelstelling:** Een antwoord op de volgende deelvragen:
        - Wat zijn de beperkingen van de huidige Azure Functions met Dedicated plan in termen van kosten, schaalbaarheid en prestaties en welke prestatieproblemen treden er op bij een hoge belasting?
        - Wat maakt de huidige Azure Functions dynamisch en welke architecturale en technische factoren zijn hierbij belangrijk?
        - Aan welke eisen moet een nieuwe oplossing voldoen op vlak van kosten, schaalbaarheid en prestaties om als succesvol aanzien te worden? 
    - **Aanpak:**
        - Analyse huidig systeem
        - Interview met CTO belanghebbenden 
    - **Resultaat, deliverable(s):** Requirementslijst
- **Fase 2: Literatuurstudie**
    - **Doelstelling:** Een antwoord op de volgende deelvraag: "Wat zijn de belangrijkste technische verschillen in schaalbaarheid, kostenstructuur en prestaties tussen Azure Functions met Dedicated plan en het Premium plan of Azure Container Apps?".
    - **Aanpak:**
        - Literatuurstudie
        - Opvolgmeetings om longlist en shortlist te bespreken en een stand van zaken mee te geven. 
    - **Resultaat, deliverable(s):** Longlist en shortlist alternatieven
- **Fase 3: Proof-of-Concept**
    - **Doelstelling:** Een antwoord op de volgende deelvraag: "Wat zijn de architecturale overwegingen en uitdagingen bij een migratie van Dedicated plan naar het Premium plan of Azure Container Apps?".
    - **Aanpak:**
        - Opzetten testomgeving
        - Opzetten testscenario's
        - Maken van scripts en commando's voor automatisering benchmarks
        - Benchmarking van schaalbaarheid, prestaties en kosten in verschillende scenario's en omgevingen 
    - **Resultaat, deliverable(s):** CSV met resultaten, proefopstelling, scripts/commando's
- **Fase 4: Verwerking resultaten**
    - **Doelstelling:** Een antwoord op de volgende deelvraag: "Welke impact heeft een migratie van Azure Functions met Dedicated plan naar Premium plan en Azure Container Apps op de prestaties, kosten en schaalbaarheid bij een dynamische belasting en wat is de superieure oplossing in deze context?".
    - **Aanpak:**
        - Analyse resultaten
        - Datavisualisatie door python
        - Statistische testen
    - **Resultaat, deliverable(s):** Advies, best practices, datavisualisatie

## Verloop

Gebruik (een) Mermaid-diagram(men) om de stappen of het tijdverloop de visualiseren (flowchart en/of Gantt-diagram; zie instructies).

```mermaid
gantt
    title Planning BP-onderzoek
    dateFormat  YYYY-MM-DD
    tickInterval 1week
    weekday monday
    todayMarker off

    section Schrijven onderzoeksvoorstel
    Onderzoeksvoorstel v1        :prop1, 2025-11-28, 2w
    Onderzoeksidee pitchen       :milestone, 2025-12-02, 0d
    Indienen v1                  :crit, 2025-12-12, 1d
    Feedback promotor            :milestone, 2026-01-09, 0d
    Onderzoeksvoorstel v2        :prop2, 2026-01-09, 2w
    Indienen v2                  :crit, 2026-01-23, 1d

    section Requirement-analyse
    Requirement-analyse          :a1, 2025-12-15, 4w
    Requirements-lijst v1 + gebruiksrapporten       :milestone, 2025-12-29,0d
    Requirements-lijst v2        :milestone, 2026-01-12,0d

    section Literatuuroderzoek
    Literatuurstudie             :lit1, 2025-12-15, 20w

    section Proof-of-Concept
    PoC                          :2026-02-23, 10w
    Testscenario's               :milestone, 2026-03-02, 0d
    Testomgevingen               :milestone, 2026-03-16, 0d
    Experimenten                 :milestone, 2026-04-06, 0d

    section Resultaten verwerken
    Analyse resultaten           :2026-04-06, 4w

    section Schrijven aan bachelor proef
    BP schrijven                 :2026-01-26, 17w
    Inleiding                    :milestone, 2026-02-09, 0d
    Methodologie                 :milestone, 2026-02-23, 0d
    Experimenten + resultaten    :milestone, 2026-05-04, 0d
    Draft BP indienen            :crit, draftbp, 2026-03-02, 1d
    Feedback promotor            :milestone, 2026-03-11, 0d
    Feedback verwerken           :2026-03-11, 4w
    Finale draft BP indienen     :crit, finalbp, 2026-05-04, 1d
    Bachelorproef indienen       :crit, bp, 2026-05-29, 1d

    section Meetings belanghebbenden
    Eerste interview CTO         :milestone, meet1, 2025-10-22, 0d
    Opvolgmeeting                :milestone, 2025-12-29, 0d
    Opvolgmeeting                :milestone, 2026-01-23, 0d
    Opvolgmeeting                :milestone, 2026-03-02, 0d
    Opvolgmeeting                :milestone, 2026-04-20, 0d
    Finale meeting               :milestone, 2026-05-22, 0d
```