---
title: Ressourcentyp excludedApps
description: Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90216c639d36a989b2fad5dbdc1adbd11fe46ede
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943949"
---
# <a name="excludedapps-resource-type"></a>Ressourcentyp excludedApps

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|access|Boolescher Wert|Der Wert für die If MS Office Access davon ausgeschlossen werden soll.|
|Excel-|Boolescher Wert|Der Wert für die If MS Office Excel davon ausgeschlossen werden soll.|
|Groove|Boolescher Wert|Der Wert für die If MS Office OneDrive for Business - Groove ausgeschlossen werden soll, oder nicht.|
|infoPath|Boolescher Wert|Der Wert für die If MS Office InfoPath davon ausgeschlossen werden soll.|
|Lync|Boolescher Wert|Der Wert für die If MS Office Skype for Business – Lync ausgeschlossen werden soll, oder nicht.|
|oneDrive|Boolescher Wert|Der Wert für die If MS Office OneDrive davon ausgeschlossen werden soll.|
|oneNote|Boolescher Wert|Der Wert für die If MS Office OneNote davon ausgeschlossen werden soll.|
|Outlook|Boolescher Wert|Der Wert für die If MS Office Outlook oder nicht ausgeschlossen werden soll.|
|powerPoint|Boolescher Wert|Der Wert für die If MS Office PowerPoint davon ausgeschlossen werden soll.|
|publisher|Boolescher Wert|Der Wert für die If MS Office Publisher davon ausgeschlossen werden soll.|
|SharePoint Designer|Boolescher Wert|Der Wert für die If MS Office SharePoint Designer davon ausgeschlossen werden soll.|
|Visio|Boolescher Wert|Der Wert für die If MS Office Visio davon ausgeschlossen werden soll.|
|Word|Boolescher Wert|Der Wert für die If MS Office Word davon ausgeschlossen werden soll.|

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





