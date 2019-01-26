---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: Erhalten Sie Informationen über die Anzahl und Art der in Ihrem Unternehmen gehaltenen Sitzungen. Zu den Sitzungsarten gehören Chat, Audio, Video, Anwendungsfreigabe und Dateiübertragung.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4b080c7ed60f07c78dcf11574277b08086613d5a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576941"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="11707-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="11707-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11707-105">Erhalten Sie Informationen über die Anzahl und Art der in Ihrem Unternehmen gehaltenen Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="11707-105">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="11707-106">Zu den Sitzungsarten gehören Chat, Audio, Video, Anwendungsfreigabe und Dateiübertragung.</span><span class="sxs-lookup"><span data-stu-id="11707-106">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="11707-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Peer-to-Peer-Aktivität](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="11707-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="11707-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="11707-108">Permissions</span></span>

<span data-ttu-id="11707-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11707-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11707-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11707-111">Permission type</span></span>                        | <span data-ttu-id="11707-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11707-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="11707-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11707-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="11707-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11707-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="11707-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11707-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11707-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11707-116">Not supported.</span></span>                           |
| <span data-ttu-id="11707-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11707-117">Application</span></span>                            | <span data-ttu-id="11707-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11707-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="11707-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11707-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="11707-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="11707-120">Function parameters</span></span>

<span data-ttu-id="11707-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="11707-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="11707-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="11707-122">Parameter</span></span> | <span data-ttu-id="11707-123">Typ</span><span class="sxs-lookup"><span data-stu-id="11707-123">Type</span></span>   | <span data-ttu-id="11707-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11707-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="11707-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="11707-125">period</span></span>    | <span data-ttu-id="11707-126">string</span><span class="sxs-lookup"><span data-stu-id="11707-126">string</span></span> | <span data-ttu-id="11707-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="11707-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="11707-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="11707-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="11707-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="11707-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="11707-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="11707-130">Required.</span></span> |

<span data-ttu-id="11707-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="11707-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="11707-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="11707-132">The default output type is text/csv.</span></span> <span data-ttu-id="11707-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="11707-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11707-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11707-134">Request headers</span></span>

| <span data-ttu-id="11707-135">Name</span><span class="sxs-lookup"><span data-stu-id="11707-135">Name</span></span>          | <span data-ttu-id="11707-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11707-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="11707-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="11707-137">Authorization</span></span> | <span data-ttu-id="11707-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="11707-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="11707-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="11707-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="11707-141">CSV</span><span class="sxs-lookup"><span data-stu-id="11707-141">CSV</span></span>

<span data-ttu-id="11707-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="11707-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="11707-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="11707-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="11707-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="11707-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="11707-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="11707-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="11707-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="11707-146">Report Refresh Date</span></span>
- <span data-ttu-id="11707-147">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="11707-147">Report Date</span></span>
- <span data-ttu-id="11707-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="11707-148">Report Period</span></span>
- <span data-ttu-id="11707-149">Chat</span><span class="sxs-lookup"><span data-stu-id="11707-149">IM</span></span>
- <span data-ttu-id="11707-150">Audio</span><span class="sxs-lookup"><span data-stu-id="11707-150">Audio</span></span>
- <span data-ttu-id="11707-151">Video</span><span class="sxs-lookup"><span data-stu-id="11707-151">Video</span></span>
- <span data-ttu-id="11707-152">Gemeinsame Nutzung von Anwendungen</span><span class="sxs-lookup"><span data-stu-id="11707-152">App Sharing</span></span>
- <span data-ttu-id="11707-153">Dateiübertragung</span><span class="sxs-lookup"><span data-stu-id="11707-153">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="11707-154">JSON</span><span class="sxs-lookup"><span data-stu-id="11707-154">JSON</span></span>

<span data-ttu-id="11707-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="11707-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11707-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11707-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="11707-157">CSV</span><span class="sxs-lookup"><span data-stu-id="11707-157">CSV</span></span>

<span data-ttu-id="11707-158">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="11707-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="11707-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11707-159">Request</span></span>

<span data-ttu-id="11707-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11707-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="11707-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="11707-161">Response</span></span>

<span data-ttu-id="11707-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="11707-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="11707-163">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="11707-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```

### <a name="json"></a><span data-ttu-id="11707-164">JSON</span><span class="sxs-lookup"><span data-stu-id="11707-164">JSON</span></span>

<span data-ttu-id="11707-165">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11707-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="11707-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11707-166">Request</span></span>

<span data-ttu-id="11707-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11707-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="11707-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="11707-168">Response</span></span>

<span data-ttu-id="11707-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="11707-169">The following is an example of the response.</span></span>

> <span data-ttu-id="11707-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="11707-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityCounts)", 
  "value": [
    {
      "im": 1177, 
      "audio": 107, 
      "video": 7, 
      "appSharing": 74, 
      "fileTransfer": 24, 
      "reportRefreshDate": "2017-09-01", 
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
