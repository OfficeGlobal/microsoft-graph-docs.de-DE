---
title: Ressourcentyp cartToClassAssociation
description: CartToClassAssociation Schulungsräume Gerät Toilettengebäude zuzuordnen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b832e4597b15f062289a086d068ea3da71d9f66a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395692"
---
# <a name="carttoclassassociation-resource-type"></a>Ressourcentyp cartToClassAssociation

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

CartToClassAssociation Schulungsräume Gerät Toilettengebäude zuzuordnen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Auflistung|Listeneigenschaften und Beziehungen der [CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekte.|
|[Abrufen von cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Lesen Sie Eigenschaften und Beziehungen des [CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts.|
|[Erstellen von cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Erstellen eines neuen [CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts.|
|[CartToClassAssociation löschen](../api/intune-deviceconfig-carttoclassassociation-delete.md)|Keine|Löscht eine [CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).|
|[CartToClassAssociation aktualisieren](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Aktualisieren Sie die Eigenschaften eines [CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität.|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|Version|Int32|Version der CartToClassAssociation.|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt).|
|description|Zeichenfolge|Admin bereitgestellte Beschreibung für die CartToClassAssociation.|
|deviceCartIds|Zeichenfolgenauflistung|Bezeichner des Geräts Toilettengebäude Klassen zugeordnet werden soll.|
|classroomIds|Zeichenfolgenauflistung|Die IDs der Schulungsräume Gerät Toilettengebäude zugeordnet werden soll.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cartToClassAssociation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "classroomIds": [
    "String"
  ]
}
```




