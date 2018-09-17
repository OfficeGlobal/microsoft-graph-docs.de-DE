# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType Enumerationstyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Optionen, um ein Mobilgerät zur Verwaltung hinzuzufügen.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unbekannt|0|Standardwert, der Registrierungstyp wurde nicht aufgezeichnet.|
|userEnrollment|1|Vom Benutzer initiierte Registrierung über den BYOD-Kanal.|
|deviceEnrollmentManager|2|Benutzerregistrierung mit einem Geräteregistrierungs-Verwaltungskonto.|
|appleBulkWithUser|3|Apple-Stapelregistrierung mit Benutzerherausforderung (DEP, Apple Configurator).|
|appleBulkWithoutUser|4|Apple-Stapelregistrierung ohne Benutzerherausforderung (DEP, Apple Configurator, Mobile Konfiguration).|
|windowsAzureADJoin|5|Windows 10 Azure AD-Hinzufügung.|
|windowsBulkUserless|6|Windows 10-Stapelregistrierung über ICD mit Zertifikat.|
|windowsAutoEnrollment|7|Automatische 10 Windows-Registrierung. (Geschäftskonto hinzufügen)|
|windowsBulkAzureDomainJoin|8|Windows 10 Azure AD-Stapelhinzufügung.|
|windowsCoManagement|9|Windows 10 Co-Verwaltung, die durch AutoPilot oder Gruppenrichtlinien ausgelöst wurde.|



