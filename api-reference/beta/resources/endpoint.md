---
title: Endpunkt-Ressourcentyp
description: 'Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.  Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt. Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien. Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden. Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen. '
localization_priority: Normal
ms.openlocfilehash: 6f923cdeb34ec0845d776a67f51db490256ec718
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640854"
---
# <a name="endpoint-resource-type"></a>Endpunkt-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.  Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt. Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien. Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden. Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen. 

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Endpunkte auflisten](../api/group-list-endpoints.md) |[endpoint](endpoint.md)-Sammlung| Ruft eine Endpunktobjektsammlung ab. |
|[Endpunkt abrufen](../api/endpoint-get.md) | [Endpunkt](endpoint.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des endpoint-Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| Funktion     | String  | Beschreibt die Fähigkeit, die diese Ressource zugeordnet ist. (z. B. Nachrichten, Unterhaltungen, usw.)  Nicht NULL-Werte zulässt. Schreibgeschützt. |
| id             | String  | Eindeutiger Bezeichner für den Endpunkt; -Taste. Lässt keine Nullwerte zu. Schreibgeschützt.|
| providerId     | String  | Id der das zugrunde liegende Dienst veröffentlichen. Lässt keine Nullwerte zu. Schreibgeschützt.|
| providerName   | String  | Name der Veröffentlichung der zugrunde liegende Dienst. Schreibgeschützt.|
| providerResourceId|String| Für Office 365-Gruppen ist dies auf einen bekannten Namen für die Ressource (z. B. Yammer.FeedURL usw.) festgelegt. Lässt keine Nullwerte zu. Schreibgeschützt.|
| uri            | String  | URL der veröffentlichten Ressource. Lässt keine Nullwerte zu. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen

Keine.


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Endpoint"
}-->

```json
{
  "capability": "String",
  "id": "String (identifier)",
  "providerId": "String",
  "providerName": "String",
  "providerResourceId": "String",
  "uri": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/endpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
