---
title: Ressourcentyp secureScores
description: 'Top n =, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten. '
localization_priority: Normal
ms.openlocfilehash: fef5c43130aecf1604677d07f785a0cee0539568
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576080"
---
# <a name="securescores-resource-type"></a>Ressourcentyp secureScores

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt einen Mandanten sichere Faktor pro Tag der Daten, auf der Ebene Mandanten und Steuerelement bewerten. In der Standardeinstellung ist 90 Tage von Daten enthalten. Diese Daten sortiert spätesten zum frühesten durch **CreatedDateTime**, aus. Dadurch können Sie auf der Seitenantworten mithilfe von $top = n, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten. 


## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[List secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |Lesen Sie Eigenschaften und Metadaten eines SecureScores-Objekts.|


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
|   enabledServices |   Zeichenfolgenauflistung   |   Microsoft-Dienste für den Mandanten (beispielsweise Exchange online, Skype, Sharepoint).   |
|   averageComparativeScores |  [AverageComparativeScore](averagecomparativescore.md) -Auflistung    |Durchschnittliche Bewertung von unterschiedlichen Bereichen (beispielsweise Durchschnitt nach Branche, durchschnittliche durch Sitzplätze) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) innerhalb des Bereichs. |
|   controlScores | [ControlScore](controlscore.md) -Auflistung  |   Mandanten Bewertungen für eine Gruppe von Steuerelementen enthält.   |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) | Enthält Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).|

## <a name="relationships"></a>Beziehungen

Keine.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
    "id": "String",
    "azureTenantId": "String (identifier)",
    "createdDateTime": "DateTimeOffset",
    "licensedUserCount": "Int32",
    "activeUserCount": "Int32",
    "currentScore": "Double",
    "maxScore": "Double",    
    "enabledServices": ["String"],
    "averageComparativeScores": [{ "@odata.type":"microsoft.graph.averageComparativeScores"}],
    "controlScores": [{"@odata.type":"microsoft.graph.controlScores"}],
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
}
```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescores.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
