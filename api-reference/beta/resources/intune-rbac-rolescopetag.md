---
title: Ressourcentyp roleScopeTag
description: Rolle Bereich Tag
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 609d4202069f6e4258c9824a65b72ab769c365b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981854"
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
|[RoleScopeTag löschen](../api/intune-rbac-rolescopetag-delete.md)|Keine|Löscht eine [RoleScopeTag](../resources/intune-rbac-rolescopetag.md).|
|[RoleScopeTag aktualisieren](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Aktualisieren Sie die Eigenschaften eines [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Er ist schreibgeschützt und wird automatisch generiert.|
|displayName|Zeichenfolge|Das Display oder den Anzeigenamen des Tags Bereich Rolle.|
|description|Zeichenfolge|Beschreibung des Tags Bereich Rolle.|

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





