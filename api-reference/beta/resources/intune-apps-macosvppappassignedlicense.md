---
title: Ressourcentyp macOsVppAppAssignedLicense
description: Mac OS Volume Purchase Program Lizenz Zuordnung. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c3a029d0f0aca7ab295f34d108b8bf61bdc17dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430005"
---
# <a name="macosvppappassignedlicense-resource-type"></a>Ressourcentyp macOsVppAppAssignedLicense

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Mac OS Volume Purchase Program Lizenz Zuordnung. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste macOsVppAppAssignedLicenses](../api/intune-apps-macosvppappassignedlicense-list.md)|[MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Auflistung|Listeneigenschaften und Beziehungen der [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekte.|
|[Abrufen von macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-get.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Lesen Sie Eigenschaften und Beziehungen des [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.|
|[Erstellen von macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-create.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Erstellen eines neuen [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.|
|[MacOsVppAppAssignedLicense löschen](../api/intune-apps-macosvppappassignedlicense-delete.md)|Keine|Löscht eine [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).|
|[MacOsVppAppAssignedLicense aktualisieren](../api/intune-apps-macosvppappassignedlicense-update.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Aktualisieren Sie die Eigenschaften eines [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.|

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
  "@odata.type": "microsoft.graph.macOsVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```




