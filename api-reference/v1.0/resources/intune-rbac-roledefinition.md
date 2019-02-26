---
title: Ressourcentyp „roleDefinition“
description: 'Die Rollendefinitionsressource. Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune. In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert. Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen. Integrierte Rollen können nicht geändert werden. Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden. Erstellen Sie benutzerdefinierte Rollen, wenn Sie eine Rolle definieren möchten, in der beliebige der verfügbaren Ressourcen und Rollenberechtigungen kombiniert werden können.'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fca3587ccb26116257b740a91b376259e1e9dd5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262363"
---
# <a name="roledefinition-resource-type"></a>Ressourcentyp „roleDefinition“

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Rollendefinitionsressource. Die Rollendefinition bildet die Grundlage für rollenbasierten Zugriff in Intune. In der Rolle wird eine Intune-Ressource wie z. B. eine mobile App mit den zugehörigen Rollenberechtigungen, wie „Erstellen“ oder „Lesen“, für die Ressource kombiniert. Es gibt zwei Arten von Rollen: integrierte und benutzerdefinierte Rollen. Integrierte Rollen können nicht geändert werden. Für integrierte wie für benutzerdefinierte Rollen müssen Zuweisungen erzwungen werden. Erstellen Sie eine benutzerdefinierte Rolle, wenn Sie eine Rolle definieren möchten, die beliebige der verfügbaren Ressourcen und Rollenberechtigungen in einer einzigen Rolle zusammenfasst.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „roleDefinition“](../api/intune-rbac-roledefinition-list.md)|Sammlung von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) auf.|
|[Abrufen von „roleDefinition“](../api/intune-rbac-roledefinition-get.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Erstellen von „roleDefinition“](../api/intune-rbac-roledefinition-create.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Erstellt neue Objekte des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Löschen von „roleDefinition“](../api/intune-rbac-roledefinition-delete.md)|Keiner|Löscht Objekte des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Aktualisieren von „roleDefinition“](../api/intune-rbac-roledefinition-update.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Aktualisiert die Eigenschaften von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Er ist schreibgeschützt und wird automatisch generiert.|
|displayName|Zeichenfolge|Anzeigename der Rollendefinition|
|description|Zeichenfolge|Beschreibung der Rollendefinition|
|rolePermissions|Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)|Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden. Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.|
|isBuiltIn|Boolean|Rollentyp. Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|roleAssignments|Sammlung von Objekten des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md)|Liste der Rollenzuweisungen für die Rollendefinition|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



