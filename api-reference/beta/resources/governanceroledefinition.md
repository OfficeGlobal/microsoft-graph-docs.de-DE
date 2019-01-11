---
title: Ressourcentyp governanceRoleDefinition
description: Stellt die Rollendefinitionen. Für Azure Ressourcen können sie Azure RBAC-Rollen, wie Besitzer, Leser, Autor darstellen.
localization_priority: Normal
ms.openlocfilehash: 3f94dd1a741545760951875fbc064307823a65dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842450"
---
# <a name="governanceroledefinition-resource-type"></a>Ressourcentyp governanceRoleDefinition

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt. 


Stellt die Rollendefinitionen. Für Azure Ressourcen können sie Azure RBAC-Rollen, wie Besitzer, Leser, Autor darstellen.


## <a name="methods"></a>Methoden

| Methode          | Rückgabetyp |Beschreibung|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | [GovernanceRoleDefinition](../resources/governanceroledefinition.md) -Auflistung |Eine Auflistung von Rollendefinitionen für eine Ressource aufgelistet.|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Lesen Sie Eigenschaften und Beziehungen einer Rolle Definition Entität nach Id angegeben.|
Nicht `POST`, `PUT`, `PATCH`, `DELETE` wird auf unterstützt `roleDefinitions` Entität-Set für jetzt.
## <a name="properties"></a>Eigenschaften
| Eigenschaft  | Typ      |Beschreibung|
|:----|:----------|:----------|:----------|
|id         |String     |Die Id der Rollendefinition. |
|resourceId |Zeichenfolge     |Erforderlich. Die Id der Rollendefinition zugeordneten Ressource. |
|externalId   |String     |Die externe Id der Rollendefinition.|
|displayName|String     |Der Anzeigename der Rollendefinition.|
|subjectCount|Int32     |Optional. Die Anzahl der Themen, die die Rolle zugewiesen sind. Es stellt den Status des Antragstellers Zugriff auf die Ressource. Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=subjectCount` in der Abfrage.|
|eligibleAssignmentCount|Int32|Optional. Die Anzahl von zu auswählbaren rollenzuweisungen Rollendefinition zugeordnet. Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=eligibleAssignmentCount` in der Abfrage.|
|activeAssignmentCount|Int32    |Optional. Die Anzahl der aktiven rollenzuweisungen Rollendefinition zugeordnet.  Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=activeAssignmentCount` in der Abfrage.|


## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Schreibgeschützt. Die zugeordneten Ressource für die Rollendefinition.|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|Die Einstellung der zugehörige Rolle für die Rollendefinition.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
