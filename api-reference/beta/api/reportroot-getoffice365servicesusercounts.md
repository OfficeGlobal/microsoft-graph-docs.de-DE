---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab.
ms.openlocfilehash: 9f331852c5ba47643e11ea6cfa86167669557aae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060697"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="1434d-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="1434d-103">reportRoot: getOffice365ServicesUserCounts</span></span>

> <span data-ttu-id="1434d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1434d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1434d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1434d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1434d-106">Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab.</span><span class="sxs-lookup"><span data-stu-id="1434d-106">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="1434d-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="1434d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="1434d-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1434d-108">Permissions</span></span>

<span data-ttu-id="1434d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1434d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1434d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1434d-111">Permission type</span></span>                        | <span data-ttu-id="1434d-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1434d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1434d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1434d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1434d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1434d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1434d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1434d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1434d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1434d-116">Not supported.</span></span>                           |
| <span data-ttu-id="1434d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1434d-117">Application</span></span>                            | <span data-ttu-id="1434d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1434d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1434d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1434d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1434d-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="1434d-120">Function parameters</span></span>

<span data-ttu-id="1434d-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="1434d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1434d-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="1434d-122">Parameter</span></span> | <span data-ttu-id="1434d-123">Typ</span><span class="sxs-lookup"><span data-stu-id="1434d-123">Type</span></span>   | <span data-ttu-id="1434d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1434d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1434d-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="1434d-125">period</span></span>    | <span data-ttu-id="1434d-126">string</span><span class="sxs-lookup"><span data-stu-id="1434d-126">string</span></span> | <span data-ttu-id="1434d-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="1434d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1434d-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="1434d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1434d-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="1434d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1434d-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="1434d-130">Required.</span></span> |

<span data-ttu-id="1434d-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1434d-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1434d-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="1434d-132">The default output type is text/csv.</span></span> <span data-ttu-id="1434d-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="1434d-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1434d-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1434d-134">Request headers</span></span>

| <span data-ttu-id="1434d-135">Name</span><span class="sxs-lookup"><span data-stu-id="1434d-135">Name</span></span>          | <span data-ttu-id="1434d-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1434d-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1434d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="1434d-137">Authorization</span></span> | <span data-ttu-id="1434d-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1434d-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1434d-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1434d-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1434d-141">CSV</span><span class="sxs-lookup"><span data-stu-id="1434d-141">CSV</span></span>

<span data-ttu-id="1434d-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="1434d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1434d-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1434d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1434d-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="1434d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1434d-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="1434d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1434d-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="1434d-146">Report Refresh Date</span></span>
- <span data-ttu-id="1434d-147">Exchange aktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-147">Exchange Active</span></span>
- <span data-ttu-id="1434d-148">Exchange inaktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-148">Exchange Inactive</span></span>
- <span data-ttu-id="1434d-149">OneDrive aktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-149">OneDrive Active</span></span>
- <span data-ttu-id="1434d-150">OneDrive inaktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-150">OneDrive Inactive</span></span>
- <span data-ttu-id="1434d-151">SharePoint aktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-151">SharePoint Active</span></span>
- <span data-ttu-id="1434d-152">SharePoint inaktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-152">SharePoint Inactive</span></span>
- <span data-ttu-id="1434d-153">Skype for Business aktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-153">Skype For Business Active</span></span>
- <span data-ttu-id="1434d-154">Skype for Business inaktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-154">Skype For Business Inactive</span></span>
- <span data-ttu-id="1434d-155">Yammer aktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-155">Yammer Active</span></span>
- <span data-ttu-id="1434d-156">Yammer inaktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-156">Yammer Inactive</span></span>
- <span data-ttu-id="1434d-157">Teams aktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-157">Teams Active</span></span>
- <span data-ttu-id="1434d-158">Teams inaktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-158">Teams Inactive</span></span>
- <span data-ttu-id="1434d-159">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="1434d-159">Report Period</span></span>

<span data-ttu-id="1434d-160">Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="1434d-160">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="1434d-161">Yammer aktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-161">Yammer Active</span></span>
- <span data-ttu-id="1434d-162">Yammer inaktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-162">Yammer Inactive</span></span>
- <span data-ttu-id="1434d-163">Teams aktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-163">Teams Active</span></span>
- <span data-ttu-id="1434d-164">Teams inaktiv</span><span class="sxs-lookup"><span data-stu-id="1434d-164">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="1434d-165">JSON</span><span class="sxs-lookup"><span data-stu-id="1434d-165">JSON</span></span>

<span data-ttu-id="1434d-166">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1434d-166">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="1434d-167">Die folgenden Eigenschaften im **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="1434d-167">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="1434d-168">yammerActive</span><span class="sxs-lookup"><span data-stu-id="1434d-168">yammerActive</span></span>
- <span data-ttu-id="1434d-169">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="1434d-169">yammerInactive</span></span>
- <span data-ttu-id="1434d-170">teamsActive</span><span class="sxs-lookup"><span data-stu-id="1434d-170">teamsActive</span></span>
- <span data-ttu-id="1434d-171">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="1434d-171">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="1434d-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1434d-172">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1434d-173">CSV</span><span class="sxs-lookup"><span data-stu-id="1434d-173">CSV</span></span>

<span data-ttu-id="1434d-174">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="1434d-174">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1434d-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1434d-175">Request</span></span>

<span data-ttu-id="1434d-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1434d-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1434d-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="1434d-177">Response</span></span>

<span data-ttu-id="1434d-178">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1434d-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1434d-179">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="1434d-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```

### <a name="json"></a><span data-ttu-id="1434d-180">JSON</span><span class="sxs-lookup"><span data-stu-id="1434d-180">JSON</span></span> 

<span data-ttu-id="1434d-181">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1434d-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1434d-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1434d-182">Request</span></span>

<span data-ttu-id="1434d-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1434d-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1434d-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="1434d-184">Response</span></span>

<span data-ttu-id="1434d-185">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1434d-185">The following is an example of the response.</span></span>

> <span data-ttu-id="1434d-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1434d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 458

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ServicesUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeActive": 2591, 
      "exchangeInactive": 1426, 
      "oneDriveActive": 1800, 
      "oneDriveInactive": 2451, 
      "sharePointActive": 2286, 
      "sharePointInactive": 1815, 
      "skypeForBusinessActive": 2463, 
      "skypeForBusinessInactive": 1947, 
      "yammerActive": 473, 
      "yammerInactive": 2526, 
      "teamsActive": 846, 
      "teamsInactive": 1960, 
      "reportPeriod": "7"
    }
  ]
}
```
