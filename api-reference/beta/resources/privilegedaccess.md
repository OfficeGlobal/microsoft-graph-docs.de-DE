---
title: Ressourcentyp privilegedAccess
description: " beispielsweise `privilegedAccess/azureResources` PIM Verwalten von Azure Ressourcen Systemzugriff darstellt."
localization_priority: Normal
ms.openlocfilehash: f4166fb539d627730c68c7e039fd8d672ff4c785
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810052"
---
# <a name="privilegedaccess-resource-type"></a>Ressourcentyp privilegedAccess

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Gruppe von Funktionen, die vom Dienst privilegierten Identity Management (PIM) bereitgestellt. Unterschiedliche Instanzen von `privilegedAccess` darstellen von anderen Anbietern von PIM; verwaltet werden beispielsweise `privilegedAccess/azureResources` PIM Verwalten von Azure Ressourcen Systemzugriff darstellt.


`privilegedAccess`Jetzt ist schreibgeschützt. Nicht `POST`, `PUT`, `PATCH`, oder `DELETE` Vorgänge werden unterstützt, auf die `privilegedAccess` Entität festlegen.

## <a name="properties"></a>Eigenschaften
| Eigenschaft  | Typ      |Beschreibung|
|:----------|:----------|:----------|
|id         |String     |Die Id des Anbieters von PIM verwaltet werden.|
|displayName|String     |Der Anzeigename des Anbieters von PIM verwaltet werden.|


## <a name="relationships"></a>Beziehungen
| Beziehung   | Typ                                         |Beschreibung|
|:---------------|:---------------------------------------------|:----------|
|resources       |[GovernanceResource](../resources/governanceresource.md) -Auflistung            |Eine Auflistung von Ressourcen für den Anbieter.|
|roleAssignments |[GovernanceRoleAssignment](../resources/governanceroleassignment.md) -Auflistung|Eine Auflistung von rollenzuweisungen für den Anbieter.|
|roleDefinitions |[GovernanceRoleDefinition](../resources/governanceroledefinition.md) -Auflistung|Eine Auflistung von Definitionen für den Anbieter Rolle.|
|roleAssignmentRequests |[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Auflistung|Eine Auflistung von Role Assignment-Anforderungen für den Anbieter.|
|roleSettings |[GovernanceRoleSetting](../resources/governancerolesetting.md) -Auflistung|Eine Auflistung von Einstellungen für Serverrollen für den Anbieter.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedAccess"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
