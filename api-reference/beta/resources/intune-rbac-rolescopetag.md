---
title: Ressourcentyp roleScopeTag
description: Rolle Bereich Tag
ms.openlocfilehash: 9be1f1307243c18e10f8e6dfc3f302502cdb54a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061426"
---
# <a name="rolescopetag-resource-type"></a>Ressourcentyp roleScopeTag

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Rolle Bereich Tag
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste roleScopeTags](../api/intune-rbac-rolescopetag-list.md)|[RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Auflistung|Listeneigenschaften und Beziehungen der [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekte.|
|[Abrufen von roleScopeTag](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Lesen Sie Eigenschaften und Beziehungen des [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.|
|[Erstellen von roleScopeTag](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Erstellen eines neuen [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.|
|[RoleScopeTag löschen](../api/intune-rbac-rolescopetag-delete.md)|Keines|Löscht eine [RoleScopeTag](../resources/intune-rbac-rolescopetag.md).|
|[RoleScopeTag aktualisieren](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Aktualisieren Sie die Eigenschaften eines [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Er ist schreibgeschützt und wird automatisch generiert.|
|displayName|String|Das Display oder den Anzeigenamen des Tags Bereich Rolle.|
|description|String|Beschreibung des Tags Bereich Rolle.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```




