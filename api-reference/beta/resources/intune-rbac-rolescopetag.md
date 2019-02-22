---
title: roleScopeTag-Ressourcentyp
description: Rollenbereich-Tag
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8c7bfb12172f6ae99f14a65647a7a6ab8955fef
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159423"
---
# <a name="rolescopetag-resource-type"></a>roleScopeTag-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Rollenbereich-Tag

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[RoleScopeTags aufListen](../api/intune-rbac-rolescopetag-list.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekte.|
|[RoleScopeTag abrufen](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Lesen von Eigenschaften und Beziehungen des [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.|
|[RoleScopeTag erstellen](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Erstellen eines neuen [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.|
|[RoleScopeTag löschen](../api/intune-rbac-rolescopetag-delete.md)|Keine|Löscht eine [roleScopeTag](../resources/intune-rbac-rolescopetag.md).|
|[RoleScopeTag aktualisieren](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Aktualisieren der Eigenschaften eines [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Er ist schreibgeschützt und wird automatisch generiert.|
|displayName|Zeichenfolge|Die Anzeige oder der angezeigte Name des Rollenbereichs Tags.|
|description|Zeichenfolge|Beschreibung des Rollenbereichs Tags.|

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




