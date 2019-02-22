---
title: mobileAppContent-Ressourcentyp
description: Enthält Inhaltseigenschaften für eine bestimmte App-Version. Jedes mobileAppContent-Objekt kann mehrere mobileAppContentFile-Objekte haben.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 82c2100fb7bd9e906bf6cf9092d3df88865c26e8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153445"
---
# <a name="mobileappcontent-resource-type"></a>mobileAppContent-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Inhaltseigenschaften für eine bestimmte App-Version. Jedes mobileAppContent-Objekt kann mehrere mobileAppContentFile-Objekte haben.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[mobileAppContents auflisten](../api/intune-apps-mobileappcontent-list.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekte.|
|[mobileAppContent abrufen](../api/intune-apps-mobileappcontent-get.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Lesen von Eigenschaften und Beziehungen des [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.|
|[mobileAppContent erstellen](../api/intune-apps-mobileappcontent-create.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Erstellen eines neuen [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.|
|[mobileAppContent löschen](../api/intune-apps-mobileappcontent-delete.md)|Keine|Löscht eine [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Ressource.|
|[Update mobileAppContent](../api/intune-apps-mobileappcontent-update.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Aktualisieren der Eigenschaften eines [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Die Version des App-Inhalts.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|files|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Sammlung|Die Liste der Dateien für diese App-Inhaltsversion.|
|containedApps|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Sammlung|Die Sammlung der enthaltenen apps in einem MobileLobApp, das als Paket fungiert.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```




