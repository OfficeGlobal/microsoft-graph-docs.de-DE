---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Rufen Sie die Anzahl der Gruppenaktivitäten für Gruppenarbeitslasten ab.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 72c879af55f8608dd8f5cd2f1086f8469aacb651
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571723"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="4c227-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4c227-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c227-104">Rufen Sie die Anzahl der Gruppenaktivitäten für Gruppenarbeitslasten ab.</span><span class="sxs-lookup"><span data-stu-id="4c227-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="4c227-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="4c227-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c227-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4c227-106">Permissions</span></span>

<span data-ttu-id="4c227-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c227-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c227-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4c227-109">Permission type</span></span>                        | <span data-ttu-id="4c227-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4c227-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4c227-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4c227-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c227-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c227-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4c227-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4c227-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c227-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c227-114">Not supported.</span></span>                           |
| <span data-ttu-id="4c227-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4c227-115">Application</span></span>                            | <span data-ttu-id="4c227-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c227-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4c227-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c227-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4c227-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="4c227-118">Function parameters</span></span>

<span data-ttu-id="4c227-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="4c227-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4c227-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="4c227-120">Parameter</span></span> | <span data-ttu-id="4c227-121">Typ</span><span class="sxs-lookup"><span data-stu-id="4c227-121">Type</span></span>   | <span data-ttu-id="4c227-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c227-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4c227-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="4c227-123">period</span></span>    | <span data-ttu-id="4c227-124">string</span><span class="sxs-lookup"><span data-stu-id="4c227-124">string</span></span> | <span data-ttu-id="4c227-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="4c227-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4c227-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="4c227-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4c227-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="4c227-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4c227-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="4c227-128">Required.</span></span> |

<span data-ttu-id="4c227-129">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4c227-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4c227-130">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="4c227-130">The default output type is text/csv.</span></span> <span data-ttu-id="4c227-131">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="4c227-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c227-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4c227-132">Request headers</span></span>

| <span data-ttu-id="4c227-133">Name</span><span class="sxs-lookup"><span data-stu-id="4c227-133">Name</span></span>          | <span data-ttu-id="4c227-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c227-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4c227-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c227-135">Authorization</span></span> | <span data-ttu-id="4c227-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4c227-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4c227-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c227-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4c227-139">CSV</span><span class="sxs-lookup"><span data-stu-id="4c227-139">CSV</span></span>

<span data-ttu-id="4c227-140">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="4c227-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4c227-141">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4c227-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4c227-142">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="4c227-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4c227-143">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="4c227-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4c227-144">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="4c227-144">Report Refresh Date</span></span>
- <span data-ttu-id="4c227-145">Empfangene Exchange-E-Mails</span><span class="sxs-lookup"><span data-stu-id="4c227-145">Exchange Emails Received</span></span>
- <span data-ttu-id="4c227-146">Veröffentlichte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4c227-146">Yammer Messages Posted</span></span>
- <span data-ttu-id="4c227-147">Gelesene Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4c227-147">Yammer Messages Read</span></span>
- <span data-ttu-id="4c227-148">Gelikte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4c227-148">Yammer Messages Liked</span></span>
- <span data-ttu-id="4c227-149">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="4c227-149">Report Date</span></span>
- <span data-ttu-id="4c227-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="4c227-150">Report Period</span></span>

<span data-ttu-id="4c227-151">Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="4c227-151">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="4c227-152">Veröffentlichte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4c227-152">Yammer Messages Posted</span></span>
- <span data-ttu-id="4c227-153">Gelesene Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4c227-153">Yammer Messages Read</span></span>
- <span data-ttu-id="4c227-154">Gelikte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4c227-154">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="4c227-155">JSON</span><span class="sxs-lookup"><span data-stu-id="4c227-155">JSON</span></span>

<span data-ttu-id="4c227-156">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4c227-156">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="4c227-157">Die folgenden Eigenschaften im **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="4c227-157">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="4c227-158">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="4c227-158">yammerMessagesPosted</span></span>
- <span data-ttu-id="4c227-159">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="4c227-159">yammerMessagesRead</span></span>
- <span data-ttu-id="4c227-160">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="4c227-160">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="4c227-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4c227-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4c227-162">CSV</span><span class="sxs-lookup"><span data-stu-id="4c227-162">CSV</span></span>

<span data-ttu-id="4c227-163">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="4c227-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4c227-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c227-164">Request</span></span>

<span data-ttu-id="4c227-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4c227-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4c227-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c227-166">Response</span></span>

<span data-ttu-id="4c227-167">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4c227-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4c227-168">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="4c227-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="4c227-169">JSON</span><span class="sxs-lookup"><span data-stu-id="4c227-169">JSON</span></span>

<span data-ttu-id="4c227-170">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4c227-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4c227-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c227-171">Request</span></span>

<span data-ttu-id="4c227-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4c227-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4c227-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c227-173">Response</span></span>

<span data-ttu-id="4c227-174">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4c227-174">The following is an example of the response.</span></span>

> <span data-ttu-id="4c227-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4c227-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeEmailsReceived": 0, 
      "yammerMessagesPosted": 0, 
      "yammerMessagesRead": 0, 
      "yammerMessagesLiked": 0, 
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
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
