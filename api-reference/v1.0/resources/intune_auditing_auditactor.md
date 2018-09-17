# <a name="auditactor-resource-type"></a>auditActor-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Typ|Zeichenfolge|Akteurtyp.|
|userPermissions|Zeichenfolgenauflistung|Liste der Benutzerberechtigungen, nachdem die Überwachung ausgeführt wurde.|
|applicationId|Zeichenfolge|AAD-Anwendungs-ID|
|applicationDisplayName|Zeichenfolge|Anwendungsname|
|userPrincipalName|Zeichenfolge|Benutzerprinzipalname (User Principal Name, UPN)|
|servicePrincipalName|Zeichenfolge|Dienstprinzipalnamen (Service Principal Name, SPN)|
|ipAddress|Zeichenfolge|IP-Adresse|
|userId|Zeichenfolge|Benutzer-ID|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```








