---
title: excludedApps-Ressourcentyp
description: Enthält Eigenschaften für ausgeschlossene Office365-apps.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dee0d5328f1f69c95159116bf913bc2abb959d7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571690"
---
# <a name="excludedapps-resource-type"></a>excludedApps-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für ausgeschlossene Office365-apps.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Access|Boolesch|Der Wert für, wenn MS Office Access ausgeschlossen werden soll oder nicht.|
|Excel|Boolesch|Der Wert für, wenn MS Office Excel ausgeschlossen werden soll oder nicht.|
|Groove|Boolesch|Der Wert für IF MS Office OneDrive for Business-Groove sollte ausgeschlossen werden oder nicht.|
|infoPath|Boolesch|Der Wert für, wenn MS Office InfoPath ausgeschlossen werden soll oder nicht.|
|lync|Boolesch|Der Wert für, wenn MS Office Skype for Business-lync ausgeschlossen werden soll oder nicht.|
|oneDrive|Boolesch|Der Wert für, wenn MS Office OneDrive ausgeschlossen werden soll oder nicht.|
|oneNote|Boolesch|Der Wert für, wenn MS Office OneNote ausgeschlossen werden soll oder nicht.|
|outlook|Boolesch|Der Wert für, wenn MS Office Outlook ausgeschlossen werden soll oder nicht.|
|Kulissen|Boolesch|Der Wert für IF MS Office PowerPoint sollte ausgeschlossen werden oder nicht.|
|publisher|Boolesch|Der Wert für, wenn MS Office Publisher ausgeschlossen werden soll oder nicht.|
|sharePointDesigner|Boolesch|Der Wert für, wenn MS Office SharePointDesigner ausgeschlossen werden soll oder nicht.|
|Teams|Boolesch|Der Wert für IF-MS Office Teams sollte ausgeschlossen werden oder nicht.|
|Visio|Boolesch|Der Wert für, wenn MS Office Visio ausgeschlossen werden soll oder nicht.|
|Wort|Boolesch|Der Wert für, wenn MS Office Word ausgeschlossen werden soll oder nicht.|

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
  "teams": true,
  "visio": true,
  "word": true
}
```




