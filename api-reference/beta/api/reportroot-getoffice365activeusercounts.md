---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Rufen Sie die Anzahl der im Berichtszeitraum täglich aktiven Benutzer nach Produkt ab.
localization_priority: Normal
ms.openlocfilehash: 0213ee12ec73fc43a0a321fa77d4c0d2495e4210
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844485"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="126e1-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="126e1-103">reportRoot: getOffice365ActiveUserCounts</span></span>

> <span data-ttu-id="126e1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="126e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="126e1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="126e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="126e1-106">Rufen Sie die Anzahl der im Berichtszeitraum täglich aktiven Benutzer nach Produkt ab.</span><span class="sxs-lookup"><span data-stu-id="126e1-106">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="126e1-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="126e1-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="126e1-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="126e1-108">Permissions</span></span>

<span data-ttu-id="126e1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="126e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="126e1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="126e1-111">Permission type</span></span>                        | <span data-ttu-id="126e1-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="126e1-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="126e1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="126e1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="126e1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="126e1-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="126e1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="126e1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="126e1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="126e1-116">Not supported.</span></span>                           |
| <span data-ttu-id="126e1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="126e1-117">Application</span></span>                            | <span data-ttu-id="126e1-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="126e1-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="126e1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="126e1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="126e1-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="126e1-120">Function parameters</span></span>

<span data-ttu-id="126e1-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="126e1-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="126e1-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="126e1-122">Parameter</span></span> | <span data-ttu-id="126e1-123">Typ</span><span class="sxs-lookup"><span data-stu-id="126e1-123">Type</span></span>   | <span data-ttu-id="126e1-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="126e1-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="126e1-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="126e1-125">period</span></span>    | <span data-ttu-id="126e1-126">string</span><span class="sxs-lookup"><span data-stu-id="126e1-126">string</span></span> | <span data-ttu-id="126e1-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="126e1-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="126e1-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="126e1-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="126e1-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="126e1-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="126e1-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="126e1-130">Required.</span></span> |

<span data-ttu-id="126e1-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="126e1-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="126e1-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="126e1-132">The default output type is text/csv.</span></span> <span data-ttu-id="126e1-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="126e1-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="126e1-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="126e1-134">Request headers</span></span>

| <span data-ttu-id="126e1-135">Name</span><span class="sxs-lookup"><span data-stu-id="126e1-135">Name</span></span>          | <span data-ttu-id="126e1-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="126e1-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="126e1-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="126e1-137">Authorization</span></span> | <span data-ttu-id="126e1-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="126e1-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="126e1-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="126e1-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="126e1-141">CSV</span><span class="sxs-lookup"><span data-stu-id="126e1-141">CSV</span></span>

<span data-ttu-id="126e1-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="126e1-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="126e1-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="126e1-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="126e1-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="126e1-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="126e1-145">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="126e1-145">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="126e1-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="126e1-146">Report Refresh Date</span></span>
- <span data-ttu-id="126e1-147">Office 365</span><span class="sxs-lookup"><span data-stu-id="126e1-147">Office 365</span></span>
- <span data-ttu-id="126e1-148">Exchange</span><span class="sxs-lookup"><span data-stu-id="126e1-148">Exchange</span></span>
- <span data-ttu-id="126e1-149">OneDrive</span><span class="sxs-lookup"><span data-stu-id="126e1-149">OneDrive</span></span>
- <span data-ttu-id="126e1-150">SharePoint</span><span class="sxs-lookup"><span data-stu-id="126e1-150">SharePoint</span></span>
- <span data-ttu-id="126e1-151">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="126e1-151">Skype For Business</span></span> 
- <span data-ttu-id="126e1-152">Yammer</span><span class="sxs-lookup"><span data-stu-id="126e1-152">Yammer</span></span>
- <span data-ttu-id="126e1-153">Teams</span><span class="sxs-lookup"><span data-stu-id="126e1-153">Teams</span></span>
- <span data-ttu-id="126e1-154">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="126e1-154">Report Date</span></span>
- <span data-ttu-id="126e1-155">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="126e1-155">Report Period</span></span>

<span data-ttu-id="126e1-156">Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="126e1-156">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="126e1-157">Yammer</span><span class="sxs-lookup"><span data-stu-id="126e1-157">Yammer</span></span>
- <span data-ttu-id="126e1-158">Teams</span><span class="sxs-lookup"><span data-stu-id="126e1-158">Teams</span></span>

### <a name="json"></a><span data-ttu-id="126e1-159">JSON</span><span class="sxs-lookup"><span data-stu-id="126e1-159">JSON</span></span>

<span data-ttu-id="126e1-160">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="126e1-160">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="126e1-161">Die folgenden Eigenschaften im **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="126e1-161">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="126e1-162">Yammer</span><span class="sxs-lookup"><span data-stu-id="126e1-162">yammer</span></span>
- <span data-ttu-id="126e1-163">Teams</span><span class="sxs-lookup"><span data-stu-id="126e1-163">teams</span></span>

## <a name="example"></a><span data-ttu-id="126e1-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="126e1-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="126e1-165">CSV</span><span class="sxs-lookup"><span data-stu-id="126e1-165">CSV</span></span>

<span data-ttu-id="126e1-166">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="126e1-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="126e1-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="126e1-167">Request</span></span>

<span data-ttu-id="126e1-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="126e1-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="126e1-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="126e1-169">Response</span></span>

<span data-ttu-id="126e1-170">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="126e1-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="126e1-171">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="126e1-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="126e1-172">JSON</span><span class="sxs-lookup"><span data-stu-id="126e1-172">JSON</span></span>

<span data-ttu-id="126e1-173">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="126e1-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="126e1-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="126e1-174">Request</span></span>

<span data-ttu-id="126e1-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="126e1-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="126e1-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="126e1-176">Response</span></span>

<span data-ttu-id="126e1-177">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="126e1-177">The following is an example of the response.</span></span>

> <span data-ttu-id="126e1-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="126e1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
      "reportPeriod": "7"
    }
  ]
}
```
