# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelTyp Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für die Cloud-Block-Ebene
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|Nicht konfiguriert|0|Standardwert: Verwendet die standardmäßige Windows Defender Antivirus-Blockierungsstufe und bietet eine starke Erkennung, ohne das Risiko zu erhöhen, legitime Dateien zu erkennen|
|high|1|Der Wert "high" wendet eine starke Erkennungsstufe an.|
|highPlus|2|High + verwendet das High-Level und wendet zusätzliche Schutzmaßnahmen an|
|zeroTolerance|3|ZeroTolerance blockiert alle unbekannten, ausführbaren Dateien|








