# <a name="reportroot-getoffice365activationcounts"></a>reportRoot: getOffice365ActivationCounts

Erfahren Sie, wie viele Office 365-Aktivierungen auf Desktops und Geräten durchgeführt wurden.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
| :------------------------------------- | :--------------------------------------- |
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Reports.Read.All                         |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt                           |
| Anwendung                            | Reports.Read.All                         |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a>Anforderungsheader

| Name          | Beschreibung                              |
| :------------ | :--------------------------------------- |
| Authorization | Bearer {token}. Erforderlich.                |
| If-None-Match | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben. Optional. |

## <a name="response"></a>Antwort

Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet. Die URL finden Sie in der `Location`-Kopfzeile der Antwort.

Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.

Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.

- Berichtsaktualisierungsdatum
- Produkttyp
- Windows
- Mac
- Android
- iOS
- Windows 10 Mobile

## <a name="example"></a>Beispiel

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```

#### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```
