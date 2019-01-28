---
title: outlookTask-Ressourcentyp
description: 'Ein Outlook-Element, das ein Arbeitselement verfolgen kann. '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 6a6d5809f2634f4b9e0f1e30e3fddb0c798f0f6c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576437"
---
# <a name="outlooktask-resource-type"></a>outlookTask-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Outlook-Element, das ein Arbeitselement verfolgen kann. 

Sie können eine Aufgabe verwenden, um Datumsangaben und Uhrzeiten für das Startdatum, das Fälligkeitsdatum und den tatsächlichen Abschluss sowie den Fortschritt oder Status anzugeben. Außerdem können Sie angeben, ob sich die Aufgabe wiederholt und eine Erinnerung erfordert.

Datumsbezogene Eigenschaften in der **outlookTask**-Ressource umfassen Folgendes:

- completedDateTime
- createdDateTime
- dueDateTime
- lastModifiedDateTime
- reminderDateTime
- startDateTime

Die POST-, GET-, PATCH- und [complete](../api/outlooktask-complete.md)-Vorgänge geben datumsbezogene Eigenschaften in ihren REST-Antworten standardmäßig in UTC zurück. Sie können die `Prefer: outlook.timezone`-Kopfzeile verwenden, um alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darzustellen. Das folgende Beispiel gibt datumsbezogene Eigenschaften in der entsprechenden Antwort in EST zurück:

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Get outlookTask](../api/outlooktask-get.md) | [outlookTask](outlooktask.md) |Abrufen der Eigenschaften und Beziehungen einer Outlook-Aufgabe im Postfach des Benutzers.|
|[Update](../api/outlooktask-update.md) | [outlookTask](outlooktask.md) |Ändern der schreibbaren Eigenschaften einer Outlook-Aufgabe. |
|[Delete](../api/outlooktask-delete.md) | Keine |Löschen der angegebenen Aufgabe im Postfach des Benutzers. |
|[Complete](../api/outlooktask-complete.md)|[outlookTask](outlooktask.md)-Sammlung|Abschließen einer Outlook-Aufgabe, durch die die **CompletedDateTime**-Eigenschaft auf das aktuelle Datum und die **status**-Eigenschaft auf `completed` festgelegt wird.|
|**Anlagen**| | |
|[List attachments](../api/outlooktask-list-attachments.md) |[attachment](attachment.md)-Sammlung| Ruft alle Anlagen für eine Outlook-Aufgabe ab.|
|[Anlage hinzufügen](../api/outlooktask-post-attachments.md) |[Anlage](attachment.md)| Hinzufügen einer Datei, eines Elements (Nachricht, Ereignis oder Kontakt) oder eines Links zu einer Datei als Anlage einer Aufgabe.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTask](outlooktask.md)  |Erstellt eine oder mehrere einwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Outlook-Aufgabe.   |
|[Aufgabe mit erweiterter einwertiger Eigenschaft abrufen](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Ruft mithilfe von `$expand` oder `$filter` Outlook-Aufgaben mit einer einwertigen erweiterten Eigenschaft ab. |
|[Mehrwertige erweiterte Eigenschaft erstellen](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTask](outlooktask.md) | Erstellt eine oder mehrere mehrwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Outlook-Aufgabe.  |
|[Aufgabe mit erweiterter mehrwertiger Eigenschaft abrufen](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Ruft mithilfe von `$expand` eine Outlook-Aufgabe mit einer bestimmten mehrwertigen erweiterten Eigenschaft ab. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assignedTo|Zeichenfolge|Der Name der Person, der die Aufgabe zugewiesen wurde.|
|body|[itemBody](itembody.md)|Der Aufgabentext, der in der Regel Informationen zu der Aufgabe enthält. Beachten Sie, dass nur der HTML-Typ unterstützt wird.|
|categories|Zeichenfolgenauflistung|Die Kategorien, die mit der Aufgabe verknüpft sind. Jede Kategorie entspricht der **displayName**-Eigenschaft einer vom Benutzer definierten [outlookCategory](outlookcategory.md).|
|changeKey|Zeichenfolge|Version der Aufgabe.|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|Das Datum in der angegebenen Zeitzone, an dem die Aufgabe abgeschlossen wurde.|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit der Erstellung der Aufgabe. Die Standardeinstellung ist UTC. Sie können eine benutzerdefinierte Zeitzone im Anforderungsheader bereitstellen. Der Wert der Eigenschaft verwendet das ISO 8601-Format. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|dueDateTime|[dateTimeTimeZone](datetimetimezone.md)|Das Datum in der angegebenen Zeitzone, in der die Aufgabe abgeschlossen werden soll.|
|hasAttachments|Boolescher Wert|„true“, wenn die Aufgabe Anlagen hat.|
|id|Zeichenfolge|Der eindeutige Bezeichner der Aufgabe. Schreibgeschützt.|
|importance|Zeichenfolge|Die Wichtigkeit des Ereignisses. Mögliche Werte sind: `low`, `normal` und `high`.|
|isReminderOn|Boolescher Wert|„true“, wenn eingestellt ist, dass der Benutzer an die Aufgabe erinnert werden soll.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Aufgabe. Die Standardeinstellung ist UTC. Sie können eine benutzerdefinierte Zeitzone im Anforderungsheader bereitstellen. Der Eigenschaftswert verwendet das ISO 8601-Format, und die Angabe erfolgt immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|owner|Zeichenfolge|Der Name der Person, die die Aufgabe erstellt hat.|
|parentFolderId|Zeichenfolge|Der eindeutige Bezeichner für den übergeordneten Ordner der Aufgabe.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Das Serienmuster für die Aufgabe.|
|reminderDateTime|[dateTimeTimeZone](datetimetimezone.md)|Datum und Uhrzeit für eine Erinnerung der Aufgabe.|
|sensitivity|Zeichenfolge|Gibt den Grad des Datenschutzes für die Aufgabe an. Mögliche Werte: `normal`, `personal`, `private`, `confidential`|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|Das Datum in der angegebenen Zeitzone, an dem die Aufgabe begonnen werden soll.|
|status|Zeichenfolge|Gibt den Status oder den Fortschritt der Aufgabe an. Mögliche Werte: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|subject|Zeichenfolge|Eine kurze Beschreibung oder ein Titel für die Aufgabe.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md)-Sammlung|Die Sammlung der [fileAttachment](fileattachment.md)-, [itemAttachment](itemattachment.md)- und [referenceAttachment](referenceattachment.md)-Anlagen der Aufgabe.  Schreibgeschützt. Nullwerte zulassend.|
|multiValueLegacyExtendedProperty|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung|Die Sammlung erweiterter mehrwertiger Eigenschaften, die für die Aufgabe definiert sind. Schreibgeschützt. Nullwerte zulassend.|
|singleValueLegacyExtendedProperty|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung|Die Sammlung erweiterter einwertiger Eigenschaften, die für die Aufgabe definiert sind. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktask.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
