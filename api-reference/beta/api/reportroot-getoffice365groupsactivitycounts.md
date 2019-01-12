---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Rufen Sie die Anzahl der Gruppenaktivitäten für Gruppenarbeitslasten ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 39e434066dad74998c379dc3d1bc54276fd4c8ea
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966300"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="2d4f4-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="2d4f4-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

> <span data-ttu-id="2d4f4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d4f4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d4f4-106">Rufen Sie die Anzahl der Gruppenaktivitäten für Gruppenarbeitslasten ab.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-106">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="2d4f4-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="2d4f4-107">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="2d4f4-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2d4f4-108">Permissions</span></span>

<span data-ttu-id="2d4f4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d4f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d4f4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d4f4-111">Permission type</span></span>                        | <span data-ttu-id="2d4f4-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d4f4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2d4f4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d4f4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d4f4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d4f4-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2d4f4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d4f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d4f4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d4f4-116">Not supported.</span></span>                           |
| <span data-ttu-id="2d4f4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d4f4-117">Application</span></span>                            | <span data-ttu-id="2d4f4-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d4f4-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2d4f4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d4f4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2d4f4-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="2d4f4-120">Function parameters</span></span>

<span data-ttu-id="2d4f4-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2d4f4-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="2d4f4-122">Parameter</span></span> | <span data-ttu-id="2d4f4-123">Typ</span><span class="sxs-lookup"><span data-stu-id="2d4f4-123">Type</span></span>   | <span data-ttu-id="2d4f4-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d4f4-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2d4f4-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="2d4f4-125">period</span></span>    | <span data-ttu-id="2d4f4-126">string</span><span class="sxs-lookup"><span data-stu-id="2d4f4-126">string</span></span> | <span data-ttu-id="2d4f4-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2d4f4-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2d4f4-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2d4f4-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2d4f4-130">Required.</span></span> |

<span data-ttu-id="2d4f4-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2d4f4-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-132">The default output type is text/csv.</span></span> <span data-ttu-id="2d4f4-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d4f4-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d4f4-134">Request headers</span></span>

| <span data-ttu-id="2d4f4-135">Name</span><span class="sxs-lookup"><span data-stu-id="2d4f4-135">Name</span></span>          | <span data-ttu-id="2d4f4-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d4f4-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2d4f4-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d4f4-137">Authorization</span></span> | <span data-ttu-id="2d4f4-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2d4f4-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d4f4-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2d4f4-141">CSV</span><span class="sxs-lookup"><span data-stu-id="2d4f4-141">CSV</span></span>

<span data-ttu-id="2d4f4-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2d4f4-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2d4f4-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2d4f4-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2d4f4-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="2d4f4-146">Report Refresh Date</span></span>
- <span data-ttu-id="2d4f4-147">Empfangene Exchange-E-Mails</span><span class="sxs-lookup"><span data-stu-id="2d4f4-147">Exchange Emails Received</span></span>
- <span data-ttu-id="2d4f4-148">Veröffentlichte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="2d4f4-148">Yammer Messages Posted</span></span>
- <span data-ttu-id="2d4f4-149">Gelesene Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="2d4f4-149">Yammer Messages Read</span></span>
- <span data-ttu-id="2d4f4-150">Gelikte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="2d4f4-150">Yammer Messages Liked</span></span>
- <span data-ttu-id="2d4f4-151">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="2d4f4-151">Report Date</span></span>
- <span data-ttu-id="2d4f4-152">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="2d4f4-152">Report Period</span></span>

<span data-ttu-id="2d4f4-153">Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="2d4f4-153">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="2d4f4-154">Veröffentlichte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="2d4f4-154">Yammer Messages Posted</span></span>
- <span data-ttu-id="2d4f4-155">Gelesene Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="2d4f4-155">Yammer Messages Read</span></span>
- <span data-ttu-id="2d4f4-156">Gelikte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="2d4f4-156">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="2d4f4-157">JSON</span><span class="sxs-lookup"><span data-stu-id="2d4f4-157">JSON</span></span>

<span data-ttu-id="2d4f4-158">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-158">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="2d4f4-159">Die folgenden Eigenschaften im **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="2d4f4-159">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="2d4f4-160">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="2d4f4-160">yammerMessagesPosted</span></span>
- <span data-ttu-id="2d4f4-161">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="2d4f4-161">yammerMessagesRead</span></span>
- <span data-ttu-id="2d4f4-162">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="2d4f4-162">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="2d4f4-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d4f4-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2d4f4-164">CSV</span><span class="sxs-lookup"><span data-stu-id="2d4f4-164">CSV</span></span>

<span data-ttu-id="2d4f4-165">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2d4f4-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d4f4-166">Request</span></span>

<span data-ttu-id="2d4f4-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="2d4f4-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d4f4-168">Response</span></span>

<span data-ttu-id="2d4f4-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2d4f4-170">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="2d4f4-171">JSON</span><span class="sxs-lookup"><span data-stu-id="2d4f4-171">JSON</span></span>

<span data-ttu-id="2d4f4-172">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2d4f4-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d4f4-173">Request</span></span>

<span data-ttu-id="2d4f4-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="2d4f4-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d4f4-175">Response</span></span>

<span data-ttu-id="2d4f4-176">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-176">The following is an example of the response.</span></span>

> <span data-ttu-id="2d4f4-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2d4f4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
