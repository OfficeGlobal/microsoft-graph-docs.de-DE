---
title: Ressourcentyp historyItem
description: Stellt ein Verlaufselement für eine Aktivität in einer app. Die Benutzeraktivitäten darstellen ein einziges Ziel in der app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel. Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als Element Verlauf erfasst, das die Start- und Endzeit für diese Aktivität angibt. Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.
ms.openlocfilehash: 5687e592a65e162c105d97c90cd7a6f8f578d303
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065378"
---
# <a name="historyitem-resource-type"></a>Ressourcentyp historyItem

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt ein Verlaufselement für eine [Aktivität](projectrome-activity.md) in einer app. Die Benutzeraktivitäten darstellen ein einziges Ziel in der app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel. Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als Element Verlauf erfasst, das die Start- und Endzeit für diese Aktivität angibt. Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.

Wenn eine app eine Sitzung erstellt, sollte ein **HistoryItem** -Objekt auf die **Aktivität** -Objekt entsprechend den Zeitraum eines Auftrags für Benutzer hinzugefügt werden. Jedes Mal wird ein Benutzer mit einer Aktivität erneut aktiviert wird, eine neue **HistoryItem** Aktivität auf die Benutzer Engagements fällig hinzugefügt.

## <a name="methods"></a>Methoden

|Methode | Rückgabetyp | Beschreibung|
|:------|:------------|:-----------|
|[Erstellen oder ersetzen historyItem](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | Erstellt oder eine vorhandene **HistoryItem** für diese Aktivität (Upsert) ersetzt. Die ID muss eine GUID sein.|
|[Löschen einer historyItem](../api/projectrome-delete-historyitem.md) | Kein Inhalt | Löscht das angegebene **HistoryItem** für diese Aktivität.|

## <a name="properties"></a>Eigenschaften

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|status | EnumType | Vom Server festgelegt. Einen Statuscode verwendet, um gültige Objekte identifizieren. Werte: aktiv, aktualisiert, gelöscht, ignoriert.|
|userTimezone | Zeichenfolge | Optional. Die Zeitzone, in der das Gerät des Benutzers verwendet, um die Aktivität generieren zum Zeitpunkt der Erstellung Aktivität gefunden wurde. Werte, die zur Unterstützung der plattformübergreifende Darstellung als Olson-IDs angegeben.|
|createdDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, wenn das Objekt auf dem Server erstellt wurde.|
|lastModifiedDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, wenn das Objekt auf dem Server geändert wurde.|
|id | Zeichenfolge | Erforderlich. Client-Set-GUID für das **HistoryItem** -Objekt.|
|startedDateTime | DateTimeOffset | Erforderlich. UTC-DateTime beim **HistoryItem** (Aktivität Sitzung) gestartet wurde. Erforderlich für die Versionsgeschichte der Zeitachse.|
|lastActiveDateTime | DateTimeOffset | Optional. UTC-DateTime beim letzten **HistoryItem** (Aktivität Sitzung) als aktiv oder fertig - bei null **HistoryItem** Status erkannt wurden, sollte laufend Besprechung sein.|
|expirationDateTime | DateTimeOffset | Optional. UTC-DateTime, wenn die **HistoryItem** harten Löschens durchläuft. Kann vom Client festgelegt werden.|
|activeDurationSeconds | Int | Optional. Die Dauer des Engagements aktiver Benutzer. Wenn nicht angegeben ist, erfolgt die Berechnung von der **StartedDateTime** und **LastActiveDateTime**.|

## <a name="relationships"></a>Beziehungen

|Beziehung | Typ | Beschreibung|
|:------------|:-----|:-----------|
|activity| [Aktivität](../resources/projectrome-activity.md) | Optional. NavigationProperty/Kapselung; Navigationseigenschaft der zugeordneten Aktivität.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "@odata.type": "microsoft.graph.historyItem"
}-->

```json
{
    "status": "String (EnumType)",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
