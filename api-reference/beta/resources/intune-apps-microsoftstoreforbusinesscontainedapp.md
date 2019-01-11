---
title: Ressourcentyp microsoftStoreForBusinessContainedApp
description: Eine Klasse, die eine enthaltene eine MicrosoftStoreForBusinessApp-app darstellt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f783475e2f1f49745b29903689e75d854c233352
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876972"
---
# <a name="microsoftstoreforbusinesscontainedapp-resource-type"></a>Ressourcentyp microsoftStoreForBusinessContainedApp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine Klasse, die eine enthaltene eine MicrosoftStoreForBusinessApp-app darstellt.

Erbt vom [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste microsoftStoreForBusinessContainedApps](../api/intune-apps-microsoftstoreforbusinesscontainedapp-list.md)|[MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Auflistung|Listeneigenschaften und Beziehungen der [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekte.|
|[Abrufen von microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-get.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|Lesen Sie Eigenschaften und Beziehungen des [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts.|
|[Erstellen von microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-create.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|Erstellen eines neuen [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts.|
|[MicrosoftStoreForBusinessContainedApp löschen](../api/intune-apps-microsoftstoreforbusinesscontainedapp-delete.md)|Keine|Löscht eine [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).|
|[MicrosoftStoreForBusinessContainedApp aktualisieren](../api/intune-apps-microsoftstoreforbusinesscontainedapp-update.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|Aktualisieren Sie die Eigenschaften eines [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|
|appUserModelId|String|Die app Benutzer Modell-ID der app enthaltenen von einer MicrosoftStoreForBusinessApp.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```





