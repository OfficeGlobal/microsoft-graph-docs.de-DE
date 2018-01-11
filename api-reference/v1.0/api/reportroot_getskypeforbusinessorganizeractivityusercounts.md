# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a>reportRoot: getSkypeForBusinessOrganizerActivityUserCounts

Erhalten Sie Informationen über die Anzahl der eindeutigen Benutzer und die Art der von Benutzern in Ihrer Organisation gehaltenen und organisierten Konferenzsitzungen. Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web, Einwahl/Auswahl Drittanbieter und Einwahl/Auswahl Microsoft.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Konferenzorganisationsaktivität](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
| :------------------------------------- | :--------------------------------------- |
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Nicht unterstützt                           |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt                           |
| Anwendung                            | Reports.Read.All                         |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a>Anforderungsparameter

Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit einem gültigen Wert bereit.

| Parameter | Typ   | Beschreibung                              |
| :-------- | :----- | :--------------------------------------- |
| Zeitraum    | Zeichenfolge | Gibt die Zeitspanne an, für die der Bericht aggregiert wird. Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180. Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird. Erforderlich. |

## <a name="request-headers"></a>Anforderungsheader

| Name          | Beschreibung               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Erforderlich. |
| If-None-Match | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben. Optional. |

## <a name="response"></a>Antwort

Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet. Die URL finden Sie in der `Location`-Kopfzeile der Antwort.

Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.

Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.

- Berichtsaktualisierungsdatum
- Berichtsdatum
- Berichtszeitraum
- Chat
- Audio/Video
- Gemeinsame Nutzung von Anwendungen
- Web
- Einwahl/Auswahl Drittanbieter
- Einwahl/Auswahl Microsoft

## <a name="example"></a>Beispiel

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')
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

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```
