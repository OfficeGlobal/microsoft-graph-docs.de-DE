---
title: macOsVppAppAssignedLicense-Ressourcentyp
description: Mac OS-Lizenzzuweisung für das Volume Purchase-Programm. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8c7d8eea98c92ae1a041b8220c171d62fceb385
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158891"
---
# <a name="macosvppappassignedlicense-resource-type"></a>macOsVppAppAssignedLicense-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mac OS-Lizenzzuweisung für das Volume Purchase-Programm. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MacOsVppAppAssignedLicenses aufListen](../api/intune-apps-macosvppappassignedlicense-list.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekte.|
|[MacOsVppAppAssignedLicense abrufen](../api/intune-apps-macosvppappassignedlicense-get.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Lesen von Eigenschaften und Beziehungen des [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.|
|[MacOsVppAppAssignedLicense erstellen](../api/intune-apps-macosvppappassignedlicense-create.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Erstellen eines neuen [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.|
|[MacOsVppAppAssignedLicense löschen](../api/intune-apps-macosvppappassignedlicense-delete.md)|Keine|Löscht eine [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).|
|[MacOsVppAppAssignedLicense aktualisieren](../api/intune-apps-macosvppappassignedlicense-update.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Aktualisieren der Eigenschaften eines [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.|

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




