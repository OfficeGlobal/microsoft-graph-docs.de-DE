---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Rufen Sie die Anzahl der eindeutigen Benutzer ab, die über eine E-Mail-App mit Exchange Online verbunden sind.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 242a7256bab59fa8fa010a1e1966e262c81797c2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574243"
---
# <a name="reportroot-getemailappusageusercounts"></a>reportRoot: getEmailAppUsageUserCounts

Rufen Sie die Anzahl der eindeutigen Benutzer ab, die über eine E-Mail-App mit Exchange Online verbunden sind.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Nutzung von E-Mail-Apps](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).

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
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
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
- E-Mail für Mac
- Outlook für Mac
- Outlook für Windows
- Outlook für mobile Geräte
- Weiteres für mobile Geräte
- Outlook für Web
- POP3-App
- IMAP4-App
- SMTP-App
- Berichtsdatum
- Berichtszeitraum

## <a name="example"></a>Beispiel

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserCounts(period='D7')
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

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```
