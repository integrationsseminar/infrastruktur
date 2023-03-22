# Infrastruktur und DevOps Team - Projekt TROMEGA
Dies ist das Repository des Infrastruktur und DevOps Teams des Projekt TROMEGA. In diesem Repository wird auch das Deployment diverser anderer Uniprojekte verwaltet, lasst euch also nicht überraschen, wenn euch in den hosting files etwas über den Weg läuft, das nicht nach TROMEGA aussieht :)


## Helpdesk
Für Fragen, Bug-Reports, Feature requests und das Hinzufügen von Environment Variablen in die Produktionsumgebung, öffnet bitte ein Issue. Wir versuchen, eure Anfrage so schnell wie möglich zu bearbeiten. 

## Übersicht über den Projektbeitrag
### Prozesse
Ganz im Sinne des ersten DevOps Weges haben wir direkt zu Beginn des Projekts Prozesse entwickelt, um die Developer Experience des Projekts zu maximieren und unnötige Arbeit, beispielsweise durch das Lösen von großen Mergekonflikten zu minimieren. Der Entwicklungsprozess des Projekt TROMEGA ist an das [Trunk-based Development](https://cloud.google.com/architecture/devops/devops-tech-trunk-based-development?hl=de) angelehnt. Im speziellen wird ein Branch-per-Issue Ansatz verfolgt. Das bedeutet, dass alle Aufgaben in möglichst kleine in sich zusammenhängende Arbeitspakete aufgespalten werden, die jeweils durch ein eigenes Issue im GitHub Project Board repräsentiert werden. Für die Bearbeitung jedes Issues wird ein eigener Branch erstellt und nach Abschluss der Arbeitspaketes in den main-Branch gemerged. So werden große Merge-Konflikte verhindert und gleichzeitig eine hohe Aktualität des main-Branches gewährleistet.
  
### CI/CD Pipelines
Um den Flow zwischen Entwicklung und IT-Operations zu optimieren, haben wir uns entschieden, eine Reihe an Automatisierungen im Bereich des Continous Integration (CI) und Continous Deployment (CD) zu implementieren. Unter dem Einsatz von GitHub Actions entstanden unter anderem Pipelines, die alle Schritte vom merge in den Main-Branch bis zum Starten der neuen Applikationsversion auf dem Linux-Server vollautomatisiert ausführen. Weiterhin haben wir durch das Einführen von Merge Requirements versucht, von Anfang an eine hohe Code Qualität forcieren. Zu den Merge Requirements zählen unter anderem das Ausführen automatisierter Unit-Tests und die Überprüfung der Test-Coverage. 

### Hosting
Das Backend des Projekt TROMEGA sowie eine Web-Version des Flutter Frontends wird auf einer Linux-VM unter der Domain (api.)fitnessapp.gang-of-fork.de gehostet. Die Services laufen dabei jeweils in einem Docker-Container und werden mit Hilfe eines Traefik Reverse-Proxy über das Netzwerk erreichbar gemacht.
### Monitoring
### Logging


## Links zu den Applikationen
### TROMEGA
[![FA-Frontend](https://img.shields.io/website?down_color=red&down_message=offline&label=TROMEGA%20Frontend&logo=flutter&style=plastic&up_color=green&up_message=online&url=https%3A%2F%2Ffitnessapp.gang-of-fork.de)](https://fitnessapp.gang-of-fork.de)   
[![FA-Backend](https://img.shields.io/website?down_color=red&down_message=offline&label=TROMEGA%20Backend&logo=express&style=plastic&up_color=green&up_message=online&url=https%3A%2F%2Fapi.fitnessapp.gang-of-fork.de%2Fping)](https://api.fitnessapp.gang-of-fork.de/ping)


<details open>
<summary>Andere Projekte</summary>
 
### Learning-Analytics

[![LA-Frontend](https://img.shields.io/website?down_color=red&down_message=offline&label=Learnings-Analytics%20Frontend&logo=flutter&style=plastic&up_color=green&up_message=online&url=https%3A%2F%2Flearning-analytics.gang-of-fork.de)](https://learning-analytics.gang-of-fork.de)  
[![LA-Backend](https://img.shields.io/website?down_color=red&down_message=offline&label=Learnings-Analytics%20Backend&logo=express&style=plastic&up_color=green&up_message=online&url=https%3A%2F%2Fapi.learning-analytics.gang-of-fork.de%2Fping)](https://api.learning-analytics.gang-of-fork.de/ping)


### PlantExchange

[![PE-Frontend](https://img.shields.io/website?down_color=red&down_message=offline&label=PlantExchange%20Frontend&logo=svelte&style=plastic&up_color=green&up_message=online&url=https%3A%2F%2Fplantexchange.gang-of-fork.de)](https://plantexchange.gang-of-fork.de)  
[![PE-Backend](https://img.shields.io/website?down_color=red&down_message=offline&label=PlantExchange%20Backend&logo=deno&style=plastic&up_color=green&up_message=online&url=https%3A%2F%2Fapi.plantexchange.gang-of-fork.de%2Fapi%2Fv1%2Fping)](https://api.plantexchange.gang-of-fork.de/api/v1/ping) 

</details>


## Entwicklungshinweise
<details>
<summary>Server-Port-Konfiguration</summary>
<br>
- xx0x : Fitnessapp
<br>
- xx1x : Learning-Analytics
<br>
- xx2x : PlantExchange
<br>
- xx3x : ODatafy MongoDB Example
</details>
