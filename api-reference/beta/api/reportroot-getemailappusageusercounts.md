---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Rufen Sie die Anzahl der eindeutigen Benutzer ab, die über eine E-Mail-App mit Exchange Online verbunden sind.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d7812f0209b07af877cf44c2bff10d9ddfc48ef6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956131"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="24905-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="24905-103">reportRoot: getEmailAppUsageUserCounts</span></span>

> <span data-ttu-id="24905-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="24905-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24905-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24905-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24905-106">Rufen Sie die Anzahl der eindeutigen Benutzer ab, die über eine E-Mail-App mit Exchange Online verbunden sind.</span><span class="sxs-lookup"><span data-stu-id="24905-106">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="24905-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Nutzung von E-Mail-Apps](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="24905-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="24905-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="24905-108">Permissions</span></span>

<span data-ttu-id="24905-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24905-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24905-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24905-111">Permission type</span></span>                        | <span data-ttu-id="24905-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24905-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="24905-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24905-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="24905-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="24905-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="24905-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24905-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24905-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24905-116">Not supported.</span></span>                           |
| <span data-ttu-id="24905-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24905-117">Application</span></span>                            | <span data-ttu-id="24905-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="24905-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="24905-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24905-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="24905-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="24905-120">Function parameters</span></span>

<span data-ttu-id="24905-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="24905-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="24905-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="24905-122">Parameter</span></span> | <span data-ttu-id="24905-123">Typ</span><span class="sxs-lookup"><span data-stu-id="24905-123">Type</span></span>   | <span data-ttu-id="24905-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24905-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="24905-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="24905-125">period</span></span>    | <span data-ttu-id="24905-126">string</span><span class="sxs-lookup"><span data-stu-id="24905-126">string</span></span> | <span data-ttu-id="24905-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="24905-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="24905-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="24905-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="24905-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="24905-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="24905-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="24905-130">Required.</span></span> |

<span data-ttu-id="24905-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24905-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="24905-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="24905-132">The default output type is text/csv.</span></span> <span data-ttu-id="24905-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="24905-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24905-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24905-134">Request headers</span></span>

| <span data-ttu-id="24905-135">Name</span><span class="sxs-lookup"><span data-stu-id="24905-135">Name</span></span>          | <span data-ttu-id="24905-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24905-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="24905-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="24905-137">Authorization</span></span> | <span data-ttu-id="24905-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24905-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="24905-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="24905-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="24905-141">CSV</span><span class="sxs-lookup"><span data-stu-id="24905-141">CSV</span></span>

<span data-ttu-id="24905-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="24905-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="24905-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24905-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="24905-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="24905-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="24905-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="24905-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="24905-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="24905-146">Report Refresh Date</span></span>
- <span data-ttu-id="24905-147">E-Mail für Mac</span><span class="sxs-lookup"><span data-stu-id="24905-147">Mail For Mac</span></span>
- <span data-ttu-id="24905-148">Outlook für Mac</span><span class="sxs-lookup"><span data-stu-id="24905-148">Outlook For Mac</span></span>
- <span data-ttu-id="24905-149">Outlook für Windows</span><span class="sxs-lookup"><span data-stu-id="24905-149">Outlook For Windows</span></span>
- <span data-ttu-id="24905-150">Outlook für mobile Geräte</span><span class="sxs-lookup"><span data-stu-id="24905-150">Outlook For Mobile</span></span>
- <span data-ttu-id="24905-151">Weiteres für mobile Geräte</span><span class="sxs-lookup"><span data-stu-id="24905-151">Other For Mobile</span></span>
- <span data-ttu-id="24905-152">Outlook für Web</span><span class="sxs-lookup"><span data-stu-id="24905-152">Outlook For Web</span></span>
- <span data-ttu-id="24905-153">POP3-App</span><span class="sxs-lookup"><span data-stu-id="24905-153">POP3 App</span></span>
- <span data-ttu-id="24905-154">IMAP4-App</span><span class="sxs-lookup"><span data-stu-id="24905-154">IMAP4 App</span></span>
- <span data-ttu-id="24905-155">SMTP-App</span><span class="sxs-lookup"><span data-stu-id="24905-155">SMTP App</span></span>
- <span data-ttu-id="24905-156">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="24905-156">Report Date</span></span>
- <span data-ttu-id="24905-157">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="24905-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="24905-158">JSON</span><span class="sxs-lookup"><span data-stu-id="24905-158">JSON</span></span>

<span data-ttu-id="24905-159">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[EmailAppUsageUserCounts](../resources/emailappusageusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="24905-159">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24905-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24905-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="24905-161">CSV</span><span class="sxs-lookup"><span data-stu-id="24905-161">CSV</span></span>

<span data-ttu-id="24905-162">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="24905-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="24905-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24905-163">Request</span></span>

<span data-ttu-id="24905-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="24905-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="24905-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="24905-165">Response</span></span>

<span data-ttu-id="24905-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24905-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="24905-167">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="24905-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="24905-168">JSON</span><span class="sxs-lookup"><span data-stu-id="24905-168">JSON</span></span>

<span data-ttu-id="24905-169">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24905-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="24905-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24905-170">Request</span></span>

<span data-ttu-id="24905-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="24905-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="24905-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="24905-172">Response</span></span>

<span data-ttu-id="24905-173">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24905-173">The following is an example of the response.</span></span>

> <span data-ttu-id="24905-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="24905-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 0, 
      "outlookForMac": 0, 
      "outlookForWindows": 0, 
      "outlookForMobile": 0, 
      "otherForMobile": 0, 
      "outlookForWeb": 0, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
