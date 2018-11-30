---
title: Endpunkt-Ressourcentyp
description: 'Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.  Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt. Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien. Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden. Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen. '
ms.openlocfilehash: 8d95cef8e25095512e94d5aed5ec7540562862bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059776"
---
# <a name="endpoint-resource-type"></a>Endpunkt-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.  Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt. Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien. Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden. Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen. 

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Endpunkte auflisten](../api/group-list-endpoints.md) |[Endpunkt](endpoint.md) -Auflistung| Rufen Sie eine Auflistung der Endpunkt-Objekts. |
|[Get-Endpunkt](../api/endpoint-get.md) | [Endpunkt](endpoint.md) |Lesen Sie Eigenschaften und Beziehungen eines Endpunkts-Objekts.|

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
<!-- {
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->