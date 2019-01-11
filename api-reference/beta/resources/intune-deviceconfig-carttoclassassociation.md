---
title: Ressourcentyp cartToClassAssociation
description: CartToClassAssociation Schulungsräume Gerät Toilettengebäude zuzuordnen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 02a7d04b40d4d984f98f04eb653ee45ed436d099
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868033"
---
# <a name="carttoclassassociation-resource-type"></a>Ressourcentyp cartToClassAssociation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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
|deviceCartIds|Collection von Objekten des Typs „String“|Bezeichner des Geräts Toilettengebäude Klassen zugeordnet werden soll.|
|classroomIds|Collection von Objekten des Typs „String“|Die IDs der Schulungsräume Gerät Toilettengebäude zugeordnet werden soll.|

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





