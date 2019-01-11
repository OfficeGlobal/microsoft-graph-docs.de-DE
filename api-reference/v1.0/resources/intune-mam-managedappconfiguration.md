---
title: managedAppConfiguration-Ressourcentyp
description: Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b3acf921f76e34e21427364ef84d1647cc7d0f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861320"
---
# <a name="managedappconfiguration-resource-type"></a>managedAppConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Konfiguration wird verwendet, um eine Reihe benutzerdefinierter Einstellungen in der vorliegenden Form an Apps für Benutzer zu übermitteln, auf die die Konfiguration beschränkt wurde.

Erbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedAppConfigurations auflisten](../api/intune-mam-managedappconfiguration-list.md)|[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekte.|
|[managedAppConfiguration abrufen](../api/intune-mam-managedappconfiguration-get.md)|[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Anzeigename der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|String|Beschreibung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|String|Schlüssel der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|Version|String|Version der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|customSettings|[keyValuePair](../resources/intune-mam-keyvaluepair.md)-Sammlung|Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



