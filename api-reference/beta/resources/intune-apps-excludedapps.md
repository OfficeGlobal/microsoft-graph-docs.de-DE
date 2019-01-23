---
title: Ressourcentyp excludedApps
description: Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d3cd9a159597689a64070181640415a6ce2fc61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395678"
---
# <a name="excludedapps-resource-type"></a>Ressourcentyp excludedApps

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|access|Boolean|Der Wert für die If MS Office Access davon ausgeschlossen werden soll.|
|Excel-|Boolean|Der Wert für die If MS Office Excel davon ausgeschlossen werden soll.|
|Groove|Boolean|Der Wert für die If MS Office OneDrive for Business - Groove ausgeschlossen werden soll, oder nicht.|
|infoPath|Boolean|Der Wert für die If MS Office InfoPath davon ausgeschlossen werden soll.|
|Lync|Boolean|Der Wert für die If MS Office Skype for Business – Lync ausgeschlossen werden soll, oder nicht.|
|oneDrive|Boolean|Der Wert für die If MS Office OneDrive davon ausgeschlossen werden soll.|
|oneNote|Boolean|Der Wert für die If MS Office OneNote davon ausgeschlossen werden soll.|
|Outlook|Boolean|Der Wert für die If MS Office Outlook oder nicht ausgeschlossen werden soll.|
|powerPoint|Boolean|Der Wert für die If MS Office PowerPoint davon ausgeschlossen werden soll.|
|publisher|Boolean|Der Wert für die If MS Office Publisher davon ausgeschlossen werden soll.|
|SharePoint Designer|Boolean|Der Wert für die If MS Office SharePoint Designer davon ausgeschlossen werden soll.|
|Visio|Boolean|Der Wert für die If MS Office Visio davon ausgeschlossen werden soll.|
|Word|Boolean|Der Wert für die If MS Office Word davon ausgeschlossen werden soll.|

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




