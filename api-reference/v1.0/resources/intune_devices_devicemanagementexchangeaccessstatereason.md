# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>DeviceManagementExchangeAccessStateReason Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Grund des Gerätezustandes des Exchange-Zugriffs.
## <a name="members"></a>Mitglieder
|Mitglied|Wert|Beschreibung|
|:---|:---|:---|
|Keine|0|Kein Zugriffszustandsgrund von Exchange gefunden|
|unbekannt|1|Unbekannter Grund des Zugriffszustandes|
|exchangeGlobalRule|2|Zugriffszustand durch Exchange globale Regel bestimmt|
|exchangeIndividualRule|3|Zugriffszustand durch Exchange einzelne Regel bestimmt|
|exchangeDeviceRule|4|Zugriffszustand, der von der Exchange-Geräteregel bestimmt wird|
|exchangeUpgrade|5|Zugriffszustand aufgrund von Exchange-upgrade|
|exchangeMailboxPolicy|6|Zugriffszustand von Exchange-Postfachrichtlinie bestimmt|
|sonstige|7|Zugriffszustand durch Exchange bestimmt|
|konform|8|Zugriffszustand, der von der Compliance-Herausforderung gewährt wird|
|notCompliant|9|Der Zugriffszustand wurde durch die Compliance-Herausforderung widerrufen|
|notEnrolled|10|Zugriffszustand wurde durch die Verwaltungsherausforderung widerrufen|
|unknownLocation|12|Zugriffszustand aufgrund von unbekanntem Speicherort|
|mfaRequired|13|Zugriffszustand aufgrund der MFA-Herausforderung|
|azureADBlockDueToAccessPolicy|14|Zugriffszustand durch AAD-Zugriffsrichtlinie widerrufen|
|compromisedPassword|15|Zugriffszustand wurde durch kompromittierendes Kennwort widerrufen|
|deviceNotKnownWithManagedApp|16|Zugriffszustand wurde durch die Herausforderung für verwaltete Anwendungen widerrufen|



