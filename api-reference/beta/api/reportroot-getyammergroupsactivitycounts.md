---
title: 'reportRoot: getYammerGroupsActivityCounts'
description: Rufen Sie die Anzahl der in Gruppen veröffentlichten, gelesenen und gelikten Yammer-Nachrichten ab.
ms.openlocfilehash: 2850bf9e1076f545005721062ee8cf4733d55bb5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063503"
---
# <a name="reportroot-getyammergroupsactivitycounts"></a><span data-ttu-id="40e69-103">reportRoot: getYammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="40e69-103">reportRoot: getYammerGroupsActivityCounts</span></span>

> <span data-ttu-id="40e69-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="40e69-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40e69-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40e69-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40e69-106">Rufen Sie die Anzahl der in Gruppen veröffentlichten, gelesenen und gelikten Yammer-Nachrichten ab.</span><span class="sxs-lookup"><span data-stu-id="40e69-106">Get the number of Yammer messages posted, read, and liked in groups.</span></span>

> <span data-ttu-id="40e69-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gruppenaktivität](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="40e69-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="40e69-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="40e69-108">Permissions</span></span>

<span data-ttu-id="40e69-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40e69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40e69-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40e69-111">Permission type</span></span>                        | <span data-ttu-id="40e69-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40e69-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="40e69-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40e69-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="40e69-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="40e69-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="40e69-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40e69-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40e69-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40e69-116">Not supported.</span></span>                           |
| <span data-ttu-id="40e69-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40e69-117">Application</span></span>                            | <span data-ttu-id="40e69-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="40e69-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="40e69-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40e69-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="40e69-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="40e69-120">Function parameters</span></span>

<span data-ttu-id="40e69-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="40e69-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="40e69-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="40e69-122">Parameter</span></span> | <span data-ttu-id="40e69-123">Typ</span><span class="sxs-lookup"><span data-stu-id="40e69-123">Type</span></span>   | <span data-ttu-id="40e69-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40e69-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="40e69-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="40e69-125">period</span></span>    | <span data-ttu-id="40e69-126">string</span><span class="sxs-lookup"><span data-stu-id="40e69-126">string</span></span> | <span data-ttu-id="40e69-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="40e69-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="40e69-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="40e69-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="40e69-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="40e69-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="40e69-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="40e69-130">Required.</span></span> |

<span data-ttu-id="40e69-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="40e69-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="40e69-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="40e69-132">The default output type is text/csv.</span></span> <span data-ttu-id="40e69-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="40e69-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40e69-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40e69-134">Request headers</span></span>

| <span data-ttu-id="40e69-135">Name</span><span class="sxs-lookup"><span data-stu-id="40e69-135">Name</span></span>          | <span data-ttu-id="40e69-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40e69-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="40e69-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="40e69-137">Authorization</span></span> | <span data-ttu-id="40e69-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="40e69-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="40e69-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="40e69-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="40e69-141">CSV</span><span class="sxs-lookup"><span data-stu-id="40e69-141">CSV</span></span>

<span data-ttu-id="40e69-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="40e69-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="40e69-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="40e69-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="40e69-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="40e69-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="40e69-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="40e69-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="40e69-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="40e69-146">Report Refresh Date</span></span>
- <span data-ttu-id="40e69-147">Gelikt</span><span class="sxs-lookup"><span data-stu-id="40e69-147">Liked</span></span>
- <span data-ttu-id="40e69-148">Gepostet</span><span class="sxs-lookup"><span data-stu-id="40e69-148">Posted</span></span>
- <span data-ttu-id="40e69-149">Gelesen</span><span class="sxs-lookup"><span data-stu-id="40e69-149">Read</span></span>
- <span data-ttu-id="40e69-150">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="40e69-150">Report Date</span></span>
- <span data-ttu-id="40e69-151">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="40e69-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="40e69-152">JSON</span><span class="sxs-lookup"><span data-stu-id="40e69-152">JSON</span></span>

<span data-ttu-id="40e69-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[YammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="40e69-153">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40e69-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40e69-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="40e69-155">CSV</span><span class="sxs-lookup"><span data-stu-id="40e69-155">CSV</span></span>

<span data-ttu-id="40e69-156">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="40e69-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="40e69-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40e69-157">Request</span></span>

<span data-ttu-id="40e69-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40e69-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="40e69-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="40e69-159">Response</span></span>

<span data-ttu-id="40e69-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="40e69-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="40e69-161">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="40e69-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="40e69-162">JSON</span><span class="sxs-lookup"><span data-stu-id="40e69-162">JSON</span></span>

<span data-ttu-id="40e69-163">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40e69-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="40e69-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40e69-164">Request</span></span>

<span data-ttu-id="40e69-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40e69-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="40e69-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="40e69-166">Response</span></span>

<span data-ttu-id="40e69-167">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="40e69-167">The following is an example of the response.</span></span>

> <span data-ttu-id="40e69-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="40e69-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 241

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 13, 
      "posted": 50, 
      "read": 69, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
