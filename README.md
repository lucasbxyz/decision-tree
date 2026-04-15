# Decision Trees & Random Forests – Loan Repayment

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lucasbxyz/decision-tree/HEAD)

Vorhersage, ob Kreditnehmer auf LendingClub.com ihren Kredit vollständig zurückzahlen, mithilfe von Decision Trees und Random Forests. Der Datensatz (`loan_data.csv`) enthält Kreditdaten von 2007–2010 mit Features wie FICO-Score, Zinssatz und Kreditverwendungszweck.

## Ausführung

1. Auf den **Binder Badge** oben klicken — die Umgebung startet automatisch.
2. Im Jupyter-Interface das Notebook `3-Decision_Trees_und_Random_Forests.ipynb` öffnen.
3. **Cell → Run All** ausführen (oder Zellen einzeln mit Shift+Enter durchlaufen).
4. Die Ausführung dauert ca. 1–2 Minuten.

## Erwartete Ergebnisse

- **Explorative Analyse:** Visualisierungen der Kreditdaten (FICO-Verteilung, Zinssätze etc.).
- **Decision Tree:** Zunächst ein einzelner Decision Tree — liefert eine Accuracy von ca. **73 %**.
- **Random Forest:** Anschließend ein Random Forest (600 Estimators), der die Performance deutlich verbessert.
- **Classification Report** des Random Forest (ca.):

| Metrik    | Klasse 0 (zurückgezahlt) | Klasse 1 (nicht zurückgezahlt) |
|-----------|--------------------------|-------------------------------|
| Precision | 0.85                     | 0.47                          |
| Recall    | 1.00                     | 0.02                          |
| F1-Score  | 0.92                     | 0.04                          |

- **Gesamtgenauigkeit Random Forest:** ca. **85 %**
- Die niedrige Recall-Rate für Klasse 1 zeigt die typische Herausforderung bei unbalancierten Klassen.

## Dateien

| Datei | Beschreibung |
|-------|-------------|
| `3-Decision_Trees_und_Random_Forests.ipynb` | Jupyter Notebook mit der Analyse |
| `loan_data.csv` | LendingClub-Kreditdatensatz |
| `requirements.txt` | Python-Abhängigkeiten für Binder |
