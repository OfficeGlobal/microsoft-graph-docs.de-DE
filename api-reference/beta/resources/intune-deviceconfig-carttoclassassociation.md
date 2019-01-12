---
title: Ressourcentyp cartToClassAssociation
description: CartToClassAssociation Schulungsräume Gerät Toilettengebäude zuzuordnen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38d9b940dd3e7a5450854f29ba69b2eac69e2a45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943935"
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





