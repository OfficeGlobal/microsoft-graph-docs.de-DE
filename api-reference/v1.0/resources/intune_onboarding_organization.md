# <a name="organization-resource-type"></a>organization-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Organisationen auflisten](../api/intune_onboarding_organization_list.md)|[organization](../resources/intune_onboarding_organization.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [organization](../resources/intune_onboarding_organization.md)-Objekte.|
|[Organisation abrufen](../api/intune_onboarding_organization_get.md)|[Organisation](../resources/intune_onboarding_organization.md)|Dient zum Lesen der Eigenschaften und Beziehungen des [organization](../resources/intune_onboarding_organization.md)-Objekts.|
|[Organisation aktualisieren](../api/intune_onboarding_organization_update.md)|[Organisation](../resources/intune_onboarding_organization.md)|Aktualisieren der Eigenschaften eines [organization](../resources/intune_onboarding_organization.md)-Objekts.|
|[setMobileDeviceManagementAuthority-Aktion](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|Int32|Autorität für die Verwaltung mobiler Geräte festlegen|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Die GUID für das Objekt.|
|mobileDeviceManagementAuthority|[mdmAuthority](../resources/intune_onboarding_mdmauthority.md)|Managementautorität für mobile Geräte. Mögliche Werte sind: `unknown`, `intune`, `sccm`, `office365`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->






