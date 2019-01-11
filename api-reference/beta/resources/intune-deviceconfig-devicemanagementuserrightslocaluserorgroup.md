---
title: Ressourcentyp deviceManagementUserRightsLocalUserOrGroup
description: Stellt Informationen für einen lokalen Benutzer oder eine Gruppe, die zum Festlegen von Benutzerrechten an.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d795e2b259c71612b1d0720796b6ad76145bb36d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885741"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>Ressourcentyp deviceManagementUserRightsLocalUserOrGroup

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt Informationen für einen lokalen Benutzer oder eine Gruppe, die zum Festlegen von Benutzerrechten an.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|Zeichenfolge|Der Name des lokalen Benutzers oder der Gruppe.|
|description|Zeichenfolge|Der Admin-Beschreibung des lokalen Benutzers oder der Gruppe.|
|securityIdentifier|Zeichenfolge|Die Sicherheits-ID der lokalen Benutzer oder Gruppen (z. B. * S-1-5-32-544).|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





