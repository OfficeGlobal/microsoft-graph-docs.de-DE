---
title: deviceAndAppManagementRoleAssignment-Ressourcentyp
description: Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.
author: tfitzmac
ms.openlocfilehash: c8226f632699237fc30008fce844388f96983601
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349210"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a>deviceAndAppManagementRoleAssignment-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.

Erbt von [roleAssignment](../resources/intune-rbac-roleassignment.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceAndAppManagementRoleAssignments auflisten](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|[DeviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekte.|
|[DeviceAndAppManagementRoleAssignment abrufen](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Lesen von Eigenschaften und Beziehungen des [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.|
|[DeviceAndAppManagementRoleAssignment erstellen](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Erstellen eines neuen [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.|
|[DeviceAndAppManagementRoleAssignment löschen](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|Keine|Löscht ein [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekt.|
|[DeviceAndAppManagementRoleAssignment aktualisieren](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Dies ist schreibgeschützt und wird automatisch generiert. Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)|
|displayName|String|Der Anzeigename der Rollenzuweisung. Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)|
|description|String|Beschreibung der Rollenzuweisung. Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)|
|scopeMembers|String collection|Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.  Dies sind IDs aus Azure Active Directory. Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)|
|scopeType|[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)|Gibt den Typ des Bereichs für eine Rollenzuweisung. Standardtyp 'ResourceScope' ermöglicht die Zuweisung von ResourceScopes. Für 'AllDevices', 'AllLicensedUsers' und 'AllDevicesAndLicensedUsers' sollte die ResourceScopes-Eigenschaft leer bleiben. Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md). Mögliche Werte: sind `resourceScope`, `allDevices`, `allLicensedUsers` und `allDevicesAndLicensedUsers`.|
|resourceScopes|String collection|Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.  Dies sind IDs aus Azure Active Directory. Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)|
|Elemente|String collection|Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen. Dies sind IDs aus Azure Active Directory.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Die Rollendefinition, in der diese Zuweisung enthalten ist. Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)|
|roleScopeTags|[RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Auflistung|Der Satz von Rolle Bereich Tags für die Rollenzuweisung definiert.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```





