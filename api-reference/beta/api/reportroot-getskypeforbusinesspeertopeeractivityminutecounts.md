---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Erhalten Sie Informationen über die Dauer (in Minuten) und die Art der in Ihrem Unternehmen gehaltenen Peer-to-Peer-Sitzungen. Zu den Sitzungsarten gehören Audio und Video.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 357c3d2e972cc70be4d517556946a6c08d56b447
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945083"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="65506-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="65506-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

> <span data-ttu-id="65506-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="65506-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65506-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65506-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65506-107">Erhalten Sie Informationen über die Dauer (in Minuten) und die Art der in Ihrem Unternehmen gehaltenen Peer-to-Peer-Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="65506-107">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="65506-108">Zu den Sitzungsarten gehören Audio und Video.</span><span class="sxs-lookup"><span data-stu-id="65506-108">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="65506-109">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Peer-to-Peer-Aktivität](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="65506-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="65506-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="65506-110">Permissions</span></span>

<span data-ttu-id="65506-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65506-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65506-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65506-113">Permission type</span></span>                        | <span data-ttu-id="65506-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65506-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="65506-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65506-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="65506-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65506-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="65506-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65506-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65506-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65506-118">Not supported.</span></span>                           |
| <span data-ttu-id="65506-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65506-119">Application</span></span>                            | <span data-ttu-id="65506-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65506-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="65506-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65506-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="65506-122">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="65506-122">Function parameters</span></span>

<span data-ttu-id="65506-123">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="65506-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="65506-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="65506-124">Parameter</span></span> | <span data-ttu-id="65506-125">Typ</span><span class="sxs-lookup"><span data-stu-id="65506-125">Type</span></span>   | <span data-ttu-id="65506-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65506-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="65506-127">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="65506-127">period</span></span>    | <span data-ttu-id="65506-128">string</span><span class="sxs-lookup"><span data-stu-id="65506-128">string</span></span> | <span data-ttu-id="65506-129">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="65506-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="65506-130">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="65506-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="65506-131">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="65506-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="65506-132">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="65506-132">Required.</span></span> |

<span data-ttu-id="65506-133">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="65506-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="65506-134">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="65506-134">The default output type is text/csv.</span></span> <span data-ttu-id="65506-135">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="65506-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65506-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65506-136">Request headers</span></span>

| <span data-ttu-id="65506-137">Name</span><span class="sxs-lookup"><span data-stu-id="65506-137">Name</span></span>          | <span data-ttu-id="65506-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65506-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="65506-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="65506-139">Authorization</span></span> | <span data-ttu-id="65506-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="65506-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="65506-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="65506-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="65506-143">CSV</span><span class="sxs-lookup"><span data-stu-id="65506-143">CSV</span></span>

<span data-ttu-id="65506-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="65506-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="65506-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="65506-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="65506-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="65506-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="65506-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="65506-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="65506-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="65506-148">Report Refresh Date</span></span>
- <span data-ttu-id="65506-149">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="65506-149">Report Date</span></span>
- <span data-ttu-id="65506-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="65506-150">Report Period</span></span>
- <span data-ttu-id="65506-151">Audio</span><span class="sxs-lookup"><span data-stu-id="65506-151">Audio</span></span>
- <span data-ttu-id="65506-152">Video</span><span class="sxs-lookup"><span data-stu-id="65506-152">Video</span></span>

### <a name="json"></a><span data-ttu-id="65506-153">JSON</span><span class="sxs-lookup"><span data-stu-id="65506-153">JSON</span></span>

<span data-ttu-id="65506-154">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="65506-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65506-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65506-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="65506-156">CSV</span><span class="sxs-lookup"><span data-stu-id="65506-156">CSV</span></span>

<span data-ttu-id="65506-157">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="65506-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="65506-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65506-158">Request</span></span>

<span data-ttu-id="65506-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65506-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="65506-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="65506-160">Response</span></span>

<span data-ttu-id="65506-161">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="65506-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="65506-162">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="65506-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
```

### <a name="json"></a><span data-ttu-id="65506-163">JSON</span><span class="sxs-lookup"><span data-stu-id="65506-163">JSON</span></span>

<span data-ttu-id="65506-164">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65506-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="65506-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65506-165">Request</span></span>

<span data-ttu-id="65506-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65506-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="65506-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="65506-167">Response</span></span>

<span data-ttu-id="65506-168">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="65506-168">The following is an example of the response.</span></span>

> <span data-ttu-id="65506-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="65506-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts)", 
  "value": [
    {
      "audio": 836, 
      "video": 35, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
