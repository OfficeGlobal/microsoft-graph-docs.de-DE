# <a name="create-domain"></a>Domäne erstellen

Fügt eine Domäne zum Mandanten hinzu.

**Wichtig**: Sie können eine zugeordnete Domäne erst dann mit Ihrem Azure AD-Mandanten verwenden, nachdem der Besitz überprüft wurde. Weitere Informationen finden Sie unter [verificationDnsRecords auflisten](domain_list_verificationdnsrecords.md). Stammdomänen erfordern eine Überprüfung. Beispielsweise muss „contoso.com“ überprüft werden. Wenn eine Stammdomäne überprüft wird, werden Unterdomänen der Stammdomäne automatisch überprüft. Beispielsweise wird „subdomain.contoso.com“ automatisch überprüft, wenn „contoso.com“ überprüft wurde.

### <a name="prerequisites"></a>Voraussetzungen

Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Domain.ReadWrite.All* oder *Directory.AccessAsUser.All*

### <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
### <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich.|
| Content-Type  | application/json |

### <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des [domain](../resources/domain.md)-Objekts an.

> Der Anforderungstext enthält die id-Eigenschaft für die neue Domäne. Die id-Eigenschaft ist die einzige Eigenschaft, die angegeben werden kann, und sie ist erforderlich. Der Wert der id-Eigenschaft ist der vollqualifizierte Domänenname, der erstellt werden soll.

### <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.

### <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung

Geben Sie im Anforderungstext eine JSON-Darstellung des [domain](../resources/domain.md)-Objekts an.

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/V1.0/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a>Antwort
Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->