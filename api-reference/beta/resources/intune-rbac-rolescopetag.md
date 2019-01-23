---
title: Ressourcentyp roleScopeTag
description: Rolle Bereich Tag
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3a63ac05ea6161843aa1ad664a99003b7f69d38e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400564"
---
# <a name="rolescopetag-resource-type"></a>Ressourcentyp roleScopeTag

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




