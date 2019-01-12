---
title: 'reportRoot: getOneDriveActivityUserCounts'
description: Rufen Sie die Anzahl der aktiven OneDrive-Benutzer ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 727dbfc08c029b4a85b227f0d86c739463af0c94
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954057"
---
# <a name="reportroot-getonedriveactivityusercounts"></a><span data-ttu-id="08e6d-103">reportRoot: getOneDriveActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="08e6d-103">reportRoot: getOneDriveActivityUserCounts</span></span>

> <span data-ttu-id="08e6d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="08e6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08e6d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08e6d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08e6d-106">Rufen Sie die Anzahl der aktiven OneDrive-Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="08e6d-106">Get the trend in the number of active OneDrive users.</span></span>

> <span data-ttu-id="08e6d-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Aktivität](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="08e6d-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="08e6d-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="08e6d-108">Permissions</span></span>

<span data-ttu-id="08e6d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08e6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08e6d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08e6d-111">Permission type</span></span>                        | <span data-ttu-id="08e6d-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08e6d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="08e6d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08e6d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="08e6d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08e6d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="08e6d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08e6d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08e6d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08e6d-116">Not supported.</span></span>                           |
| <span data-ttu-id="08e6d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08e6d-117">Application</span></span>                            | <span data-ttu-id="08e6d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08e6d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="08e6d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08e6d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="08e6d-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="08e6d-120">Function parameters</span></span>

<span data-ttu-id="08e6d-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="08e6d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="08e6d-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="08e6d-122">Parameter</span></span> | <span data-ttu-id="08e6d-123">Typ</span><span class="sxs-lookup"><span data-stu-id="08e6d-123">Type</span></span>   | <span data-ttu-id="08e6d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08e6d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="08e6d-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="08e6d-125">period</span></span>    | <span data-ttu-id="08e6d-126">string</span><span class="sxs-lookup"><span data-stu-id="08e6d-126">string</span></span> | <span data-ttu-id="08e6d-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="08e6d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="08e6d-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="08e6d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="08e6d-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="08e6d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="08e6d-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="08e6d-130">Required.</span></span> |

<span data-ttu-id="08e6d-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="08e6d-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="08e6d-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="08e6d-132">The default output type is text/csv.</span></span> <span data-ttu-id="08e6d-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="08e6d-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08e6d-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08e6d-134">Request headers</span></span>

| <span data-ttu-id="08e6d-135">Name</span><span class="sxs-lookup"><span data-stu-id="08e6d-135">Name</span></span>          | <span data-ttu-id="08e6d-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08e6d-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="08e6d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="08e6d-137">Authorization</span></span> | <span data-ttu-id="08e6d-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="08e6d-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="08e6d-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="08e6d-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="08e6d-141">CSV</span><span class="sxs-lookup"><span data-stu-id="08e6d-141">CSV</span></span>

<span data-ttu-id="08e6d-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="08e6d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="08e6d-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="08e6d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="08e6d-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="08e6d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="08e6d-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="08e6d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="08e6d-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="08e6d-146">Report Refresh Date</span></span>
- <span data-ttu-id="08e6d-147">Angezeigt oder Bearbeitet</span><span class="sxs-lookup"><span data-stu-id="08e6d-147">Viewed Or Edited</span></span>
- <span data-ttu-id="08e6d-148">Synchronisiert</span><span class="sxs-lookup"><span data-stu-id="08e6d-148">Synced</span></span>
- <span data-ttu-id="08e6d-149">Intern freigegeben</span><span class="sxs-lookup"><span data-stu-id="08e6d-149">Shared Internally</span></span>
- <span data-ttu-id="08e6d-150">Extern freigegeben</span><span class="sxs-lookup"><span data-stu-id="08e6d-150">Shared Externally</span></span>
- <span data-ttu-id="08e6d-151">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="08e6d-151">Report Date</span></span>
- <span data-ttu-id="08e6d-152">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="08e6d-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="08e6d-153">JSON</span><span class="sxs-lookup"><span data-stu-id="08e6d-153">JSON</span></span>

<span data-ttu-id="08e6d-154">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SiteActivitySummary](../resources/siteactivitysummary.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="08e6d-154">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08e6d-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08e6d-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="08e6d-156">CSV</span><span class="sxs-lookup"><span data-stu-id="08e6d-156">CSV</span></span>

<span data-ttu-id="08e6d-157">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="08e6d-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="08e6d-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08e6d-158">Request</span></span>

<span data-ttu-id="08e6d-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08e6d-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="08e6d-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="08e6d-160">Response</span></span>

<span data-ttu-id="08e6d-161">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="08e6d-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="08e6d-162">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="08e6d-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="08e6d-163">JSON</span><span class="sxs-lookup"><span data-stu-id="08e6d-163">JSON</span></span>

<span data-ttu-id="08e6d-164">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08e6d-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="08e6d-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08e6d-165">Request</span></span>

<span data-ttu-id="08e6d-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08e6d-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="08e6d-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="08e6d-167">Response</span></span>

<span data-ttu-id="08e6d-168">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="08e6d-168">The following is an example of the response.</span></span>

> <span data-ttu-id="08e6d-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="08e6d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 93, 
      "synced": 26, 
      "sharedInternally": 6, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
