---
title: 'reportRoot: getOffice365GroupsActivityFileCounts'
description: Rufen Sie die Gesamtzahl der Dateien ab und erfahren Sie, wie viele der Dateien in allen Office 365-Gruppen zugeordneten Gruppenwebsites aktiv waren.
ms.openlocfilehash: 33050098ef970894ec08a1c264848b2bd92128c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016748"
---
# <a name="reportroot-getoffice365groupsactivityfilecounts"></a>reportRoot: getOffice365GroupsActivityFileCounts

Rufen Sie die Gesamtzahl der Dateien ab und erfahren Sie, wie viele der Dateien in allen Office 365-Gruppen zugeordneten Gruppenwebsites aktiv waren.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

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
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a>Funktionsparameter

Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.

| Parameter | Typ   | Beschreibung                              |
| :-------- | :----- | :--------------------------------------- |
| Zeitraum    | string | Gibt die Zeitspanne an, für die der Bericht aggregiert wird. Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180. Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird. Erforderlich.  |

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
- Gesamt
- Aktiv
- Berichtsdatum
- Berichtszeitraum

## <a name="example"></a>Beispiel

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityFileCounts(period='D7')
```

#### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```