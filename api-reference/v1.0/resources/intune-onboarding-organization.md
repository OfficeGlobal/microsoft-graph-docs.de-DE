---
title: organization-Ressourcentyp
description: Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e1afa1ded131844f687fa2dbad1a8e07639b264
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250054"
---
# <a name="organization-resource-type"></a>organization-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|Zeichenfolge|Die GUID für das Objekt.|
|mobileDeviceManagementAuthority|[mdmAuthority](../resources/intune-onboarding-mdmauthority.md)|Autorität für die Verwaltung mobiler Geräte. Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.|

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
  "mobileDeviceManagementAuthority": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->



