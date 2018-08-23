# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason Enumerationstyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Top-Level-Fehlerkategorien für die Registrierung.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unbekannt|0|Standardwert, Fehlerursache ist unbekannt.|
|Authentifizierung|1|Authentifizierung fehlgeschlagen|
|Autorisierung|2|Der Aufruf wurde authentifiziert, jedoch nicht für eine Registrierung autorisiert.|
|accountValidation|3|Validierung des Kontos für die Registrierung ist fehlgeschlagen. (Konto wurde blockiert, Registrierung wurde nicht ermöglicht)|
|userValidation|4|Benutzer konnte nicht validiert werden. (Benutzer existiert nicht, Lizenz fehlt)|
|deviceNotSupported|5|Gerät unterstützt die Verwaltung von Mobilgeräten nicht.|
|inMaintenance|6|Konto befindet sich gerade in Wartung.|
|badRequest|7|Der Client hat eine Anfrage gesendet, die vom Dienst nicht verstanden/unterstützt wird.|
|featureNotSupported|8|Die von dieser Registrierung genutzte(n) Funktion(en) werden für dieses Konto nicht unterstützt.|
|enrollmentRestrictionsEnforced|9|Vom Administrator konfigurierte Registrierungseinschränkungen haben diese Registrierung blockiert.|
|clientDisconnected|10|Client ist abgelaufen oder die Registrierung wurde vom Endbenutzer abgebrochen.|



