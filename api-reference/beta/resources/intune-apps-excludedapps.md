---
title: excludedApps-Ressourcentyp
description: Enthält Eigenschaften für ausgeschlossene Office365-apps.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ba3e53a26ff71dde2d5a95fde811e42ba2ccb99
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154026"
---
# <a name="excludedapps-resource-type"></a>excludedApps-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für ausgeschlossene Office365-apps.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|access|Boolescher Wert|Der Wert für, wenn MS Office Access ausgeschlossen werden soll oder nicht.|
|Excel|Boolescher Wert|Der Wert für, wenn MS Office Excel ausgeschlossen werden soll oder nicht.|
|Groove|Boolescher Wert|Der Wert für IF MS Office OneDrive for Business-Groove sollte ausgeschlossen werden oder nicht.|
|infoPath|Boolescher Wert|Der Wert für, wenn MS Office InfoPath ausgeschlossen werden soll oder nicht.|
|lync|Boolescher Wert|Der Wert für, wenn MS Office Skype for Business-lync ausgeschlossen werden soll oder nicht.|
|oneDrive|Boolescher Wert|Der Wert für, wenn MS Office OneDrive ausgeschlossen werden soll oder nicht.|
|oneNote|Boolescher Wert|Der Wert für, wenn MS Office OneNote ausgeschlossen werden soll oder nicht.|
|outlook|Boolescher Wert|Der Wert für, wenn MS Office Outlook ausgeschlossen werden soll oder nicht.|
|Kulissen|Boolescher Wert|Der Wert für IF MS Office PowerPoint sollte ausgeschlossen werden oder nicht.|
|publisher|Boolescher Wert|Der Wert für, wenn MS Office Publisher ausgeschlossen werden soll oder nicht.|
|sharePointDesigner|Boolescher Wert|Der Wert für, wenn MS Office SharePointDesigner ausgeschlossen werden soll oder nicht.|
|Visio|Boolescher Wert|Der Wert für, wenn MS Office Visio ausgeschlossen werden soll oder nicht.|
|Wort|Boolescher Wert|Der Wert für, wenn MS Office Word ausgeschlossen werden soll oder nicht.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "excel": true,
  "groove": true,
  "infoPath": true,
  "lync": true,
  "oneDrive": true,
  "oneNote": true,
  "outlook": true,
  "powerPoint": true,
  "publisher": true,
  "sharePointDesigner": true,
  "visio": true,
  "word": true
}
```




