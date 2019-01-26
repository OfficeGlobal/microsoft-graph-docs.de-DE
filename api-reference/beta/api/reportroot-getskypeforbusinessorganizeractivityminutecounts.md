---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Erhalten Sie Informationen über die Dauer (in Minuten) und die Art der von Benutzern aus Ihrem Unternehmen gehaltenen und organisierten Konferenzsitzungen. Arten von Konferenzsitzungen sind Audio/Video und Einwahl/Auswahl - Microsoft.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7b20fd8dd9636b55bd614ebee8b1a3c19f38d7b0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571667"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="1d465-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="1d465-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d465-105">Erhalten Sie Informationen über die Dauer (in Minuten) und die Art der von Benutzern aus Ihrem Unternehmen gehaltenen und organisierten Konferenzsitzungen.</span><span class="sxs-lookup"><span data-stu-id="1d465-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="1d465-106">Arten von Konferenzsitzungen sind Audio/Video und Einwahl/Auswahl - Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1d465-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="1d465-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Konferenzorganisationsaktivität](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="1d465-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="1d465-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1d465-108">Permissions</span></span>

<span data-ttu-id="1d465-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d465-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1d465-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d465-111">Permission type</span></span>                        | <span data-ttu-id="1d465-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d465-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1d465-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d465-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d465-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d465-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1d465-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d465-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d465-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d465-116">Not supported.</span></span>                           |
| <span data-ttu-id="1d465-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d465-117">Application</span></span>                            | <span data-ttu-id="1d465-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d465-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1d465-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d465-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1d465-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="1d465-120">Function parameters</span></span>

<span data-ttu-id="1d465-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="1d465-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1d465-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="1d465-122">Parameter</span></span> | <span data-ttu-id="1d465-123">Typ</span><span class="sxs-lookup"><span data-stu-id="1d465-123">Type</span></span>   | <span data-ttu-id="1d465-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d465-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1d465-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="1d465-125">period</span></span>    | <span data-ttu-id="1d465-126">string</span><span class="sxs-lookup"><span data-stu-id="1d465-126">string</span></span> | <span data-ttu-id="1d465-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="1d465-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1d465-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="1d465-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1d465-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="1d465-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1d465-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="1d465-130">Required.</span></span> |

<span data-ttu-id="1d465-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1d465-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1d465-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="1d465-132">The default output type is text/csv.</span></span> <span data-ttu-id="1d465-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="1d465-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d465-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d465-134">Request headers</span></span>

| <span data-ttu-id="1d465-135">Name</span><span class="sxs-lookup"><span data-stu-id="1d465-135">Name</span></span>          | <span data-ttu-id="1d465-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d465-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1d465-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d465-137">Authorization</span></span> | <span data-ttu-id="1d465-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1d465-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1d465-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d465-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1d465-141">CSV</span><span class="sxs-lookup"><span data-stu-id="1d465-141">CSV</span></span>

<span data-ttu-id="1d465-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="1d465-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1d465-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1d465-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1d465-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="1d465-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1d465-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="1d465-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1d465-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="1d465-146">Report Refresh Date</span></span>
- <span data-ttu-id="1d465-147">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="1d465-147">Report Date</span></span>
- <span data-ttu-id="1d465-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="1d465-148">Report Period</span></span>
- <span data-ttu-id="1d465-149">Audio/Video</span><span class="sxs-lookup"><span data-stu-id="1d465-149">Audio/Video</span></span>
- <span data-ttu-id="1d465-150">Einwahl von Microsoft</span><span class="sxs-lookup"><span data-stu-id="1d465-150">Dial-in Microsoft</span></span>
- <span data-ttu-id="1d465-151">Auswahl von Microsoft</span><span class="sxs-lookup"><span data-stu-id="1d465-151">Dial-out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="1d465-152">JSON</span><span class="sxs-lookup"><span data-stu-id="1d465-152">JSON</span></span>

<span data-ttu-id="1d465-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1d465-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d465-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d465-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1d465-155">CSV</span><span class="sxs-lookup"><span data-stu-id="1d465-155">CSV</span></span>

<span data-ttu-id="1d465-156">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="1d465-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1d465-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d465-157">Request</span></span>

<span data-ttu-id="1d465-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d465-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1d465-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d465-159">Response</span></span>

<span data-ttu-id="1d465-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1d465-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1d465-161">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="1d465-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
```

### <a name="json"></a><span data-ttu-id="1d465-162">JSON</span><span class="sxs-lookup"><span data-stu-id="1d465-162">JSON</span></span>

<span data-ttu-id="1d465-163">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d465-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1d465-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d465-164">Request</span></span>

<span data-ttu-id="1d465-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d465-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1d465-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d465-166">Response</span></span>

<span data-ttu-id="1d465-167">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1d465-167">The following is an example of the response.</span></span>

> <span data-ttu-id="1d465-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1d465-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts)", 
  "value": [
    {
      "audioVideo": 1912, 
      "dialInMicrosoft": 108, 
      "dialOutMicrosoft": 0, 
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
