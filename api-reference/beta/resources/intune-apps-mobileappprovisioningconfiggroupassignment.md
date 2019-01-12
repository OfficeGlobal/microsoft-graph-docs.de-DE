---
title: Ressourcentyp mobileAppProvisioningConfigGroupAssignment
description: Enthält die Eigenschaften verwendet, um eine App-Bereitstellung Konfiguration einer Gruppe zuweisen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6996bf29776910d8af3da08d63003889b817cfbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912134"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a>Ressourcentyp mobileAppProvisioningConfigGroupAssignment

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält die Eigenschaften verwendet, um eine App-Bereitstellung Konfiguration einer Gruppe zuweisen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste mobileAppProvisioningConfigGroupAssignments](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Auflistung|Listeneigenschaften und Beziehungen der [MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekte.|
|[Abrufen von mobileAppProvisioningConfigGroupAssignment](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|Lesen Sie Eigenschaften und Beziehungen des [MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekts.|
|[Erstellen von mobileAppProvisioningConfigGroupAssignment](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|Erstellen eines neuen [MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekts.|
|[MobileAppProvisioningConfigGroupAssignment löschen](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|Keine|Löscht eine [MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).|
|[MobileAppProvisioningConfigGroupAssignment aktualisieren](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|Aktualisieren Sie die Eigenschaften eines [MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|targetGroupId|Zeichenfolge|Die ID der Gruppe der AAD, in der die app-Bereitstellung Konfiguration vorgesehen ist.|
|id|Zeichenfolge|Schlüssel der Entität|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppProvisioningConfigGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "String",
  "id": "String (identifier)"
}
```





