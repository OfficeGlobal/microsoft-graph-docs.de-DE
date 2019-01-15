---
title: Planen wiederkehrender Termine als wiederkehrende Ereignisse in Outlook
description: Ereignisserien sind ein wichtiger Bestandteil der Kalenderfunktionen von Outlook. Ganz gleich, ob es sich um eine wöchentliche Besprechung mit Ihrem Vorgesetzten oder eine Abteilungsbesprechung handelt, die jeden zweiten Dienstag im Monat stattfindet, mit Ereignisserien können Sie ganz einfach eine Ereignisserie erstellen und der Server füllt den Kalender mit dem Rest der Serie.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 9cdd7e7170dc48c2739514674786893efeae1b4e
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016765"
---
# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a>Planen wiederkehrender Termine als wiederkehrende Ereignisse in Outlook

Ereignisserien sind ein wichtiger Bestandteil der Kalenderfunktionen von Outlook. Ganz gleich, ob es sich um eine wöchentliche Besprechung mit Ihrem Vorgesetzten oder eine Abteilungsbesprechung handelt, die jeden zweiten Dienstag im Monat stattfindet, mit Ereignisserien können Sie ganz einfach eine Ereignisserie erstellen und der Server füllt den Kalender mit dem Rest der Serie.

Die wichtigsten Informationen, mit denen Ereignisserien in einzelne Termine „erweitert“ werden können, die Serienregel. In der Serie ist die Wiederholungsfrequenz und Dauer eines Ereignisses angegeben. Die Outlook-REST-APIs modellieren Serienregeln in der **Serien**-Eigenschaft der [Ereignisressource](/graph/api/resources/event?view=graph-rest-1.0). 

Jede Serie besteht aus zwei Teilen: dem Serienmuster (wie oft) und dem Serienbereich (für wie lange).

## <a name="recurrence-patterns"></a>Serienmuster

Der erste Teil einer Serie ist das Muster. Darin ist angegeben, wie oft das Ereignis wiederholt wird. Beispielsweise könnte ein Ereignis „alle 3 Tage“, „jeden Donnerstag“ oder „jedes Jahr am 22. Juli“ wiederholt werden. Ein Muster wird in der API durch die [recurrencePattern-Ressource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0) dargestellt.

Je nach Mustertyp sind bestimmte Felder des **recurrencePattern** obligatorisch, optional oder werden ignoriert.

> **Hinweis:** Auch wenn ein Feld ignoriert wird, wird es dennoch überprüft. Wenn ein Feld über eine festgelegte Liste möglicher Werte verfügt, führt ein Wert außerhalb der zulässigen Gruppe von Werten zu einem Fehler, selbst wenn das Feld ignoriert wird.

Werfen Sie einen Blick auf die einzelnen Arten möglicher Muster.

### <a name="daily"></a>Täglich

Das tägliche Serienmuster bewirkt, dass ein Ereignis basierend auf einer Anzahl von Tagen zwischen zwei Vorkommen wiederholt wird.

#### <a name="relevant-properties"></a>Relevante Eigenschaften

| Eigenschaft | Relevanz | Beschreibung |
|----------|-----------|-------------|
| **Intervall** | Erforderlich | Gibt die Anzahl der Tage zwischen zwei Vorkommen an. |
| **Typ** | Erforderlich | Muss auf `daily` festgelegt werden. |

#### <a name="examples"></a>Beispiele

- Dieses Ereignis täglich wiederholen

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- Dieses Ereignis alle drei Tage wiederholen

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a>Wöchentlich

Das wöchentliche Serienmuster bewirkt, dass ein Ereignis am gleichen Tag oder an den gleichen Tagen einer Woche basierend auf der Anzahl von Wochen zwischen zwei Vorkommen wiederholt wird.

#### <a name="relevant-properties"></a>Relevante Eigenschaften

| Eigenschaft | Relevanz | Beschreibung |
|----------|-----------|-------------|
| **daysOfWeek** | Erforderlich | Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintritt. |
| **firstDayOfWeek** | Optional | Gibt an, welcher Tag als erster Tag der Woche angesehen wird. Standardwert: `Sunday`. |
| **Intervall** | Erforderlich | Gibt die Anzahl der Wochen zwischen zwei Vorkommen an. |
| **Typ** | Erforderlich | Muss auf `weekly` festgelegt werden. |

#### <a name="examples"></a>Beispiele

- Dieses Ereignis jeden Donnerstag wiederholen

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- Dieses Ereignis jeden Montag und Dienstag wiederholen

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 2,
      "daysOfWeek": [
        "Monday",
        "Tuesday"
      ]
    }
  ```

### <a name="absolute-monthly"></a>Absolut monatlich

Das absolute monatliche Muster bewirkt, dass ein Ereignis am gleichen Tag des Monats (z. B. dem 15.) basierend auf der Anzahl der Monate zwischen zwei Vorkommen stattfindet.

#### <a name="relevant-properties"></a>Relevante Eigenschaften

| Eigenschaft | Relevanz | Beschreibung |
|----------|-----------|-------------|
| **dayOfMonth** | Erforderlich | Gibt an, an welchem Tag des Monats das Ereignis eintritt. |
| **Intervall** | Erforderlich | Gibt die Anzahl der Monate zwischen zwei Vorkommen an. |
| **Typ** | Erforderlich | Muss auf `absoluteMonthly` festgelegt werden. |

#### <a name="examples"></a>Beispiele

- Dieses Ereignis jeden Monat am 15. wiederholen

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- Dieses Ereignis vierteljährlich (alle 3 Monate) am 7. wiederholen

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a>Relativ monatlich

Das relative monatliche Muster bewirkt, dass ein Ereignis am gleichen Wochentag an der gleichen relativen Position des Monats basierend auf der Anzahl der Monate zwischen zwei Vorkommen stattfindet. Beispielsweise „jeden zweiten Mittwoch des Monats“.

#### <a name="relevant-properties"></a>Relevante Eigenschaften

| Eigenschaft | Relevanz | Beschreibung |
|----------|-----------|-------------|
| **daysOfWeek** | Erforderlich | Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintreten kann. Relative monatliche Ereignisse treten nur einmal pro Monat ein, wird also mehr als ein Wert angegeben, fällt das Ereignis auf den ersten Tag, der das Muster erfüllt. |
| **Index** | Optional | Gibt an, in welcher Instanz der zulässigen Tage, die unter **daysOfsWeek** angegeben sind, das Ereignis eintritt, ausgehend von der ersten Instanz des Monats gezählt. Mögliche Werte: `first`, `second`, `third`, `fourth` und `last`. Standardwert: `first`. |
| **Intervall** | Erforderlich | Gibt die Anzahl der Monate zwischen zwei Vorkommen an. |
| **Typ** | Erforderlich | Muss auf `relativeMonthly` festgelegt werden. |

#### <a name="examples"></a>Beispiele

- Dieses Ereignis jeden zweiten Mittwoch des Monats wiederholen

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- Dieses Ereignis jeden zweiten Mittwoch des Monats wiederholen

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a>Absolut jährlich

Das absolut jährliche Muster bewirkt, dass ein Ereignis am gleichen Tag und im gleichen Monat (z. B. dem 15. April), basierend auf der Anzahl der Jahre zwischen zwei Vorkommen stattfindet.

#### <a name="relevant-properties"></a>Relevante Eigenschaften

| Eigenschaft | Relevanz | Beschreibung |
|----------|-----------|-------------|
| **dayOfMonth** | Erforderlich | Gibt an, an welchem Tag des Monats das Ereignis eintritt. |
| **Monat** | Erforderlich | Gibt an, in welchem Monat das Ereignis auftritt. |
| **Intervall** | Erforderlich | Gibt die Anzahl der Jahre zwischen zwei Vorkommen an. |
| **Typ** | Erforderlich | Muss auf `absoluteYearly` festgelegt werden. |

#### <a name="example"></a>Beispiel

- Dieses Ereignis jedes Jahr am 15. April wiederholen

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a>Relativ jährlich

Das relative jährliche Muster bewirkt, dass ein Ereignis am gleichen Wochentag an der gleichen relativen Position eines bestimmten Monats basierend auf der Anzahl der Jahre zwischen zwei Vorkommen stattfindet. Beispielsweise „jeden letzten Mittwoch im November“.

#### <a name="relevant-properties"></a>Relevante Eigenschaften

| Eigenschaft | Relevanz | Beschreibung |
|----------|-----------|-------------|
| **daysOfWeek** | Erforderlich | Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintreten kann. Relative jährliche Ereignisse treten nur einmal pro Jahr ein, wird also mehr als ein Wert angegeben, fällt das Ereignis auf den ersten Tag, der das Muster erfüllt. |
| **Index** | Optional | Gibt an, in welcher Instanz der zulässigen Tage, die unter **daysOfsWeek** angegeben sind, das Ereignis eintritt, ausgehend von der ersten Instanz des Monats gezählt. Mögliche Werte: `first`, `second`, `third`, `fourth` und `last`. Standardwert: `first`. |
| **Monat** | Erforderlich | Gibt an, in welchem Monat das Ereignis auftritt. |
| **Intervall** | Erforderlich | Gibt die Anzahl der Jahre zwischen zwei Vorkommen an. |
| **Typ** | Erforderlich | Muss auf `relativeYearly` festgelegt werden. |

#### <a name="examples"></a>Beispiele

- Dieses Ereignis jedes Jahr am letzten Mittwoch im November wiederholen

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a>Serienbereiche

Der zweite Teil einer Serie ist das Muster. Dies gibt an, wie lange das Muster wiederholt wird. Ein Ereignis könnte beispielsweise nach 10 Vorkommen an einem bestimmten Datum enden oder kein Ende haben. Ein Bereich wird in der API durch die [recurrenceRange-Ressource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0) dargestellt.

Je nach Bereichstyp sind bestimmte Felder der **recurrenceRange** obligatorisch oder werden ignoriert.

> **Hinweis:** Auch wenn ein Feld ignoriert wird, wird es dennoch überprüft. Wenn ein Feld über eine festgelegte Liste möglicher Werte verfügt, führt ein Wert außerhalb der zulässigen Gruppe von Werten zu einem Fehler, selbst wenn das Feld ignoriert wird.

Werfen wir einen Blick auf die einzelnen Arten möglicher Bereiche.

### <a name="numbered-range"></a>Nummerierter Bereich

Der nummerierte Bereich bewirkt, dass ein Ereignis eine feste Anzahl von Vorkommen (basierend auf dem Muster) ab einem Startdatum auftritt.

#### <a name="relevant-properties"></a>Relevante Eigenschaften

| Eigenschaft | Relevanz | Beschreibung |
|----------|-----------|-------------|
| **numberOfOccurences** | Erforderlich | Gibt die Anzahl von Vorkommen an. Das Vorkommen muss eine positive ganze Zahl sein. |
| **recurrenceTimeZone** | Optional | Gibt die Zeitzone für die **StartDate**-Eigenschaft an. Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet. |
| **startDate** | Erforderlich | Gibt das Datum des Starts des Anwendens des Musters an. Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](/graph/api/resources/event?view=graph-rest-1.0) entsprechen. Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt. |
| **Typ** | Erforderlich | Muss auf `numbered` festgelegt werden. |

#### <a name="examples"></a>Beispiele

- Dieses Ereignis 10 Mal wiederholen

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a>Enddatumsbereich

Der Enddatumsbereich bewirkt, dass ein Ereignis an allen Tagen eintritt, die das entsprechende Muster zwischen einem Startdatum und einem Enddatum aufweisen.

#### <a name="relevant-properties"></a>Relevante Eigenschaften

| Eigenschaft | Relevanz | Beschreibung |
|----------|-----------|-------------|
| **endDate** | Erforderlich | Gibt das Datum zum Beenden des Anwendens des Musters an. Hinweis: Das letzte Vorkommen der Besprechung kann nicht an diesem Datum auftreten, wenn es nicht in das Muster passt. |
| **recurrenceTimeZone** | Optional | Gibt die Zeitzone für die **startDate**- und **endDate**-Eigenschaften an. Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet. |
| **startDate** | Erforderlich | Gibt das Datum des Starts des Anwendens des Musters an. Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](/graph/api/resources/event?view=graph-rest-1.0) entsprechen. Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt. |
| **Typ** | Erforderlich | Muss auf **EndDate** festgelegt werden. |

#### <a name="examples"></a>Beispiele

- Dieses Ereignis vom 1. Juli 2017 bis zum 31. Juli 2017 wiederholen

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a>Kein Endbereich

Der Enddatumsbereich bewirkt, dass ein Ereignis an allen Tagen eintritt, die dem anwendbaren Muster nach einem Startdatum entsprechen.

#### <a name="relevant-properties"></a>Relevante Eigenschaften

| Eigenschaft | Relevanz | Beschreibung |
|----------|-----------|-------------|
| **recurrenceTimeZone** | Optional | Gibt die Zeitzone für die **StartDate**-Eigenschaft an. Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet. |
| **startDate** | Erforderlich | Gibt das Datum des Starts des Anwendens des Musters an. Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](/graph/api/resources/event?view=graph-rest-1.0) entsprechen. Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt. |
| **Typ** | Erforderlich | Muss auf `noEnd` festgelegt werden. |

#### <a name="examples"></a>Beispiele

- Dieses Ereignis ab dem 15. Mai 2017 immer wiederholen

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a>Verwenden von Mustern und Bereichen zum Erstellen von Ereignisserien

Nachdem wir uns nun Muster und Bereiche separat angesehen haben, schauen wir uns nun deren Zusammenwirken und Interagieren mit den **Start**- und **End**-Eigenschaften zu dem Ereignis an.

### <a name="creating-a-recurrence-rule"></a>Erstellen einer Serienregel

Um eine Serienregel zu erstellen, müssen Sie sowohl ein Muster als auch einen Bereich angeben. Jeder Mustertyp kann mit einem beliebigen Bereichstyp arbeiten. Im Anschluss finden Sie einige Beispiele:

#### <a name="examples"></a>Beispiele

- **Besprechung von 13:00-13:30 Uhr, jeden Montag ab dem 4. September 2017 bis zum Ende des Jahres**

  - Die Anforderung „jeden Montag“ wird ganz einfach durch den `weekly`-Serienmustertyp erfüllt.
  - Die Anforderung „bis zum Ende des Jahres“ gibt einen `endDate`-Serienbereichstypen an.

  ```json
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1,
        "daysOfWeek": [ "Monday" ]
      },
      "range": {
        "type": "endDate",
        "startDate": "2017-09-04",
        "endDate": "2017-12-31"
      }
    }
  ```

  Da der 31. Dezember 2017 auf einen Sonntag fällt, ist das letzte Vorkommen in dieser Serie am Montag, den 25. Dezember.

- **Besprechung von 14:00-15:00 Uhr am ersten Donnerstag jeden zweiten Monat, ab dem 29. August 2017**

  - Die Anforderung „erster Donnerstag jeden zweiten Monat“ kann durch ein relatives monatliches Muster erfüllt werden. Der Teil „jeden zweiten Monats“ gibt an, dass das **Intervall** auf `2` festgelegt werden sollte.
  - Da es keine Anforderung an ein Enddatum gibt, kann ein `noEnd`-Bereichstyp verwendet werden.

  ```json
    "recurrence": {
      "pattern": {
        "type": "relativeMonthly",
        "interval": 2,
        "daysOfWeek": [ "Thursday" ],
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "startDate": "2017-08-29"
      }
    }
  ```

  Da der Wert von **startDate** nach dem ersten Donnerstag im August liegt, ist das erste Vorkommen dieser Serie im September.

## <a name="next-steps"></a>Nächste Schritte
    
Erfahren Sie mehr zur [Integration in Outlook-Kalender](outlook-calendar-concept-overview.md).
