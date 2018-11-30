---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: Erhalten Sie Informationen über die Anzahl und die Art der von Benutzern aus Ihrem Unternehmen gehaltenen und organisierten Konferenzsitzungen. Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web, Einwahl/Auswahl Drittanbieter und Einwahl/Auswahl Microsoft.
ms.openlocfilehash: 79711fe618c0549b56779a957d1bce8825debae5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059154"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="e81b5-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="e81b5-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

> <span data-ttu-id="e81b5-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e81b5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e81b5-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e81b5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e81b5-107">Erhalten Sie Informationen über die Anzahl und die Art der von Benutzern aus Ihrem Unternehmen gehaltenen und organisierten Konferenzsitzungen.</span><span class="sxs-lookup"><span data-stu-id="e81b5-107">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="e81b5-108">Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web, Einwahl/Auswahl Drittanbieter und Einwahl/Auswahl Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e81b5-108">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="e81b5-109">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Konferenzorganisationsaktivität](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="e81b5-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="e81b5-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e81b5-110">Permissions</span></span>

<span data-ttu-id="e81b5-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e81b5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e81b5-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e81b5-113">Permission type</span></span>                        | <span data-ttu-id="e81b5-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e81b5-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e81b5-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e81b5-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e81b5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e81b5-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e81b5-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e81b5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e81b5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e81b5-118">Not supported.</span></span>                           |
| <span data-ttu-id="e81b5-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e81b5-119">Application</span></span>                            | <span data-ttu-id="e81b5-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e81b5-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e81b5-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e81b5-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e81b5-122">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="e81b5-122">Function parameters</span></span>

<span data-ttu-id="e81b5-123">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="e81b5-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e81b5-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="e81b5-124">Parameter</span></span> | <span data-ttu-id="e81b5-125">Typ</span><span class="sxs-lookup"><span data-stu-id="e81b5-125">Type</span></span>   | <span data-ttu-id="e81b5-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e81b5-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e81b5-127">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="e81b5-127">period</span></span>    | <span data-ttu-id="e81b5-128">string</span><span class="sxs-lookup"><span data-stu-id="e81b5-128">string</span></span> | <span data-ttu-id="e81b5-129">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="e81b5-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e81b5-130">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="e81b5-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e81b5-131">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="e81b5-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e81b5-132">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e81b5-132">Required.</span></span> |

<span data-ttu-id="e81b5-133">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e81b5-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e81b5-134">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="e81b5-134">The default output type is text/csv.</span></span> <span data-ttu-id="e81b5-135">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="e81b5-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e81b5-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e81b5-136">Request headers</span></span>

| <span data-ttu-id="e81b5-137">Name</span><span class="sxs-lookup"><span data-stu-id="e81b5-137">Name</span></span>          | <span data-ttu-id="e81b5-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e81b5-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e81b5-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="e81b5-139">Authorization</span></span> | <span data-ttu-id="e81b5-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e81b5-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e81b5-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="e81b5-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e81b5-143">CSV</span><span class="sxs-lookup"><span data-stu-id="e81b5-143">CSV</span></span>

<span data-ttu-id="e81b5-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="e81b5-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e81b5-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e81b5-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e81b5-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="e81b5-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e81b5-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="e81b5-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e81b5-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="e81b5-148">Report Refresh Date</span></span>
- <span data-ttu-id="e81b5-149">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="e81b5-149">Report Date</span></span>
- <span data-ttu-id="e81b5-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="e81b5-150">Report Period</span></span>
- <span data-ttu-id="e81b5-151">Chat</span><span class="sxs-lookup"><span data-stu-id="e81b5-151">IM</span></span>
- <span data-ttu-id="e81b5-152">Audio/Video</span><span class="sxs-lookup"><span data-stu-id="e81b5-152">Audio/Video</span></span>
- <span data-ttu-id="e81b5-153">Gemeinsame Nutzung von Anwendungen</span><span class="sxs-lookup"><span data-stu-id="e81b5-153">App Sharing</span></span>
- <span data-ttu-id="e81b5-154">Web</span><span class="sxs-lookup"><span data-stu-id="e81b5-154">Web</span></span>
- <span data-ttu-id="e81b5-155">Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="e81b5-155">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="e81b5-156">Einwahl/Auswahl Microsoft</span><span class="sxs-lookup"><span data-stu-id="e81b5-156">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="e81b5-157">JSON</span><span class="sxs-lookup"><span data-stu-id="e81b5-157">JSON</span></span>

<span data-ttu-id="e81b5-158">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e81b5-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e81b5-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e81b5-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e81b5-160">CSV</span><span class="sxs-lookup"><span data-stu-id="e81b5-160">CSV</span></span>

<span data-ttu-id="e81b5-161">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="e81b5-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e81b5-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e81b5-162">Request</span></span>

<span data-ttu-id="e81b5-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e81b5-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e81b5-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="e81b5-164">Response</span></span>

<span data-ttu-id="e81b5-165">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e81b5-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e81b5-166">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="e81b5-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="e81b5-167">JSON</span><span class="sxs-lookup"><span data-stu-id="e81b5-167">JSON</span></span>

<span data-ttu-id="e81b5-168">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e81b5-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e81b5-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e81b5-169">Request</span></span>

<span data-ttu-id="e81b5-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e81b5-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e81b5-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="e81b5-171">Response</span></span>

<span data-ttu-id="e81b5-172">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e81b5-172">The following is an example of the response.</span></span>

> <span data-ttu-id="e81b5-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e81b5-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
