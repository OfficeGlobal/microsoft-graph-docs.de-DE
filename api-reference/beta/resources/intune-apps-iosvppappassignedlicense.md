---
title: iosVppAppAssignedLicense-Ressourcentyp
description: iOS Volume Purchase Program-Lizenzzuweisung. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3499f3cfb1b15c76dbd70ec1a0634367c3107f87
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169335"
---
# <a name="iosvppappassignedlicense-resource-type"></a>iosVppAppAssignedLicense-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

iOS Volume Purchase Program-Lizenzzuweisung. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[IosVppAppAssignedLicenses aufListen](../api/intune-apps-iosvppappassignedlicense-list.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekte.|
|[IosVppAppAssignedLicense abrufen](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Lesen von Eigenschaften und Beziehungen des [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.|
|[IosVppAppAssignedLicense erstellen](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Erstellen eines neuen [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.|
|[IosVppAppAssignedLicense löschen](../api/intune-apps-iosvppappassignedlicense-delete.md)|Keine|Löscht eine [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).|
|[IosVppAppAssignedLicense aktualisieren](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Aktualisieren der Eigenschaften eines [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|userEmailAddress|Zeichenfolge|Die Benutzer-e-Mail-Adresse.|
|userId|Zeichenfolge|Die Benutzer-ID.|
|userName|Zeichenfolge|Der Benutzername.|
|userPrincipalName|Zeichenfolge|Der Benutzerprinzipalname.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```




