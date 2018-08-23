
# <a name="update-user"></a>Benutzer aktualisieren

Mit dieser API können Sie die Eigenschaften eines Benutzerobjekts aktualisieren.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | User.ReadWrite    |
|Anwendung | User.ReadWrite.All, Directory.ReadWrite.All |

Zum Aktualisieren der Eigenschaft „passwordProfile“ ist die folgende Berechtigung erforderlich: Directory.AccessAsUser.All.

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```
## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert|
|:-----------|:------|
| Autorisierung  | Bearer {token}. Erforderlich.  |
| Inhaltstyp  | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|aboutMe|Zeichenfolge|Ein Freihandform-Texteingabefeld, in dem der Benutzer sich selbst beschreiben kann.|
|accountEnabled|Boolesch| **true**, wenn das Konto aktiviert ist; andernfalls **false**. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Unterstützt $filter.    |
|birthday|DateTimeOffset|Der Geburtstag des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|city|Zeichenfolge|Die Stadt, in der sich der Benutzer befindet. Unterstützt $filter.|
|Land|Zeichenfolge|Land/Region, in dem/der sich der Benutzer befindet; z. B. „USA“ oder „UK“. Unterstützt $filter.|
|department|Zeichenfolge|Der Name der Abteilung, in der der Benutzer arbeitet. Unterstützt $filter.|
|displayName|Zeichenfolge|cDer Name, der im Adressbuch für den Benutzer angezeigt wird. Dies ist normalerweise eine Kombination aus dem Vornamen, der Initiale des weiteren Vornamens und des Nachnamens. Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden. Unterstützt $Filter und $orderby.|
|givenName|Zeichenfolge|Der Vorname des Benutzers. Unterstützt $filter.|
|hireDate|DateTimeOffset|Das Einstellungsdatum des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|interests|Zeichenfolgenauflistung|Eine Liste für den Benutzer, um dessen Interessen zu beschreiben.|
|jobTitle|Zeichenfolge|Die Position des Benutzers. Unterstützt $filter.|
|mailNickname|Zeichenfolge|Der E-Mail-Alias für den Benutzer. Diese Eigenschaft muss beim Erstellen eines Benutzers angegeben werden. Unterstützt $filter.|
|mobilePhone|Zeichenfolge|Die Nummer des primären Mobiltelefons für den Benutzer.|
|mySite|Zeichenfolge|Die URL für die persönliche Website des Benutzers.|
|officeLocation|Zeichenfolge|Der Bürostandort der Firma des Benutzers|
|onPremisesImmutableId|Zeichenfolge|Diese Eigenschaft wird verwendet, um ein lokales Active Directory-Benutzerkonto dem Azure AD-Benutzerobjekt zuzuordnen. Diese Eigenschaft muss angegeben werden, wenn ein neues Benutzerkonto in Graph erstellt wird, wenn Sie eine Verbunddomäne für die **UserPrincipalName**-Eigenschaft (UPN) des Benutzers verwenden. **Wichtig:** Die Zeichen **$** und **_** können nicht verwendet werden, wenn Sie diese Eigenschaft angeben. Unterstützt $filter.                            |
|passwordPolicies|Zeichenfolge|Gibt die Kennwortrichtlinien für den Benutzer an. Dieser Wert ist eine Enumeration, deren einziger möglicher Wert „DisableStrongPassword“ lautet. Damit können schwächere Kennwörter als in der Standardrichtlinie angegeben festgelegt werden. Auch „DisablePasswordExpiration“ kann angegeben werden. Beide können zusammen angegeben werden, z. B.: „DisablePasswordExpiration, DisableStrongPassword“.|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md)|Gibt das Kennwortprofil für den Benutzer an. Das Profil enthält das Kennwort des Benutzers. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Das Kennwort im Profil muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft angegeben. Standardmäßig ist ein sicheres Kennwort erforderlich.|
|pastProjects|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der erledigten Projekte eines Benutzers.|
|postalCode|Zeichenfolge|Die Postleitzahl für die Postanschrift des Benutzers. Die Postleitzahl ist für das Land/die Region des Benutzers spezifisch. In den USA enthält dieses Attribut den ZIP Code.|
|preferredLanguage|Zeichenfolge|Die bevorzugte Sprache für den Benutzer. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en-US“.|
|preferredName|Zeichenfolge|Der bevorzugte Name für den Benutzer.|
|responsibilities|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der Verantwortlichkeiten eines Benutzers.|
|schools|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der vom Benutzer besuchten Schulen.|
|skills|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der Qualifikationen eines Benutzers.|
|state|Zeichenfolge|Bundesland oder Kanton in der Adresse des Benutzers. Unterstützt $filter.|
|streetAddress|Zeichenfolge|Die Straße der Firma des Benutzers.|
|surname|Zeichenfolge|Der Nachname des Benutzers. Unterstützt $filter.|
|usageLocation|Zeichenfolge|Ein aus zwei Buchstaben bestehender Ländercode (ISO-Standard 3166). Erforderlich für Benutzer, denen Lizenzen zugewiesen werden, aufgrund der gesetzlichen Vorschrift, dass die Verfügbarkeit von Diensten in einzelnen Ländern geprüft werden muss.  Beispiele sind: „US“, „JP“ und „GB“. Lässt keine NULL-Werte zu. Unterstützt $filter.|
|userPrincipalName|Zeichenfolge|Der User Principal Name (UPN) des Benutzers. Der UPN ist ein Anmeldename des Benutzers im Internetformat, der auf dem Internetstandard RFC 822 basiert. Gemäß der Konvention sollte er dem E-Mail-Namen des Benutzers zugeordnet sein. Das allgemeine Format lautet „alias@domäne“, wobei „domäne“ in der Sammlung der verifizierten Domänen des Mandanten vorhanden sein muss. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Auf die verifizierten Domänen für den Mandanten kann über die **verifiedDomains** -Eigenschaft von [organization](../resources/organization.md) zugegriffen werden. Unterstützt $Filter und $orderby.
|userType|Zeichenfolge|Ein Zeichenfolgenwert kann zum Klassifizieren der Benutzertypen in Ihrem Verzeichnis verwendet werden, z. B. „Member“ und „Guest“. Unterstützt $filter.          |

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
