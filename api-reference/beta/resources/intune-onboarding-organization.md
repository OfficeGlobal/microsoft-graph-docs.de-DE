---
title: organization-Ressourcentyp
description: Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
ms.openlocfilehash: e7e49e5676e412ea0e174b2e158b98efea8e0c7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061781"
---
# <a name="organization-resource-type"></a>organization-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Organisationen auflisten](../api/intune-onboarding-organization-list.md)|[organization](../resources/intune-onboarding-organization.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [organization](../resources/intune-onboarding-organization.md)-Objekte.|
|[Organisation abrufen](../api/intune-onboarding-organization-get.md)|[organization](../resources/intune-onboarding-organization.md)|Dient zum Lesen der Eigenschaften und Beziehungen des [organization](../resources/intune-onboarding-organization.md)-Objekts.|
|[Organisation aktualisieren](../api/intune-onboarding-organization-update.md)|[organization](../resources/intune-onboarding-organization.md)|Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.|
|[setMobileDeviceManagementAuthority-Aktion](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|Int32|Autorität für die Verwaltung mobiler Geräte festlegen|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Die GUID für das Objekt.|
|mobileDeviceManagementAuthority|[mdmAuthority](../resources/intune-onboarding-mdmauthority.md)|Autorität für die Verwaltung mobiler Geräte. Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.|
|certificateConnectorSetting|[certificateConnectorSetting](../resources/intune-onboarding-certificateconnectorsetting.md)|Connector-Einstellung Zertifikat.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 1024,
    "certExpiryTime": "String (timestamp)",
    "enrollmentError": "String",
    "lastConnectorConnectionTime": "String (timestamp)",
    "connectorVersion": "String",
    "lastUploadVersion": 1024
  }
}
```





