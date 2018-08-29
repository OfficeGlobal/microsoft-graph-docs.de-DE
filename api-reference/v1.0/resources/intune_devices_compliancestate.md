# <a name="compliancestate-enum-type"></a>complianceState Enumerationstyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Compliance-Status.
## <a name="members"></a>Mitglieder
|Mitglied|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Unbekannt.|
|compliant|1|Kompatibel.|
|noncompliant|2|Das Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.|
|conflict|3|Konflikt mit anderen Regeln.|
|error|4|Fehler.|
|inGracePeriod|254
|Das Gerät ist nicht kompatibel, hat aber dennoch Zugriff auf Unternehmensressourcen|
|configManager|255|Vom Konfigurations-Manager verwaltet|


