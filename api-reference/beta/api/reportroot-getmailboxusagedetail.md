---
title: 'reportRoot: getMailboxUsageDetail'
description: Erhalten Sie detaillierte Informationen über die Postfachnutzung.
ms.openlocfilehash: 317d258a51250992c47b20675bb2cb580ce408dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058146"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="e839f-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="e839f-103">reportRoot: getMailboxUsageDetail</span></span>

> <span data-ttu-id="e839f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e839f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e839f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e839f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e839f-106">Erhalten Sie detaillierte Informationen über die Postfachnutzung.</span><span class="sxs-lookup"><span data-stu-id="e839f-106">Get details about mailbox usage.</span></span>

> <span data-ttu-id="e839f-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Postfachnutzung](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="e839f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="e839f-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e839f-108">Permissions</span></span>

<span data-ttu-id="e839f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e839f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e839f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e839f-111">Permission type</span></span>                        | <span data-ttu-id="e839f-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e839f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e839f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e839f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e839f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e839f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e839f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e839f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e839f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e839f-116">Not supported.</span></span>                           |
| <span data-ttu-id="e839f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e839f-117">Application</span></span>                            | <span data-ttu-id="e839f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e839f-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e839f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e839f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e839f-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="e839f-120">Function parameters</span></span>

<span data-ttu-id="e839f-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="e839f-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e839f-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="e839f-122">Parameter</span></span> | <span data-ttu-id="e839f-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e839f-123">Type</span></span>   | <span data-ttu-id="e839f-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e839f-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e839f-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="e839f-125">period</span></span>    | <span data-ttu-id="e839f-126">string</span><span class="sxs-lookup"><span data-stu-id="e839f-126">string</span></span> | <span data-ttu-id="e839f-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="e839f-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e839f-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="e839f-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e839f-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="e839f-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e839f-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e839f-130">Required.</span></span> |

<span data-ttu-id="e839f-131">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e839f-131">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e839f-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="e839f-132">The default output type is text/csv.</span></span> <span data-ttu-id="e839f-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="e839f-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e839f-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e839f-134">Request headers</span></span>

| <span data-ttu-id="e839f-135">Name</span><span class="sxs-lookup"><span data-stu-id="e839f-135">Name</span></span>          | <span data-ttu-id="e839f-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e839f-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e839f-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="e839f-137">Authorization</span></span> | <span data-ttu-id="e839f-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e839f-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e839f-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="e839f-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e839f-141">CSV</span><span class="sxs-lookup"><span data-stu-id="e839f-141">CSV</span></span>

<span data-ttu-id="e839f-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="e839f-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e839f-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e839f-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e839f-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="e839f-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e839f-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="e839f-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e839f-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="e839f-146">Report Refresh Date</span></span>
- <span data-ttu-id="e839f-147">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="e839f-147">User Principal Name</span></span>
- <span data-ttu-id="e839f-148">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="e839f-148">Display Name</span></span>
- <span data-ttu-id="e839f-149">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="e839f-149">Is Deleted</span></span>
- <span data-ttu-id="e839f-150">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="e839f-150">Deleted Date</span></span>
- <span data-ttu-id="e839f-151">Erstellungsdatum</span><span class="sxs-lookup"><span data-stu-id="e839f-151">Created Date</span></span>
- <span data-ttu-id="e839f-152">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="e839f-152">Last Activity Date</span></span>
- <span data-ttu-id="e839f-153">Elementanzahl</span><span class="sxs-lookup"><span data-stu-id="e839f-153">Item Count</span></span>
- <span data-ttu-id="e839f-154">Verwendeter Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="e839f-154">Storage Used (Byte)</span></span>
- <span data-ttu-id="e839f-155">Kontingent für Problemwarnung (Byte)</span><span class="sxs-lookup"><span data-stu-id="e839f-155">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="e839f-156">Kontingent für Senden verbieten (Byte)</span><span class="sxs-lookup"><span data-stu-id="e839f-156">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="e839f-157">Kontingent für Senden/Empfangen verbieten (Byte)</span><span class="sxs-lookup"><span data-stu-id="e839f-157">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="e839f-158">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="e839f-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e839f-159">JSON</span><span class="sxs-lookup"><span data-stu-id="e839f-159">JSON</span></span>

<span data-ttu-id="e839f-160">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[MailboxUsageDetail](../resources/mailboxusagedetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e839f-160">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="e839f-161">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="e839f-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="e839f-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e839f-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e839f-163">CSV</span><span class="sxs-lookup"><span data-stu-id="e839f-163">CSV</span></span>

<span data-ttu-id="e839f-164">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="e839f-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e839f-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e839f-165">Request</span></span>

<span data-ttu-id="e839f-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e839f-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e839f-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="e839f-167">Response</span></span>

<span data-ttu-id="e839f-168">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e839f-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e839f-169">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="e839f-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="e839f-170">JSON</span><span class="sxs-lookup"><span data-stu-id="e839f-170">JSON</span></span>

<span data-ttu-id="e839f-171">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e839f-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e839f-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e839f-172">Request</span></span>

<span data-ttu-id="e839f-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e839f-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e839f-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="e839f-174">Response</span></span>

<span data-ttu-id="e839f-175">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e839f-175">The following is an example of the response.</span></span>

> <span data-ttu-id="e839f-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e839f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
