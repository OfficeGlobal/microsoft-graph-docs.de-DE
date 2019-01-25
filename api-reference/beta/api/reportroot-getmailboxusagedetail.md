---
title: 'reportRoot: getMailboxUsageDetail'
description: Erhalten Sie detaillierte Informationen über die Postfachnutzung.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d7844978d0a7f0fb2617def7a55782dbf6cb61c3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511261"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="0153b-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="0153b-103">reportRoot: getMailboxUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0153b-104">Erhalten Sie detaillierte Informationen über die Postfachnutzung.</span><span class="sxs-lookup"><span data-stu-id="0153b-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="0153b-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Postfachnutzung](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="0153b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="0153b-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0153b-106">Permissions</span></span>

<span data-ttu-id="0153b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0153b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0153b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0153b-109">Permission type</span></span>                        | <span data-ttu-id="0153b-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0153b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0153b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0153b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0153b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0153b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0153b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0153b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0153b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0153b-114">Not supported.</span></span>                           |
| <span data-ttu-id="0153b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0153b-115">Application</span></span>                            | <span data-ttu-id="0153b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0153b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0153b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0153b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0153b-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="0153b-118">Function parameters</span></span>

<span data-ttu-id="0153b-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="0153b-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0153b-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="0153b-120">Parameter</span></span> | <span data-ttu-id="0153b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0153b-121">Type</span></span>   | <span data-ttu-id="0153b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0153b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0153b-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="0153b-123">period</span></span>    | <span data-ttu-id="0153b-124">string</span><span class="sxs-lookup"><span data-stu-id="0153b-124">string</span></span> | <span data-ttu-id="0153b-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0153b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0153b-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="0153b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0153b-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0153b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0153b-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="0153b-128">Required.</span></span> |

<span data-ttu-id="0153b-129">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0153b-129">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0153b-130">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="0153b-130">The default output type is text/csv.</span></span> <span data-ttu-id="0153b-131">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="0153b-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0153b-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0153b-132">Request headers</span></span>

| <span data-ttu-id="0153b-133">Name</span><span class="sxs-lookup"><span data-stu-id="0153b-133">Name</span></span>          | <span data-ttu-id="0153b-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0153b-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0153b-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="0153b-135">Authorization</span></span> | <span data-ttu-id="0153b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0153b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0153b-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="0153b-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0153b-139">CSV</span><span class="sxs-lookup"><span data-stu-id="0153b-139">CSV</span></span>

<span data-ttu-id="0153b-140">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="0153b-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0153b-141">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0153b-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0153b-142">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="0153b-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0153b-143">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="0153b-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0153b-144">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="0153b-144">Report Refresh Date</span></span>
- <span data-ttu-id="0153b-145">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="0153b-145">User Principal Name</span></span>
- <span data-ttu-id="0153b-146">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="0153b-146">Display Name</span></span>
- <span data-ttu-id="0153b-147">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="0153b-147">Is Deleted</span></span>
- <span data-ttu-id="0153b-148">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="0153b-148">Deleted Date</span></span>
- <span data-ttu-id="0153b-149">Erstellungsdatum</span><span class="sxs-lookup"><span data-stu-id="0153b-149">Created Date</span></span>
- <span data-ttu-id="0153b-150">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="0153b-150">Last Activity Date</span></span>
- <span data-ttu-id="0153b-151">Elementanzahl</span><span class="sxs-lookup"><span data-stu-id="0153b-151">Item Count</span></span>
- <span data-ttu-id="0153b-152">Verwendeter Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="0153b-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="0153b-153">Kontingent für Problemwarnung (Byte)</span><span class="sxs-lookup"><span data-stu-id="0153b-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="0153b-154">Kontingent für Senden verbieten (Byte)</span><span class="sxs-lookup"><span data-stu-id="0153b-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="0153b-155">Kontingent für Senden/Empfangen verbieten (Byte)</span><span class="sxs-lookup"><span data-stu-id="0153b-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="0153b-156">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="0153b-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0153b-157">JSON</span><span class="sxs-lookup"><span data-stu-id="0153b-157">JSON</span></span>

<span data-ttu-id="0153b-158">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[MailboxUsageDetail](../resources/mailboxusagedetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0153b-158">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="0153b-159">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="0153b-159">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="0153b-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0153b-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0153b-161">CSV</span><span class="sxs-lookup"><span data-stu-id="0153b-161">CSV</span></span>

<span data-ttu-id="0153b-162">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="0153b-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0153b-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0153b-163">Request</span></span>

<span data-ttu-id="0153b-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0153b-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0153b-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="0153b-165">Response</span></span>

<span data-ttu-id="0153b-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0153b-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0153b-167">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="0153b-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="0153b-168">JSON</span><span class="sxs-lookup"><span data-stu-id="0153b-168">JSON</span></span>

<span data-ttu-id="0153b-169">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0153b-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0153b-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0153b-170">Request</span></span>

<span data-ttu-id="0153b-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0153b-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0153b-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="0153b-172">Response</span></span>

<span data-ttu-id="0153b-173">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0153b-173">The following is an example of the response.</span></span>

> <span data-ttu-id="0153b-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0153b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "createdDate": "2016-03-30", 
      "lastActivityDate": "2017-09-01", 
      "itemCount": 138481, 
      "storageUsedInBytes": 10414748704, 
      "issueWarningQuotaInBytes": 10522698752, 
      "prohibitSendQuotaInBytes": 10630040576, 
      "prohibitSendReceiveQuotaInBytes": 10737418240, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getmailboxusagedetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
