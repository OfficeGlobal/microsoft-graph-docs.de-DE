# <a name="resourceoperation-resource-type"></a>Ressourcentyp „resourceOperation“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Dieser Ressourcentyp definiert eine Operation oder eine Aktion, die auf eine Intune-Ressource oder Intune-Entität angewendet werden kann.  Gängige Operationen sind „Lesen“, „Löschen“, „Aktualisieren“ und „Erstellen“.  Diese Operationen ermöglichen eine grundlegende Verwaltung der zugrunde liegenden Intune-Ressource selbst.  In einigen Fällen sind für eine Intune-Ressource Operationen möglich, über die die Ressource Aktionen in Kombination mit anderen Ressourcen ausführen kann.  Beispiel: Die Operation „Zuweisen“ wird verwendet, um eine Ressource des Typs „mobileApp“ einer AAD-Sicherheitsgruppe zuzuweisen.  Ressourcenoperationen für integrierte Rollen können nicht geändert werden. Dieser Ressourcentyp definiert eine Operation oder eine Aktion, die auf eine Intune-Ressource oder Intune-Entität angewendet werden kann.  Gängige Operationen sind „Abrufen“, „Auflisten“, „Löschen“, „Aktualisieren“ und „Erstellen“.  Diese Operationen ermöglichen eine grundlegende Verwaltung der zugrunde liegenden Intune-Ressource selbst.  In einigen Fällen sind für eine Intune-Ressource Operationen möglich, über die die Ressource Aktionen in Kombination mit anderen Ressourcen ausführen kann.  Beispiel: Die Operation „Zuweisen“ wird verwendet, um eine Ressource des Typs „mobileApp“ einer AAD-Sicherheitsgruppe zuzuweisen.  Ressourcenoperationen für integrierte Rollen können nicht geändert werden.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „resourceOperation“](../api/intune_rbac_resourceoperation_list.md)|Sammlung von Objekten des Typs [resourceOperation](../resources/intune_rbac_resourceoperation.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune_rbac_resourceoperation.md) auf.|
|[Abrufen von „resourceOperation“](../api/intune_rbac_resourceoperation_get.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [resourceOperation](../resources/intune_rbac_resourceoperation.md).|
|[Erstellen von „resourceOperation“](../api/intune_rbac_resourceoperation_create.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|Erstellt neue Objekte des Typs [resourceOperation](../resources/intune_rbac_resourceoperation.md).|
|[Löschen von „resourceOperation“](../api/intune_rbac_resourceoperation_delete.md)|Keiner|Löscht Objekte des Typs [resourceOperation](../resources/intune_rbac_resourceoperation.md).|
|[Aktualisieren von „resourceOperation“](../api/intune_rbac_resourceoperation_update.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|Aktualisiert die Eigenschaften von Objekten des Typs [resourceOperation](../resources/intune_rbac_resourceoperation.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Ressourcenoperation. Er ist schreibgeschützt und wird automatisch generiert.|
|resourceName|String|Name der Ressource, auf die die Operation angewendet wird|
|actionName|String|Typ von Aktion, den die Operation ausführen wird. Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.|
|description|String|Beschreibung der Ressourcenoperation. Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
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
  "resourceName": "String",
  "actionName": "String",
  "description": "String"
}
```



