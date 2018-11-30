---
title: Ressourcentyp governanceResource
description: Stellt die Ressourcen, die von privilegierten Identity Management (PIM) verwaltet werden konnte. Für Azure Ressourcen können sie ein Abonnement, eine Ressourcengruppe und eine Ressource, z. B. einen virtuellen Computer, eine SQL-Datenbank sein.
ms.openlocfilehash: 9e47f1295f9498796d51414a0a97acbe51fe1aae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062421"
---
# <a name="governanceresource-resource-type"></a>Ressourcentyp governanceResource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Ressourcen, die von privilegierten Identity Management (PIM) verwaltet werden konnte. Für Azure Ressourcen können sie ein Abonnement, eine Ressourcengruppe und eine Ressource, z. B. einen virtuellen Computer, eine SQL-Datenbank sein.


## <a name="methods"></a>Methoden

| Methode          | Rückgabetyp |Beschreibung|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | [GovernanceResource](../resources/governanceresource.md) -Auflistung|Eine Auflistung von Ressourcen, denen der Requestor Zugriff auf hat aufgelistet.|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |Eigenschaften lesen und Beziehungen einer Ressource Entität nach Id angegeben.|

Nicht `POST`, `PUT`, `PATCH`, `DELETE` werden unterstützt, auf `roleDefinitions` Entität-Set für jetzt.

## <a name="properties"></a>Eigenschaften
| Eigenschaft          |Typ         |Beschreibung|
|:------------------|:----------|:----------|
|id                 |String     |Die Id der Ressource. Es ist im GUID-Format.|
|externalId           |String   |Die externe Id der Ressource, seiner ursprüngliche-Id in der externen Datenbank darstellt. Beispielsweise kann ein Abonnement Ressource externe Id "/ Abonnements/c14ae696-5e0c-4e5d-88cc-bef6637737ac" sein. |
|Typ               |Zeichenfolge     |Erforderlich. Der Ressourcentyp. Beispielsweise könnte der Typ für Azure Ressourcen sein "Abonnements", "ResourceGroup", "Microsoft.Sql/server".|
|displayName        |String     |Der Anzeigename der Ressource.|
|status             |String     |Der Status einer bestimmten Ressource. Beispielsweise könnte darstellen, ob die Ressource oder nicht gesperrt ist (Werte: `Active` / `Locked`). Hinweis: Diese Eigenschaft kann in der Zukunft verlängert werden, um weitere Szenarien unterstützen.|
|onboardDateTime|DateTimeOffset      |Es stellt das Datum / Uhrzeit, wann die Ressource beginnt von PIM verwaltet werden.|
|roleAssignmentCount|Int32      |Optional. Die Anzahl der rollenzuweisungen für die angegebene Ressource. Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=roleAssignmentCount` in der Abfrage.|
|roleDefinitionCount|Int32      |Optional. Die Anzahl der Rollendefinitionen für die angegebene Ressource. Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=roleDefinitionCount` in der Abfrage.|
|permissions|[governancePermission](../resources/governancepermission.md)      |Optional. Es stellt den Status des Antragstellers Zugriff auf die Ressource. Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=permissions` in der Abfrage.|

## <a name="relationships"></a>Beziehungen
| Beziehung   | Typ                                         |Beschreibung|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[GovernanceRoleAssignment](../resources/governanceroleassignment.md) -Auflistung|Die Auflistung von rollenzuweisungen für die Ressource.|
|roleDefinitions |[GovernanceRoleDefinition](../resources/governanceroledefinition.md) -Auflistung|Die Auflistung der Rolle Definitionen für die Ressource.|
|roleAssignmentRequests |[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Auflistung|Die Auflistung der Rolle Zuordnung Anforderungen für die Ressource.|
|roleSettings |[GovernanceRoleSetting](../resources/governancerolesetting.md) -Auflistung|Die Auflistung von Einstellungen für Serverrollen für die Ressource.|
|das übergeordnete          |[governanceResource](../resources/governanceresource.md)           |Schreibgeschützt. Die übergeordnete Ressource. für `pimforazurerbac` Szenario können sie das Abonnement die Ressource gehört zu darstellen.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceResource"
}-->
```json
{
  "id": "String (identifier)",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->