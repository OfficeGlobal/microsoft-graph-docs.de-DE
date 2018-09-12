# <a name="managementagenttype-enum-type"></a>managementAgentType Enumerationstyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Management-Agent-Typ.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|eas|1|Das Gerät wird vom Exchange Server verwaltet.|
|mdm|2|Das Gerät wird von Intune MDM verwaltet.|
|easMdm|3|Das Gerät wird sowohl von Exchange Server als auch Intune MDM verwaltet.|
|intuneClient|4|Intune Client verwaltet.|
|easIntuneClient|5|Das Gerät wird sowohl von EAS als auch von Intune-Client verwaltet.|
|configurationManagerClient|8|Das Gerät wird vom Konfigurations-Manager verwaltet.|
|configurationManagerClientMdm|10|Das Gerät wird vom Konfigurations-Manager und von MDM verwaltet.|
|configurationManagerClientMdmEas|11|Das Gerät wird vom Konfigurations-Manager, MDM und von Eas verwaltet.|
|unknown|16|Unbekannter Management-Agent-Typ.|
|jamf|32|Das Gerätattribute werden aus Jamf abgerufen.|
|googleCloudDevicePolicyController|64|Das Gerät wird von Google CloudDPC verwaltet.|








