---
title: roleAssignment-Ressourcentyp
description: Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32527fad8db54f865f054f04400897e51638e5c2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258429"
---
# <a name="roleassignment-resource-type"></a>roleAssignment-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Rollenzuweisungsressource. Rollenzuweisungen verknüpfen eine Rollendefinition mit Membern und Bereichen. Es kann eine oder mehrere Rollenzuweisungen pro Rolle geben. Dies gilt für benutzerdefinierte und integrierte Rollen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[RoleAssignments auflisten](../api/intune-rbac-roleassignment-list.md)|Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)|Auflisten von Eigenschaften und Beziehungen der [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekte.|
|[RoleAssignment abrufen](../api/intune-rbac-roleassignment-get.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|Lesen von Eigenschaften und Beziehungen des [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.|
|[RoleAssignment erstellen](../api/intune-rbac-roleassignment-create.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|Erstellen eines neuen [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.|
|[RoleAssignment löschen](../api/intune-rbac-roleassignment-delete.md)|Keine|Löscht ein [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekt.|
|[RoleAssignment aktualisieren](../api/intune-rbac-roleassignment-update.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Er ist schreibgeschützt und wird automatisch generiert.|
|displayName|Zeichenfolge|Der Anzeigename der Rollenzuweisung.|
|description|String|Beschreibung der Rollenzuweisung.|
|resourceScopes|String collection|Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.  Dies sind IDs aus Azure Active Directory.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Die Rollendefinition, in der diese Zuweisung enthalten ist.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```



