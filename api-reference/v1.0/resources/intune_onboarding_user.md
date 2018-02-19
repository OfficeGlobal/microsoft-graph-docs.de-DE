# <a name="user-resource-type"></a>user-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Benutzer auflisten](../api/intune_onboarding_user_list.md)|[user](../resources/intune_onboarding_user.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune_onboarding_user.md)-Objekte.|
|[Benutzer abrufen](../api/intune_onboarding_user_get.md)|[user](../resources/intune_onboarding_user.md)|Lesen von Eigenschaften und Beziehungen des [user](../resources/intune_onboarding_user.md)-Objekts.|
|[Benutzer erstellen](../api/intune_onboarding_user_create.md)|[user](../resources/intune_onboarding_user.md)|Erstellen eines neuen [user](../resources/intune_onboarding_user.md)-Objekts.|
|[Benutzer löschen](../api/intune_onboarding_user_delete.md)|Keine|Löscht ein [user](../resources/intune_onboarding_user.md)-Objekt.|
|[Benutzer aktualisieren](../api/intune_onboarding_user_update.md)|[user](../resources/intune_onboarding_user.md)|Aktualisieren der Eigenschaften eines [user](../resources/intune_onboarding_user.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner des Benutzers|
|deviceEnrollmentLimit|Int32|Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann. Zulässige Werte sind 5 oder 1000.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 1024
}
```



