---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Rufen Sie Details zu aktiven Office 365-Benutzern ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: ff9df2d2eb6c00990ac93e324f47f92fea8003de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934709"
---
# <a name="reportroot-getoffice365activeuserdetail"></a>reportRoot: getOffice365ActiveUserDetail

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Rufen Sie Details zu aktiven Office 365-Benutzern ab.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
| :------------------------------------- | :--------------------------------------- |
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Reports.Read.All                         |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt                           |
| Anwendung                            | Reports.Read.All                         |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a>Funktionsparameter

Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.

| Parameter | Typ   | Beschreibung                              |
| :-------- | :----- | :--------------------------------------- |
| Zeitraum    | string | Gibt die Zeitspanne an, für die der Bericht aggregiert wird. Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180. Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird. |
| date      | Datum   | Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben. {date_value} muss im Format JJJJ-MM-TT vorliegen. Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein. |

> **Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.

Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort. Der Typ der Standardwert ist Text/Csv. Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.

## <a name="request-headers"></a>Anforderungsheader

| Name          | Beschreibung               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Erforderlich. |

## <a name="response"></a>Antwort

### <a name="csv"></a>CSV

Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet. Die URL finden Sie in der `Location`-Kopfzeile der Antwort.

Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.

Die CSV-Datei verfügt über die folgenden Spaltenheader:

- Berichtsaktualisierungsdatum
- Benutzerprinzipalname
- Anzeigename
- Ist gelöscht
- Gelöscht am
- Besitzt Exchange-Lizenz
- Besitzt OneDrive-Lizenz
- Besitzt SharePoint-Lizenz
- Besitzt Skype For Business-Lizenz
- Besitzt Yammer-Lizenz
- Besitzt Teams-Lizenz
- Datum der letzten Exchange-Aktivität
- Datum der letzten OneDrive-Aktivität
- Datum der letzten SharePoint-Aktivität
- Datum der letzten Skype for Business-Aktivität
- Datum der letzten Yammer-Aktivität
- Datum der letzten Teams-Aktivität
- Datum der Exchange-Lizenzzuweisung
- Datum der OneDrive-Lizenzzuweisung
- Datum der SharePoint-Lizenzzuweisung
- Datum der Skype For Business-Lizenzzuweisung
- Datum der Yammer-Lizenzzuweisung
- Datum der Teams-Lizenzzuweisung
- Zugewiesene Produkte

Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:

- Besitzt Yammer-Lizenz
- Besitzt Teams-Lizenz
- Datum der letzten Yammer-Aktivität
- Datum der letzten Teams-Aktivität
- Datum der Yammer-Lizenzzuweisung
- Datum der Teams-Lizenzzuweisung

### <a name="json"></a>JSON

Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** -Objekts in der Antworttext.

Die folgenden Eigenschaften im **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:

- hasYammerLicense
- hasTeamsLicense
- yammerLastActivityDate
- teamsLastActivityDate
- yammerLicenseAssignDate
- teamsLicenseAssignDate

Die Seite Standardgröße für diese Anforderung ist 200 Elemente.

## <a name="example"></a>Beispiel

### <a name="csv"></a>CSV

Es folgt ein Beispiel, das CSV ausgibt.

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
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

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```

### <a name="json"></a>JSON

Es folgt ein Beispiel, das JSON zurückgegeben.

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

> **Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 853

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "hasExchangeLicense": true, 
      "hasOneDriveLicense": false, 
      "hasSharePointLicense": false, 
      "hasSkypeForBusinessLicense": false, 
      "hasYammerLicense": false, 
      "hasTeamsLicense": false, 
      "exchangeLastActivityDate": "2017-08-30", 
      "oneDriveLastActivityDate": null, 
      "sharePointLastActivityDate": null, 
      "skypeForBusinessLastActivityDate": null, 
      "yammerLastActivityDate": null, 
      "teamsLastActivityDate": null, 
      "exchangeLicenseAssignDate": "2016-05-03", 
      "oneDriveLicenseAssignDate": null, 
      "sharePointLicenseAssignDate": null, 
      "skypeForBusinessLicenseAssignDate": null, 
      "yammerLicenseAssignDate": null, 
      "teamsLicenseAssignDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ]
    }
  ]
}
```
