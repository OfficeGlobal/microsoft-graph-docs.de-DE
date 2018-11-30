---
title: Ressourcentyp secureScores
description: 'Top n =, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten. '
ms.openlocfilehash: 96d5c487bb854559b0128d93ea8e0783fcc61f0c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058982"
---
# <a name="securescores-resource-type"></a>Ressourcentyp secureScores

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Mandanten sichere Faktor pro Tag der Daten, auf der Ebene Mandanten und Steuerelement bewerten. In der Standardeinstellung ist 90 Tage von Daten enthalten. Diese Daten sortiert spätesten zum frühesten durch **CreatedDateTime**, aus. Dadurch können Sie auf der Seitenantworten mithilfe von $top = n, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten. 


## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[Liste secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |Lesen Sie Eigenschaften und Metadaten eines SecureScores-Objekts.|


## <a name="properties"></a>Eigenschaften
Typ mit Eigenschaften der Mandant Sicherheit Entität Punktzahl (tägliche Momentaufnahme Daten).

|Eigenschaft |Typ |Beschreibung |
|:--|:--|:--|
|   azureTenantId   |   String  |   GUID-Zeichenfolge für Mandanten-ID ein.  |
|   createdDateTime |   DateTimeOffset  |   Das Datum, wenn die Entität erstellt wird.  |
|   id  |   String  |   Kombination von AzureTenantId_createdDateTime.   |
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
