---
title: Ressourcentyp „resourceOperation“
description: " Vorgang wird verwendet, um eine Sicherheitsgruppe AAD eine MobileApp Ressource zuordnen.  Ressourcenoperationen für integrierte Rollen können nicht geändert werden."
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fd8a0620c56299446d8c0315ca66b318c7e6d71c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914787"
---
# <a name="resourceoperation-resource-type"></a>Ressourcentyp „resourceOperation“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Dieser Ressourcentyp definiert eine Operation oder eine Aktion, die auf eine Intune-Ressource oder Intune-Entität angewendet werden kann.  Gängige Operationen sind „Lesen“, „Löschen“, „Aktualisieren“ und „Erstellen“.  Diese Operationen ermöglichen eine grundlegende Verwaltung der zugrunde liegenden Intune-Ressource selbst.  In einigen Fällen sind für eine Intune-Ressource Operationen möglich, über die die Ressource Aktionen in Kombination mit anderen Ressourcen ausführen kann.  Beispiel: Die Operation „Zuweisen“ wird verwendet, um eine Ressource des Typs „mobileApp“ einer AAD-Sicherheitsgruppe zuzuweisen.  Ressourcenoperationen für integrierte Rollen können nicht geändert werden. Dieser Ressourcentyp definiert eine Operation oder eine Aktion, die auf eine Intune-Ressource oder Intune-Entität angewendet werden kann.  Gängige Operationen sind „Abrufen“, „Auflisten“, „Löschen“, „Aktualisieren“ und „Erstellen“.  Diese Operationen ermöglichen eine grundlegende Verwaltung der zugrunde liegenden Intune-Ressource selbst.  In einigen Fällen sind für eine Intune-Ressource Operationen möglich, über die die Ressource Aktionen in Kombination mit anderen Ressourcen ausführen kann.  Beispiel: Die Operation „Zuweisen“ wird verwendet, um eine Ressource des Typs „mobileApp“ einer AAD-Sicherheitsgruppe zuzuweisen.  Ressourcenoperationen für integrierte Rollen können nicht geändert werden.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „resourceOperation“](../api/intune-rbac-resourceoperation-list.md)|Sammlung von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md) auf.|
|[Abrufen von „resourceOperation“](../api/intune-rbac-resourceoperation-get.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Erstellen von „resourceOperation“](../api/intune-rbac-resourceoperation-create.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Erstellt neue Objekte des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Löschen von „resourceOperation“](../api/intune-rbac-resourceoperation-delete.md)|Keiner|Löscht Objekte des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Aktualisieren von „resourceOperation“](../api/intune-rbac-resourceoperation-update.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Aktualisiert die Eigenschaften von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[GetScopesForUser-Funktion](../api/intune-rbac-resourceoperation-getscopesforuser.md)|Zeichenfolgenauflistung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Ressourcenoperation. Er ist schreibgeschützt und wird automatisch generiert.|
|resource|Zeichenfolge|Resource-Kategorie, zu dem dieser Vorgang gehört.|
|resourceName|Zeichenfolge|Name der Ressource, auf die die Operation angewendet wird|
|actionName|Zeichenfolge|Typ von Aktion, den die Operation ausführen wird. Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.|
|description|Zeichenfolge|Beschreibung der Ressourcenoperation. Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.|
|enabledForScopeValidation|Boolescher Wert|Bestimmt, ob die Berechtigung für pro Rollenzuweisung definierten Bereiche nicht überprüft wird.|

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





