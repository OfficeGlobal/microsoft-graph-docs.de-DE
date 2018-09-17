# <a name="usersecuritystate-resource-type"></a>Ressourcentyp userSecurityState

Enthält Zustandsinformationen über das Benutzerkonto.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|aadUserId|Zeichenfolge|AAD-Benutzer-Objektbezeichner (GUID) -stellt die physische/multi-Konto-Benutzerentität dar.|
|accountName|Zeichenfolge|Kontoname des Benutzerkontos (ohne Active Directory-Domäne oder DNS-Domäne) - (auch bezeichnet als `mailNickName`).|
|Domänname|Zeichenfolge|NetBIOS/Active Directory-Domäne des Benutzerkontos (d.h., im Format Domäne\Konto).|
|emailRole|emailRole|Für E-Mail-bezogene Warnungen - die E-Mail-'Rolle' des Benutzerkontos. Mögliche Werte sind: `unknown`, `sender` und `recipient`.|
|isVpn|Boolesch|Gibt an, ob der Benutzer über ein VPN angemeldet ist.|
|logonDateTime|DateTimeOffset|Zeitpunkt, an dem die Anmeldung stattgefunden hat. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|logonId|Zeichenfolge|Benutzer-Anmelde-ID.|
|logonIp|Zeichenfolge|Die IP-Adresse, von der die Anmelde-Anforderung stammt.|
|logonLocation|Zeichenfolge|Der Speicherort (nach Zuordnung der IP-Adresse), mit dem das Benutzer-Anmelde-Ereignis zugeordnet ist.|
|logonType|logonType|Anmeldemethode des Benutzers. Mögliche Werte sind: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch` und `service`.|
|onPremisesSecurityIdentifier|Zeichenfolge|Active Directory (lokal) Sicherheitsbezeichner (SID) des Benutzers.|
|riskScore|Zeichenfolge|Vom Anbieter generierte/berechnete Risikobewertung des Benutzerkontos. Empfohlener Wertebereich von 0-1, was einem Prozentsatz entspricht.|
|userAccountType|userAccountSecurityType|Typ des Benutzerkontos (Gruppenmitgliedschaft) nach Windows-Definition. Mögliche Werte: `unknown`, `standard`, `power`, `administrator`.|
|userPrincipalName|Zeichenfolge|Benutzer-Anmeldename - Internetformat: (Benutzerkontoname) @(Benutzerkonto-DNS-Domänenname).|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
