---
title: Ressourcentyp windowsAssignedAccessProfile
description: Profil zugewiesenen Access für Windows.
author: tfitzmac
ms.openlocfilehash: 6b01f362c31f6e2791a00d8ff02a7ecd5b798e3c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328791"
---
# <a name="windowsassignedaccessprofile-resource-type"></a>Ressourcentyp windowsAssignedAccessProfile

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Profil zugewiesenen Access für Windows.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windowsAssignedAccessProfiles](../api/intune-deviceconfig-windowsassignedaccessprofile-list.md)|[WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) -Auflistung|Listeneigenschaften und Beziehungen der [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) -Objekte.|
|[Abrufen von windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-get.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) -Objekts.|
|[Erstellen von windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-create.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|Erstellen eines neuen [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) -Objekts.|
|[WindowsAssignedAccessProfile löschen](../api/intune-deviceconfig-windowsassignedaccessprofile-delete.md)|Keines|Löscht eine [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).|
|[WindowsAssignedAccessProfile aktualisieren](../api/intune-deviceconfig-windowsassignedaccessprofile-update.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|Aktualisieren Sie die Eigenschaften eines [WindowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|Profilname|String|Dies ist ein Anzeigename zur Identifizierung einer Gruppe von Anwendungen, das Layout von diese apps auf das Startmenü und die Benutzer, die diese Konfiguration Kiosk zugewiesen ist.|
|showTaskBar|Boolesch|Mit dieser Einstellung kann den Administrator an, ob der Taskleiste oder nicht angezeigt wird.|
|appUserModelIds|Collection von Objekten des Typs „String“|Dies sind die einzige Windows Store-Apps, die über das Startmenü gestartet werden.|
|desktopAppPaths|Collection von Objekten des Typs „String“|Dies sind die Pfade der Desktop-Apps, die auf das Startmenü zur Verfügung stehen, und die einzige apps des Benutzers kann zu starten.|
|userAccounts|Collection von Objekten des Typs „String“|Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt werden.|
|startMenuLayoutXml|Binär|Ermöglicht Administratoren das Standardlayout Start außer Kraft gesetzt, und verhindert, dass den Benutzer geändert wird.Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert. XML muss im Binärformat sein.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAssignedAccessProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "showTaskBar": true,
  "appUserModelIds": [
    "String"
  ],
  "desktopAppPaths": [
    "String"
  ],
  "userAccounts": [
    "String"
  ],
  "startMenuLayoutXml": "binary"
}
```





