---
title: inferenceClassification-Ressourcentyp
description: 'Klassifizierung der Nachrichten eines Benutzers, um den Fokus auf die Nachrichten zu legen, die für den Benutzer relevanter oder wichtiger sind. '
localization_priority: Normal
ms.openlocfilehash: f06177db9907deb3be38c2cdab82669764503cd6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510414"
---
# <a name="inferenceclassification-resource-type"></a>inferenceClassification-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Klassifizierung der Nachrichten eines Benutzers, um den Fokus auf die Nachrichten zu legen, die für den Benutzer relevanter oder wichtiger sind. 

Weitere Informationen finden Sie unter [Verwalten eines Posteingang mit Fokus](manage-focused-inbox.md).


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|inferenceClassificationOverride erstellen |[inferenceClassificationOverride](inferenceclassificationoverride.md)| Erstellen einer Außerkraftsetzung für einen Absender, der durch eine SMTP-Adresse identifiziert wird. Künftige Nachrichten von dieser SMTP-Adresse werden durchgängig klassifiziert wie in der Außerkraftsetzung angegeben.|
|Außerkraftsetzungen auflisten |inferenceClassificationOverride-Sammlung| Dient zum Abrufen der Außerkraftsetzungen, die ein Benutzer eingerichtet hat, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string| Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Außerkraftsetzungen|inferenceClassificationOverride-Sammlung| Eine Reihe von Außerkraftsetzungen für einen Benutzer, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren: `focused` oder `other`. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassification"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/inferenceclassification.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
