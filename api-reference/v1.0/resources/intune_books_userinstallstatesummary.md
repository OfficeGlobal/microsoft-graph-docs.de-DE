# <a name="userinstallstatesummary-resource-type"></a>userInstallStateSummary-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für die Zusammenfassung des Installationsstatus für einen Benutzer.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[userInstallStateSummaries auflisten](../api/intune_books_userinstallstatesummary_list.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)-Objekte.|
|[userInstallStateSummary abrufen](../api/intune_books_userinstallstatesummary_get.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Lesen von Eigenschaften und Beziehungen des [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)-Objekts.|
|[userInstallStateSummary erstellen](../api/intune_books_userinstallstatesummary_create.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Erstellen eines neuen [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)-Objekts.|
|[userInstallStateSummary löschen](../api/intune_books_userinstallstatesummary_delete.md)|Keine|Löscht ein [UserInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)-Objekt.|
|[userInstallStateSummary aktualisieren](../api/intune_books_userinstallstatesummary_update.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Aktualisieren der Eigenschaften eines [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Entität|
|userName|String|Name des Benutzers|
|installedDeviceCount|Int32|Anzahl der installierten Geräte|
|failedDeviceCount|Int32|Anzahl der fehlgeschlagenen Geräte|
|notInstalledDeviceCount|Int32|Anzahl der nicht installierten Geräte|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceStates|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)-Sammlung|Der Installationsstatus des E-Books.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```








