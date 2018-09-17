# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode Enumerationstyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zulassen, dass das Gerät Diagnose- und Nutzungstelemetriedaten sendet, wie z. B. Watson.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|userDefined|0|Ermöglicht es dem Benutzer, folgendes festzulegen.|
|keine|1|Es werden keine Telemetriedaten von Betriebssystemkomponenten gesendet. Hinweis: Dieser Wert kann nur für Enterprise- und Server-Geräte anwendbar. Wenn Sie diese Einstellung auf anderen Geräten wählen, entspricht dies dem Wert 1.|
|Basis|2|Es werden grundlegende Telemetriedaten gesendet.|
|erweitert|3|Es werden erweiterten Telemetriedaten gesendet, einschließlich Nutzungs- und Analysedaten.|
|voll|4|Es werden sämtliche Telemetriedaten gesendet, einschließlich Diagnosedaten, wie z.B. der Systemstatus.|








