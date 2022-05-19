# Datenbanken
## Nachrichten
### Firestore
- 1.000.000 Reads + Writes
- **46,15€**

### Cloud SQL
- 1 CPU 
- 3,75 GB RAM
- 250 GB HDD
- 148,34 €

<br>

## Benutzerprofil
### Cloud SQL
- 2 CPUs 
- 7,5 GB Ram 
- 50 GB
- **170,10 €**

<br>

## Inserate
### Cloud SQL
- 8 CPUs
- 52 GB Ram
- 2 TB
- 2 TB
- **1.158,69 €**

<br>

## Bezahlen

<br>

## Marketing

<br>

## Datenanalyse 
### Pub/Sub
- 10 GB
- 1 Sub
- **21,84 €**

<br>
<br>

# BigQuery
- Active Storage: 900 GB
- Longterm Storage: 900 GB
- Query: 3 TB
- **45,21 €**

<br>
<br>

# Cluster
6 Services, pro Service 1 CPU und 2 GB Ram.<br>
Die Mikroservices, Inserate und Benutzerprofile werden wahrscheinlich mehr als jeweils zwei CPUs beanspruchen. Die restlichen vier Mikroservices Teilen sich auf die verbleibenden 2 CPUs entsprechend auf. <br>
<br>
Der Marketingservice wird nur während den Arbeitszeiten genutzt. Dabei handelt es sich um 5 Tage mit jeweils 10 Stunden. Dadurch werden zum Wochenende Kapazitäten frei, die als Reserve genutzt werden, um den erwarteten Haupttraffic zu verarbeiten.<br>
<br>
Inserate, Benutzerprofil und Bezahlen werden auch bei geringer Auslastung mit einem Pod extra in Reserve betrieben.

Sicherheitsfaktor von 3.

Verteilt auf 3 Nodes für die Stabilität. Falls einer ausfällt sind schnell können die beiden anderen übernehmen.

- 3 Nodes
- je 6 CPU + 12 RAM
- 10 GB Boot Size
- **449,75 €** 

<br>
<br>

# Loadbalancer

