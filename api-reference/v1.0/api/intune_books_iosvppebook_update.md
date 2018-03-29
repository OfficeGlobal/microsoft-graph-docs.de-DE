# <a name="update-iosvppebook"></a>Aktualisieren von „iosVppEBook“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md).
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementApps.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md) an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md) erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|displayName|String|Name des E-Books. Geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|description|String|Beschreibung. Geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|publisher|String|Herausgeber. Geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|publishedDateTime|DateTimeOffset|Datum und Uhrzeit der Veröffentlichung des E-Books. Geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|largeCover|[mimeContent](../resources/intune_books_mimecontent.md)|Umschlagbild des Buchs. Geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der E-Book-Datei. Geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des E-Books. Geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|informationUrl|String|URL zur Seite mit weiteren Informationen. Geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|privacyInformationUrl|String|URL zur Datenschutzerklärung. Geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|vppTokenId|Guid|ID des VPP-Tokens|
|appleId|String|Apple-ID, die dem VPP-Token zugeordnet ist|
|vppOrganizationName|String|Zum VPP-Token gehörender Organisationsname|
|genres|Collection von Objekten des Typs „String“|Genres|
|language|String|Sprache|
|seller|String|Verkäufer|
|totalLicenseCount|Int32|Gesamtanzahl von Lizenzen|
|usedLicenseCount|Int32|Gesamtanzahl von genutzten Lizenzen|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md) im Antworttext zurück.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 803

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 961

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```


