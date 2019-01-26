---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: Erhalten Sie Informationen über die Anzahl und die Art der von Benutzern aus Ihrem Unternehmen gehaltenen und organisierten Konferenzsitzungen. Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web, Einwahl/Auswahl Drittanbieter und Einwahl/Auswahl Microsoft.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8114091136e390c3a8fda62ed69ecf3b923ba852
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572290"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="5d735-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="5d735-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d735-105">Erhalten Sie Informationen über die Anzahl und die Art der von Benutzern aus Ihrem Unternehmen gehaltenen und organisierten Konferenzsitzungen.</span><span class="sxs-lookup"><span data-stu-id="5d735-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="5d735-106">Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web, Einwahl/Auswahl Drittanbieter und Einwahl/Auswahl Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5d735-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="5d735-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Konferenzorganisationsaktivität](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="5d735-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d735-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5d735-108">Permissions</span></span>

<span data-ttu-id="5d735-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d735-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d735-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d735-111">Permission type</span></span>                        | <span data-ttu-id="5d735-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d735-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5d735-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d735-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d735-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d735-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5d735-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d735-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d735-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d735-116">Not supported.</span></span>                           |
| <span data-ttu-id="5d735-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d735-117">Application</span></span>                            | <span data-ttu-id="5d735-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d735-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5d735-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d735-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5d735-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="5d735-120">Function parameters</span></span>

<span data-ttu-id="5d735-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="5d735-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5d735-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="5d735-122">Parameter</span></span> | <span data-ttu-id="5d735-123">Typ</span><span class="sxs-lookup"><span data-stu-id="5d735-123">Type</span></span>   | <span data-ttu-id="5d735-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d735-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5d735-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="5d735-125">period</span></span>    | <span data-ttu-id="5d735-126">string</span><span class="sxs-lookup"><span data-stu-id="5d735-126">string</span></span> | <span data-ttu-id="5d735-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="5d735-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5d735-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="5d735-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5d735-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="5d735-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5d735-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="5d735-130">Required.</span></span> |

<span data-ttu-id="5d735-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d735-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5d735-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="5d735-132">The default output type is text/csv.</span></span> <span data-ttu-id="5d735-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="5d735-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d735-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d735-134">Request headers</span></span>

| <span data-ttu-id="5d735-135">Name</span><span class="sxs-lookup"><span data-stu-id="5d735-135">Name</span></span>          | <span data-ttu-id="5d735-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d735-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5d735-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d735-137">Authorization</span></span> | <span data-ttu-id="5d735-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5d735-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5d735-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d735-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5d735-141">CSV</span><span class="sxs-lookup"><span data-stu-id="5d735-141">CSV</span></span>

<span data-ttu-id="5d735-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="5d735-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5d735-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d735-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5d735-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="5d735-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5d735-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="5d735-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5d735-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="5d735-146">Report Refresh Date</span></span>
- <span data-ttu-id="5d735-147">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="5d735-147">Report Date</span></span>
- <span data-ttu-id="5d735-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="5d735-148">Report Period</span></span>
- <span data-ttu-id="5d735-149">Chat</span><span class="sxs-lookup"><span data-stu-id="5d735-149">IM</span></span>
- <span data-ttu-id="5d735-150">Audio/Video</span><span class="sxs-lookup"><span data-stu-id="5d735-150">Audio/Video</span></span>
- <span data-ttu-id="5d735-151">Gemeinsame Nutzung von Anwendungen</span><span class="sxs-lookup"><span data-stu-id="5d735-151">App Sharing</span></span>
- <span data-ttu-id="5d735-152">Web</span><span class="sxs-lookup"><span data-stu-id="5d735-152">Web</span></span>
- <span data-ttu-id="5d735-153">Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="5d735-153">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="5d735-154">Einwahl/Auswahl Microsoft</span><span class="sxs-lookup"><span data-stu-id="5d735-154">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="5d735-155">JSON</span><span class="sxs-lookup"><span data-stu-id="5d735-155">JSON</span></span>

<span data-ttu-id="5d735-156">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5d735-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d735-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d735-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5d735-158">CSV</span><span class="sxs-lookup"><span data-stu-id="5d735-158">CSV</span></span>

<span data-ttu-id="5d735-159">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="5d735-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5d735-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d735-160">Request</span></span>

<span data-ttu-id="5d735-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d735-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="5d735-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d735-162">Response</span></span>

<span data-ttu-id="5d735-163">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d735-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5d735-164">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="5d735-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5d735-165">JSON</span><span class="sxs-lookup"><span data-stu-id="5d735-165">JSON</span></span>

<span data-ttu-id="5d735-166">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d735-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5d735-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d735-167">Request</span></span>

<span data-ttu-id="5d735-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d735-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="5d735-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d735-169">Response</span></span>

<span data-ttu-id="5d735-170">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d735-170">The following is an example of the response.</span></span>

> <span data-ttu-id="5d735-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5d735-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityCounts)", 
  "value": [
    {
      "im": 20, 
      "audioVideo": 43, 
      "appSharing": 20, 
      "web": 6, 
      "dialInOut3rdParty": 0, 
      "dialInOutMicrosoft": 48, 
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
