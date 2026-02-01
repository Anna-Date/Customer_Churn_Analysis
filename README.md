# Customer_Churn_Analysis_Project
Vollständiges Customer Churn Analyse-Projekt für ein kanadisches Telekommunikationsunternehmen
---
## Projekt-Übersicht
Vollständiges Customer Churn Analytics Projekt für ein fiktives kanadisches Telekommunikationsunternehmen.

> Das Projekt bildet ein realistisches, relationales Unternehmensdatenmodell ab und kombiniert Kunden-, Vertrags-, Transaktions-, Zahlungs-, Nutzungs- und Churn-Daten zur Durchführung zeitbasierter Analysen und Business-Insights.
**Projektumfang:**
* 64,374 Kunden
* 1,010,527 Transaktionen
* 1,520,581 Aktivitätseinträge
* Zeitraum: 2023-2025
* Regionen: Ontario, Quebec, British Columbia, Alberta, Manitoba, Saskatchewan, Nova Scotia
---
## Daten 
> Als Ausgangspunkt wurde das öffentlich verfügbare Customer Churn Dataset von Kaggle verwendet.
Dieses Dataset wurde strukturell erweitert und durch **synthetisch generierte Zeit- und Verhaltensdaten** ergänzt, um ein realistisches, mehrtabelliges Analytics-Szenario abzubilden und komplexe Fragestellungen im Bereich Customer Lifecycle und Churn-Analyse zu ermöglichen.

Die synthetische Datengenerierung orientiert sich an realistischen Geschäftsannahmen (z. B. abnehmende Nutzung vor Churn, Zahlungsprobleme, Vertragslaufzeiten).

### Generierte Dateien
> Daten (CSV)
* **customers.csv** - Kundenstammdaten (64,374 Zeilen)
  - customer_id, signup_date, region, gender, age
* **contract.csv** - Vertragsdetails (64,374 Zeilen)
  - contract_id, customer_id, subscription_type, contract_length, start_date, end_date
* **transactions.csv** - Transaktionshistorie (1,010,527 Zeilen)
  - transaction_id, customer_id, transaction_date, product_id, revenue
* **payments.csv** - Zahlungsdaten (678,972 Zeilen)
  - payment_id, transaction_id, payment_delay_days, payment_status
* **customer_activity.csv** - Monatliche Aktivität (1,520,581 Zeilen)
  - activity_id, customer_id, activity_month, logins, support_calls
* **churn_events.csv** - Abwanderungsereignisse (30,493 Zeilen)
  - customer_id, churn_date, churn_reason
