---
title: mobileAppContent-Ressourcentyp
description: Enthält Inhaltseigenschaften für eine bestimmte App-Version. Jedes mobileAppContent-Objekt kann mehrere mobileAppContentFile-Objekte haben.
author: tfitzmac
ms.openlocfilehash: 8cc5bd6e3c7aa5f08236d2662821a9a5d03707d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360347"
---
# <a name="mobileappcontent-resource-type"></a>mobileAppContent-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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
|containedApps|[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Auflistung|Die Auflistung der enthaltenen apps in einer MobileLobApp fungiert als Paket.|

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





