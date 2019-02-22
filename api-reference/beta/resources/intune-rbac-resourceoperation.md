---
title: Ressourcentyp „resourceOperation“
description: Beschreibt die resourceoperation-Ressource (Entity) der Microsoft Graph-API für InTune (REST), die rollenbasierte Zugriffs Steuerungs Szenarien für mandantenorganisationen unterstützt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a299247815993a6ac1e99fe11ecead7ab66e2f2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165002"
---
# <a name="resourceoperation-resource-type"></a>Ressourcentyp „resourceOperation“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Dieser Ressourcentyp definiert eine Operation oder eine Aktion, die auf eine Intune-Ressource oder Intune-Entität angewendet werden kann.  Gängige Operationen sind „Lesen“, „Löschen“, „Aktualisieren“ und „Erstellen“.  Diese Operationen ermöglichen eine grundlegende Verwaltung der zugrunde liegenden Intune-Ressource selbst.  In einigen Fällen sind für eine Intune-Ressource Operationen möglich, über die die Ressource Aktionen in Kombination mit anderen Ressourcen ausführen kann.  Beispiel: Die Operation „Zuweisen“ wird verwendet, um eine Ressource des Typs „mobileApp“ einer AAD-Sicherheitsgruppe zuzuweisen.  Ressourcenoperationen für integrierte Rollen können nicht geändert werden. Dieser Ressourcentyp definiert eine Operation oder eine Aktion, die auf eine Intune-Ressource oder Intune-Entität angewendet werden kann.  Gängige Operationen sind „Abrufen“, „Auflisten“, „Löschen“, „Aktualisieren“ und „Erstellen“.  Diese Operationen ermöglichen eine grundlegende Verwaltung der zugrunde liegenden Intune-Ressource selbst.  In einigen Fällen sind für eine Intune-Ressource Operationen möglich, über die die Ressource Aktionen in Kombination mit anderen Ressourcen ausführen kann.  Beispiel: Die Operation „Zuweisen“ wird verwendet, um eine Ressource des Typs „mobileApp“ einer AAD-Sicherheitsgruppe zuzuweisen.  Ressourcenoperationen für integrierte Rollen können nicht geändert werden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „resourceOperation“](../api/intune-rbac-resourceoperation-list.md)|Sammlung von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md) auf.|
|[Abrufen von „resourceOperation“](../api/intune-rbac-resourceoperation-get.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Erstellen von „resourceOperation“](../api/intune-rbac-resourceoperation-create.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Erstellt neue Objekte des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Löschen von „resourceOperation“](../api/intune-rbac-resourceoperation-delete.md)|Keiner|Löscht Objekte des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Aktualisieren von „resourceOperation“](../api/intune-rbac-resourceoperation-update.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Aktualisiert die Eigenschaften von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[getScopesForUser-Funktion](../api/intune-rbac-resourceoperation-getscopesforuser.md)|Zeichenfolgenauflistung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Ressourcenoperation. Er ist schreibgeschützt und wird automatisch generiert.|
|resource|Zeichenfolge|Ressourcenkategorie, zu der dieser Vorgang gehört.|
|resourceName|Zeichenfolge|Name der Ressource, auf die die Operation angewendet wird|
|actionName|Zeichenfolge|Typ von Aktion, den die Operation ausführen wird. Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.|
|description|Zeichenfolge|Beschreibung der Ressourcenoperation. Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.|
|enabledForScopeValidation|Boolescher Wert|Bestimmt, ob die Berechtigung für Bereiche validiert wird, die pro Rollenzuweisung definiert sind.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resource": "String",
  "resourceName": "String",
  "actionName": "String",
  "description": "String",
  "enabledForScopeValidation": true
}
```




