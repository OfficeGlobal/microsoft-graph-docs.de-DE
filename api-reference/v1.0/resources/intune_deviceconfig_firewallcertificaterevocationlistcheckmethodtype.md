# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType Enumerationstyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für firewallCertificateRevocationListCheckMethod
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Von Intune wurde kein Wert konfiguriert, den vom Benutzer konfigurierten Standartwerd für das Gerät nicht außer Kraft setzen|
|keine|1|Zertifikatsperrliste nicht prüfen|
|Versuch|2|CRL-Überprüfung versuchen und Zertifikat nur zulassen, wenn das Zertifikat von der Überprüfung bestätigt wird|
|erfordert|3|Erfolgreiche CRL-Überprüfung anfordern, bevor ein Zertifikat zugelassen wird|








