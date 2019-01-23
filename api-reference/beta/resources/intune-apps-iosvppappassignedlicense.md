---
title: Ressourcentyp iosVppAppAssignedLicense
description: iOS Volume Purchase Program lizenzzuweisung. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ff1d467dd0bd5ef34836d77f2f7dd034d877f1f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395657"
---
# <a name="iosvppappassignedlicense-resource-type"></a>Ressourcentyp iosVppAppAssignedLicense

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

iOS Volume Purchase Program lizenzzuweisung. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Auflistung|Listeneigenschaften und Beziehungen der [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekte.|
|[Abrufen von iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Lesen Sie Eigenschaften und Beziehungen des [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.|
|[Erstellen von iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Erstellen eines neuen [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.|
|[IosVppAppAssignedLicense löschen](../api/intune-apps-iosvppappassignedlicense-delete.md)|Keine|Löscht eine [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).|
|[IosVppAppAssignedLicense aktualisieren](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Aktualisieren Sie die Eigenschaften eines [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|userEmailAddress|Zeichenfolge|Die e-Mail-Adresse des Benutzers.|
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




