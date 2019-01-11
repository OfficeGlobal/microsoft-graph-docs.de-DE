---
title: Ressourcentyp secureScores
description: 'Top n =, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten. '
localization_priority: Normal
ms.openlocfilehash: 332a9656d8237bb07d5c7739b666e09539cf984f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828735"
---
# <a name="securescores-resource-type"></a>Ressourcentyp secureScores

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Mandanten sichere Faktor pro Tag der Daten, auf der Ebene Mandanten und Steuerelement bewerten. In der Standardeinstellung ist 90 Tage von Daten enthalten. Diese Daten sortiert spätesten zum frühesten durch **CreatedDateTime**, aus. Dadurch können Sie auf der Seitenantworten mithilfe von $top = n, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten. 


## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[List secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |Lesen Sie Eigenschaften und Metadaten eines SecureScores-Objekts.|


## <a name="properties"></a>Eigenschaften
Typ mit Eigenschaften der Mandant Sicherheit Entität Punktzahl (tägliche Momentaufnahme Daten).

|Eigenschaft |Typ |Beschreibung |
|:--|:--|:--|
|   azureTenantId   |   Zeichenfolge  |   GUID-Zeichenfolge für Mandanten-ID ein.  |
|   createdDateTime |   DateTimeOffset  |   Das Datum, wenn die Entität erstellt wird.  |
|   id  |   Zeichenfolge  |   Kombination von AzureTenantId_createdDateTime.   |
|   licensedUserCount   |   Int32   |   Die Anzahl der Benutzer des angegebenen Mandanten lizenziert.    |
|   activeUserCount |   Int32   |   Aktive Benutzeranzahl des angegebenen Mandanten.  |
|   currentScore    |   Gleitkommawert mit doppelter Genauigkeit  |   Mandanten aktuellen erreicht Score am angegebenen Datum.    |
|   MaxErgebnis |  Gleitkommawert mit doppelter Genauigkeit  |   Mandanten maximale Bewertung am angegebenen Datum.    |
|   enabledServices |   Collection von Objekten des Typs „String“   |   Microsoft-Dienste für den Mandanten (beispielsweise Exchange online, Skype, Sharepoint).   |
|   averageComparativeScores |  [AverageComparativeScore](averagecomparativescore.md) -Auflistung    |Durchschnittliche Bewertung von unterschiedlichen Bereichen (beispielsweise Durchschnitt nach Branche, durchschnittliche durch Sitzplätze) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) innerhalb des Bereichs. |
|   controlScores | [ControlScore](controlscore.md) -Auflistung  |   Mandanten Bewertungen für eine Gruppe von Steuerelementen enthält.   |


## <a name="relationships"></a>Beziehungen

Keine.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"id": "String",
"azureTenantId": "Guid",
"createdDate": "DateTimeOffset",
"licensedUserCount": "Int32",
"activeUserCount": "Int32",
"currentScore": "Int32",
"maxScore": "Int32",
"averageScore": "Double",
"enabledServices": "Collection(string)",
"averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
"controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
}

```


<!-- {
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
