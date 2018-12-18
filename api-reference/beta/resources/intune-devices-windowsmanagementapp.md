---
title: Ressourcentyp windowsManagementApp
description: Windows Management-app-Entität.
author: tfitzmac
ms.openlocfilehash: 641538644dc313234e27b0f518a26d8a38c612b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346424"
---
# <a name="windowsmanagementapp-resource-type"></a>Ressourcentyp windowsManagementApp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Windows Management-app-Entität.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von windowsManagementApp](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts.|
|[WindowsManagementApp aktualisieren](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Aktualisieren Sie die Eigenschaften eines [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die Windows Management-app|
|availableVersion|String|Windows Management app verfügbare Version.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|healthSummary|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)|Zusammenfassung für Windows Management app Integrität.|
|healthStates|[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Auflistung|Die Liste der Zustände für installierten Windows Management-Anwendung.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```





