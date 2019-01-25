---
title: Ressourcentyp governanceResource
description: Stellt die Ressourcen, die von privilegierten Identity Management (PIM) verwaltet werden konnte. Für Azure Ressourcen können sie ein Abonnement, eine Ressourcengruppe und eine Ressource, z. B. einen virtuellen Computer, eine SQL-Datenbank sein.
localization_priority: Normal
ms.openlocfilehash: 92a738350a47cc9eaf436382d020330fac89db1f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528557"
---
# <a name="governanceresource-resource-type"></a>Ressourcentyp governanceResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die Ressourcen, die von privilegierten Identity Management (PIM) verwaltet werden konnte. Für Azure Ressourcen können sie ein Abonnement, eine Ressourcengruppe und eine Ressource, z. B. einen virtuellen Computer, eine SQL-Datenbank sein.


## <a name="methods"></a>Methoden

| Methode          | Rückgabetyp |Beschreibung|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | [GovernanceResource](../resources/governanceresource.md) -Auflistung|Eine Auflistung von Ressourcen, denen der Requestor Zugriff auf hat aufgelistet.|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |Eigenschaften lesen und Beziehungen einer Ressource Entität nach Id angegeben.|
|Register | |Registrieren einer nicht verwalteten Azure-Abonnement oder Management-Gruppe zum PIM-Dienst. |

Nicht `POST`, `PUT`, `PATCH`, `DELETE` werden unterstützt, auf `roleDefinitions` Entität-Set für jetzt.

## <a name="properties"></a>Eigenschaften
| Eigenschaft          |Typ         |Beschreibung|
|:------------------|:----------|:----------|
|id                 |string     |Die ID der Ressource. Es ist im GUID-Format.|
|externalId           |String   |Die externe Id der Ressource, die im externen System seine ursprüngliche Id darstellt. Beispielsweise kann ein Abonnement Ressource externe Id "/ Abonnements/c14ae696-5e0c-4e5d-88cc-bef6637737ac" sein. |
|type               |Zeichenfolge     |Erforderlich. Ressourcentyp Beispielsweise könnte der Typ für Azure Ressourcen sein "Abonnements", "ResourceGroup", "Microsoft.Sql/server".|
|displayName        |String     |Der Anzeigename der Ressource.|
|status             |Zeichenfolge     |Der Status einer bestimmten Ressource. Beispielsweise könnte darstellen, ob die Ressource oder nicht gesperrt ist (Werte: `Active` / `Locked`). Hinweis: Diese Eigenschaft kann in der Zukunft verlängert werden, um weitere Szenarien unterstützen.|
|registeredDateTime|DateTimeOffset      |Stellt das Datum / Uhrzeit, wann die Ressource in PIM registriert ist.|
|registeredRoot|String      |Die ExternalId Stamm Bereichs, der Ressource, die im PIM registriert ist. Der Stammgültigkeitsbereich kann die übergeordnete, Bandrotationsschema oder einer höheren Vorgänger Ressourcen sein.|
|roleAssignmentCount|Int32      |Optional. Die Anzahl der rollenzuweisungen für die angegebene Ressource. Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=roleAssignmentCount` in der Abfrage.|
|roleDefinitionCount|Int32      |Optional. Die Anzahl der Rollendefinitionen für die angegebene Ressource. Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=roleDefinitionCount` in der Abfrage.|
|Berechtigungen|[governancePermission](../resources/governancepermission.md)      |Optional. Es stellt den Status des Antragstellers Zugriff auf die Ressource. Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=permissions` in der Abfrage.|

## <a name="relationships"></a>Beziehungen
| Beziehung   | Typ                                         |Beschreibung|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[GovernanceRoleAssignment](../resources/governanceroleassignment.md) -Auflistung|Die Auflistung von rollenzuweisungen für die Ressource.|
|roleDefinitions |[GovernanceRoleDefinition](../resources/governanceroledefinition.md) -Auflistung|Die Auflistung der Rolle Definitionen für die Ressource.|
|roleAssignmentRequests |[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Auflistung|Die Auflistung der Rolle Zuordnung Anforderungen für die Ressource.|
|roleSettings |[GovernanceRoleSetting](../resources/governancerolesetting.md) -Auflistung|Die Auflistung von Einstellungen für Serverrollen für die Ressource.|
|Parent          |[governanceResource](../resources/governanceresource.md)           |Schreibgeschützt. Die übergeordnete Ressource. für `pimforazurerbac` Szenario können sie das Abonnement die Ressource gehört zu darstellen.|

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
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
