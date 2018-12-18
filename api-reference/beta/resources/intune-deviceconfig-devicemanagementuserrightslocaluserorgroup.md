---
title: Ressourcentyp deviceManagementUserRightsLocalUserOrGroup
description: Stellt Informationen für einen lokalen Benutzer oder eine Gruppe, die zum Festlegen von Benutzerrechten an.
author: tfitzmac
ms.openlocfilehash: baabd2f3bb9e3bce44d172cd83f61f57c5c2c98d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303731"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>Ressourcentyp deviceManagementUserRightsLocalUserOrGroup

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt Informationen für einen lokalen Benutzer oder eine Gruppe, die zum Festlegen von Benutzerrechten an.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|String|Der Name des lokalen Benutzers oder der Gruppe.|
|description|String|Der Admin-Beschreibung des lokalen Benutzers oder der Gruppe.|
|securityIdentifier|String|Die Sicherheits-ID der lokalen Benutzer oder Gruppen (z. B. * S-1-5-32-544).|

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





