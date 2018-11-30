---
title: Ressourcentyp excludedApps
description: Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.
ms.openlocfilehash: 05c1ed7f4789e1a27ddacf92dbd773b2f5a21847
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060566"
---
# <a name="excludedapps-resource-type"></a>Ressourcentyp excludedApps

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Zugriff|Boolesch|Der Wert für die If MS Office Access davon ausgeschlossen werden soll.|
|Excel-|Boolesch|Der Wert für die If MS Office Excel davon ausgeschlossen werden soll.|
|Groove|Boolesch|Der Wert für die If MS Office OneDrive for Business - Groove ausgeschlossen werden soll, oder nicht.|
|infoPath|Boolesch|Der Wert für die If MS Office InfoPath davon ausgeschlossen werden soll.|
|Lync|Boolesch|Der Wert für die If MS Office Skype for Business – Lync ausgeschlossen werden soll, oder nicht.|
|oneDrive|Boolesch|Der Wert für die If MS Office OneDrive davon ausgeschlossen werden soll.|
|oneNote|Boolesch|Der Wert für die If MS Office OneNote davon ausgeschlossen werden soll.|
|Outlook|Boolesch|Der Wert für die If MS Office Outlook oder nicht ausgeschlossen werden soll.|
|powerPoint|Boolesch|Der Wert für die If MS Office PowerPoint davon ausgeschlossen werden soll.|
|publisher|Boolesch|Der Wert für die If MS Office Publisher davon ausgeschlossen werden soll.|
|SharePoint Designer|Boolesch|Der Wert für die If MS Office SharePoint Designer davon ausgeschlossen werden soll.|
|Visio|Boolesch|Der Wert für die If MS Office Visio davon ausgeschlossen werden soll.|
|Word|Boolesch|Der Wert für die If MS Office Word davon ausgeschlossen werden soll.|

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





