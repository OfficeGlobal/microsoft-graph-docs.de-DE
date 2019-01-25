---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Rufen Sie die Gesamtzahl der Postfächer in Ihrem Unternehmen ab und erfahren Sie, wie viele Postfächer im Berichtszeitraum täglich aktiv sind. Ein Postfach wird als aktiv betrachtet, wenn der Benutzer eine E-Mail sendet oder liest.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8d9e99de7a69d62dd7ab24e6cefee9a7c35044f7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528984"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="51574-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="51574-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51574-105">Rufen Sie die Gesamtzahl der Postfächer in Ihrem Unternehmen ab und erfahren Sie, wie viele Postfächer im Berichtszeitraum täglich aktiv sind.</span><span class="sxs-lookup"><span data-stu-id="51574-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="51574-106">Ein Postfach wird als aktiv betrachtet, wenn der Benutzer eine E-Mail sendet oder liest.</span><span class="sxs-lookup"><span data-stu-id="51574-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="51574-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Postfachnutzung](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="51574-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="51574-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="51574-108">Permissions</span></span>

<span data-ttu-id="51574-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51574-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51574-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51574-111">Permission type</span></span>                        | <span data-ttu-id="51574-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51574-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="51574-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51574-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="51574-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="51574-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="51574-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51574-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51574-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51574-116">Not supported.</span></span>                           |
| <span data-ttu-id="51574-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51574-117">Application</span></span>                            | <span data-ttu-id="51574-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="51574-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="51574-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51574-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="51574-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="51574-120">Function parameters</span></span>

<span data-ttu-id="51574-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="51574-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="51574-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="51574-122">Parameter</span></span> | <span data-ttu-id="51574-123">Typ</span><span class="sxs-lookup"><span data-stu-id="51574-123">Type</span></span>   | <span data-ttu-id="51574-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51574-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="51574-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="51574-125">period</span></span>    | <span data-ttu-id="51574-126">string</span><span class="sxs-lookup"><span data-stu-id="51574-126">string</span></span> | <span data-ttu-id="51574-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="51574-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="51574-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="51574-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="51574-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="51574-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="51574-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="51574-130">Required.</span></span> |

<span data-ttu-id="51574-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="51574-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="51574-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="51574-132">The default output type is text/csv.</span></span> <span data-ttu-id="51574-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="51574-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51574-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51574-134">Request headers</span></span>

| <span data-ttu-id="51574-135">Name</span><span class="sxs-lookup"><span data-stu-id="51574-135">Name</span></span>          | <span data-ttu-id="51574-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51574-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="51574-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="51574-137">Authorization</span></span> | <span data-ttu-id="51574-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="51574-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="51574-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="51574-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="51574-141">CSV</span><span class="sxs-lookup"><span data-stu-id="51574-141">CSV</span></span>

<span data-ttu-id="51574-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="51574-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="51574-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="51574-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="51574-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="51574-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="51574-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="51574-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="51574-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="51574-146">Report Refresh Date</span></span>
- <span data-ttu-id="51574-147">Gesamt</span><span class="sxs-lookup"><span data-stu-id="51574-147">Total</span></span>
- <span data-ttu-id="51574-148">Aktiv</span><span class="sxs-lookup"><span data-stu-id="51574-148">Active</span></span>
- <span data-ttu-id="51574-149">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="51574-149">Report Date</span></span>
- <span data-ttu-id="51574-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="51574-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="51574-151">JSON</span><span class="sxs-lookup"><span data-stu-id="51574-151">JSON</span></span>

<span data-ttu-id="51574-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[MailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="51574-152">If successful, this method returns a `200 OK` response code and a **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51574-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51574-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="51574-154">CSV</span><span class="sxs-lookup"><span data-stu-id="51574-154">CSV</span></span>

<span data-ttu-id="51574-155">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="51574-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="51574-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51574-156">Request</span></span>

<span data-ttu-id="51574-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51574-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="51574-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="51574-158">Response</span></span>

<span data-ttu-id="51574-159">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="51574-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="51574-160">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="51574-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="51574-161">JSON</span><span class="sxs-lookup"><span data-stu-id="51574-161">JSON</span></span>

<span data-ttu-id="51574-162">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51574-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="51574-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51574-163">Request</span></span>

<span data-ttu-id="51574-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51574-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="51574-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="51574-165">Response</span></span>

<span data-ttu-id="51574-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="51574-166">The following is an example of the response.</span></span>

> <span data-ttu-id="51574-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="51574-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageMailboxCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 202, 
      "active": 198, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getmailboxusagemailboxcounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
