---
title: Ressourcentyp outlookTask
description: 'Ein Outlook-Element, das eine Arbeitsaufgabe überwachen kann. '
author: angelgolfer-ms
ms.openlocfilehash: 959e7ee7d6b1844d4b66b8ab53747e26aa91d492
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335231"
---
# <a name="outlooktask-resource-type"></a>Ressourcentyp outlookTask

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Outlook-Element, das eine Arbeitsaufgabe überwachen kann. 

Eine Aufgabe können Sie den Anfang Fälligkeitsdatum und tatsächlichen Durchführung Datums- und Zeitangaben, dessen Status oder Status, nachverfolgen, ob sie wiederholt sich, und einer Erinnerung erfordert.

Die folgenden: Eigenschaften in der Ressource **OutlookTask** datumsspezifische

- completedDateTime
- createdDateTime
- dueDateTime
- lastModifiedDateTime
- reminderDateTime
- startDateTime

In der Standardeinstellung zurückgeben die POST, GET, Patches und [vollständige](../api/outlooktask-complete.md) Vorgänge datumsspezifische Eigenschaften in ihren REST Antworten in UTC. Sie können mit dem `Prefer: outlook.timezone`-Header alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darstellen. Das folgende Beispiel gibt datumsbezogene Eigenschaften in EST in der entsprechenden Antwort zurück:

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von outlookTask](../api/outlooktask-get.md) | [outlookTask](outlooktask.md) |Rufen Sie die Eigenschaften und Beziehungen zwischen Outlook-Aufgaben in das Postfach des Benutzers an.|
|[Update](../api/outlooktask-update.md) | [outlookTask](outlooktask.md) |Ändern Sie die schreibbare Eigenschaften des Outlook-Aufgaben. |
|[Delete](../api/outlooktask-delete.md) | Keine |Löscht die angegebene Aufgabe im Postfach des Benutzers. |
|[Complete](../api/outlooktask-complete.md)|[OutlookTask](outlooktask.md) -Auflistung|Führen Sie eine Outlook-Aufgabe, die auf das aktuelle Datum und die **Status** -Eigenschaft, um die **CompletedDateTime** -Eigenschaft festgelegt wird `completed`.|
|**Anlagen**| | |
|[List attachments](../api/outlooktask-list-attachments.md) |[attachment](attachment.md) collection| Rufen Sie alle Anlagen auf eine Outlook-Aufgabe.|
|[Hinzufügen einer Anlage](../api/outlooktask-post-attachments.md) |[attachment](attachment.md)| Hinzufügen einer Datei, Element (Nachricht, Ereignis oder Kontakt) oder Link in eine Datei als Anlage zu einem Vorgang.|
|**Erweiterte Eigenschaften**| | |
|[Create single-value extended property](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTask](outlooktask.md)  |Erstellen Sie mindestens einen Single-Wert erweiterte Eigenschaften in einer neuen oder vorhandenen Outlook-Aufgabe.   |
|[Aufgabe mit erweiterten Eigenschaft einwertig abrufen](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Abrufen von Outlook-Aufgaben, die einen erweiterte Eigenschaft mithilfe von Single-Wert enthalten `$expand` oder `$filter`. |
|[Create multi-value extended property](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTask](outlooktask.md) | Erstellen Sie eine oder mehrere erweiterte mehrwertige Eigenschaften in einer neuen oder vorhandenen Outlook-Aufgabe.  |
|[Aufgabe mit erweiterten Mehrfachwert-Eigenschaft abrufen](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Abrufen eine Outlook-Aufgabe, die mithilfe eine erweiterte Eigenschaft mit mehreren Werte enthält `$expand`. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assignedTo|String|Der Name der Person, die die Aufgabe zugewiesen wurde.|
|body|[itemBody](itembody.md)|Der Hauptteil der Aufgabe, die in der Regel Informationen zum Vorgang enthält. Beachten Sie, dass nur HTML-Typ unterstützt wird.|
|categories|Zeichenfolgenauflistung|Die Kategorien, die dem Vorgang zugeordnet. Jeder Kategorie entspricht die **DisplayName** -Eigenschaft von einer [OutlookCategory](outlookcategory.md) , die der Benutzer definiert wurde.|
|changeKey|String|Die Version des Vorgangs.|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|Das Datum in der angegebenen Zeitzone, dass der Vorgang abgeschlossen wurde.|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung die Aufgabe. Standardmäßig ist es in UTC. Sie können eine benutzerdefinierte Zeitzone in der Kopfzeile der Anforderung bereitstellen. Wert der Eigenschaft verwendet die ISO 8601-Format. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|dueDateTime|[dateTimeTimeZone](datetimetimezone.md)|Das Datum in der angegebenen Zeitzone, die die Aufgabe fertig gestellt werden.|
|hasAttachments|Boolescher Wert|Legen Sie auf true zurück, wenn der Vorgang Anlagen hat.|
|id|String|Der eindeutige Bezeichner des Vorgangs. Schreibgeschützt|
|importance|string|Die Wichtigkeit des Ereignisses. Mögliche Werte sind: `low`, `normal` und `high`.|
|isReminderOn|Boolean|Legen Sie auf true zurück, wenn eine Warnung festgelegt ist, um die Benutzer über die Aufgabe zu erinnern.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten die Aufgabe Änderung. Standardmäßig ist es in UTC. Sie können eine benutzerdefinierte Zeitzone in der Kopfzeile der Anforderung bereitstellen. Wert der Eigenschaft um ISO 8601-Format verwendet und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|owner|String|Der Name der Person, die die Aufgabe erstellt.|
|parentFolderId|String|Der eindeutige Bezeichner für die Aufgabe übergeordneten Ordner.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Das Serienmuster für den Vorgang.|
|reminderDateTime|[dateTimeTimeZone](datetimetimezone.md)|Datum und Zeit für eine Erinnerung des Vorgangs erfolgt.|
|sensitivity|string|Gibt die Ebene des Datenschutzes für den Vorgang an. Mögliche Werte: sind `normal`, `personal`, `private` und `confidential`.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|Das Datum in der angegebenen Zeitzone, wenn der Vorgang zu beginnen.|
|status|string|Gibt das Bundesland oder den Fortschritt des Vorgangs. Mögliche Werte sind: `notStarted`, `inProgress`, `completed`, `waitingOnOthers` und `deferred`.|
|Betreff|String|Eine kurze Beschreibung oder Titel des Vorgangs.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) collection|Die Auflistung von [FileAttachment](fileattachment.md), [ItemAttachment](itemattachment.md)und [ReferenceAttachment](referenceattachment.md) Anlagen für den Vorgang.  Schreibgeschützt. Lässt Nullwerte zu.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung|Die Auflistung der Mehrfachwert erweiterte Eigenschaften für den Task definiert. Schreibgeschützt. Lässt Nullwerte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung|Die Auflistung der einwertig erweiterte Eigenschaften für den Task definiert. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.outlookTask"
}-->

```json
{
  "assignedTo": "String",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["String"],
  "changeKey": "String",
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "id": "String (identifier)",
  "importance": "string",
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "owner": "String",
  "parentFolderId": "String",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "sensitivity": "string",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "string",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->