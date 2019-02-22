---
title: cartToClassAssociation-Ressourcentyp
description: CartToClassAssociation zum Zuordnen von Geräte Körben zu Schulungsräumen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 228a3bfc873fdaf1fbd77e51a79ca184c2416d7c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156595"
---
# <a name="carttoclassassociation-resource-type"></a>cartToClassAssociation-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

CartToClassAssociation zum Zuordnen von Geräte Körben zu Schulungsräumen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[CartToClassAssociations aufListen](../api/intune-deviceconfig-carttoclassassociation-list.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekte.|
|[CartToClassAssociation abrufen](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Lesen von Eigenschaften und Beziehungen des [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts.|
|[CartToClassAssociation erstellen](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Erstellen eines neuen [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts.|
|[CartToClassAssociation löschen](../api/intune-deviceconfig-carttoclassassociation-delete.md)|Keine|Löscht eine [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).|
|[CartToClassAssociation aktualisieren](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Aktualisieren der Eigenschaften eines [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität.|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|Version|Int32|Version von CartToClassAssociation.|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt).|
|description|Zeichenfolge|Der Administrator hat die Beschreibung des CartToClassAssociation bereitgestellt.|
|deviceCartIds|String collection|Bezeichner von Gerätewagen, die Klassen zugeordnet werden sollen.|
|classroomIds|String collection|Bezeichner der Unterrichtsräume, die mit Geräte Körben verknüpft werden sollen.|

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




