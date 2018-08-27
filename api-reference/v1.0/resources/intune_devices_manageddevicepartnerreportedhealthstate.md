# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>ManagedDevicePartnerReportedHealthState Enumerationstyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Verfügbare Integritätszustände für das Gerät Health-API
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Der Integritätszustand des Geräts wurde noch nicht gemeldet|
|activated|1|Das Gerät wurde von einem Mobile-Threat-Defense-Partner aktiviert, hat seine Integrität aber noch nicht gemeldet.|
|deactivated|2|Das Gerät wurde von einem Mobile-Threat-Defense-Partner deaktiviert. Der Integritätszustand des Geräts ist nicht bekannt.|
|secured|3|Das Gerät wird vom Mobile-Threat-Defense-Partner als gesichert angesehen.|
|lowSeverity|4|Das Gerät wird vom Mobile-Threat-Defense-Partner als geringe Bedrohung angesehen.|
|mediumSeverity|5|Das Gerät wird vom Mobile-Threat-Defense-Partner als mittlere Bedrohung angesehen.|
|highSeverity|6|Das Gerät wird vom Mobile-Threat-Defense-Partner als große Bedrohung angesehen.|
|unresponsive|7|Das Gerät reagiert laut dem Mobile-Threat-Defense-Partner nicht. Der Integritätszustand des Geräts ist nicht bekannt.|



