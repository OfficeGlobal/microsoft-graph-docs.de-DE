---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Rufen Sie die Anzahl der eindeutigen Benutzer der Desktopversion von Outlook ab.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b8e52b5a5256e307f721c575bebc7932daf800f3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575821"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="09f44-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="09f44-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09f44-104">Rufen Sie die Anzahl der eindeutigen Benutzer der Desktopversion von Outlook ab.</span><span class="sxs-lookup"><span data-stu-id="09f44-104">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="09f44-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Nutzung von E-Mail-Apps](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="09f44-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="09f44-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="09f44-106">Permissions</span></span>

<span data-ttu-id="09f44-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09f44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09f44-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09f44-109">Permission type</span></span>                        | <span data-ttu-id="09f44-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09f44-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="09f44-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09f44-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="09f44-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="09f44-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="09f44-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09f44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09f44-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09f44-114">Not supported.</span></span>                           |
| <span data-ttu-id="09f44-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09f44-115">Application</span></span>                            | <span data-ttu-id="09f44-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="09f44-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="09f44-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09f44-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="09f44-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="09f44-118">Function parameters</span></span>

<span data-ttu-id="09f44-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="09f44-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="09f44-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="09f44-120">Parameter</span></span> | <span data-ttu-id="09f44-121">Typ</span><span class="sxs-lookup"><span data-stu-id="09f44-121">Type</span></span>   | <span data-ttu-id="09f44-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09f44-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="09f44-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="09f44-123">period</span></span>    | <span data-ttu-id="09f44-124">string</span><span class="sxs-lookup"><span data-stu-id="09f44-124">string</span></span> | <span data-ttu-id="09f44-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="09f44-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="09f44-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="09f44-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="09f44-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="09f44-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="09f44-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="09f44-128">Required.</span></span> |

<span data-ttu-id="09f44-129">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="09f44-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="09f44-130">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="09f44-130">The default output type is text/csv.</span></span> <span data-ttu-id="09f44-131">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="09f44-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09f44-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09f44-132">Request headers</span></span>

| <span data-ttu-id="09f44-133">Name</span><span class="sxs-lookup"><span data-stu-id="09f44-133">Name</span></span>          | <span data-ttu-id="09f44-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09f44-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="09f44-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="09f44-135">Authorization</span></span> | <span data-ttu-id="09f44-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="09f44-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="09f44-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="09f44-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="09f44-139">CSV</span><span class="sxs-lookup"><span data-stu-id="09f44-139">CSV</span></span>

<span data-ttu-id="09f44-140">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="09f44-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="09f44-141">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="09f44-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="09f44-142">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="09f44-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="09f44-143">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="09f44-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="09f44-144">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="09f44-144">Report Refresh Date</span></span>
- <span data-ttu-id="09f44-145">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="09f44-145">Outlook 2016</span></span>
- <span data-ttu-id="09f44-146">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="09f44-146">Outlook 2013</span></span>
- <span data-ttu-id="09f44-147">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="09f44-147">Outlook 2010</span></span>
- <span data-ttu-id="09f44-148">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="09f44-148">Outlook 2007</span></span>
- <span data-ttu-id="09f44-149">Unbestimmt</span><span class="sxs-lookup"><span data-stu-id="09f44-149">Undetermined</span></span>
- <span data-ttu-id="09f44-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="09f44-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="09f44-151">JSON</span><span class="sxs-lookup"><span data-stu-id="09f44-151">JSON</span></span>

<span data-ttu-id="09f44-152">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[EmailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="09f44-152">If successful, this method returns a `200 OK` response code and an **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09f44-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09f44-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="09f44-154">CSV</span><span class="sxs-lookup"><span data-stu-id="09f44-154">CSV</span></span>

<span data-ttu-id="09f44-155">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="09f44-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="09f44-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09f44-156">Request</span></span>

<span data-ttu-id="09f44-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09f44-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="09f44-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="09f44-158">Response</span></span>

<span data-ttu-id="09f44-159">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="09f44-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="09f44-160">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="09f44-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
```

### <a name="json"></a><span data-ttu-id="09f44-161">JSON</span><span class="sxs-lookup"><span data-stu-id="09f44-161">JSON</span></span>

<span data-ttu-id="09f44-162">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09f44-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="09f44-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09f44-163">Request</span></span>

<span data-ttu-id="09f44-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09f44-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="09f44-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="09f44-165">Response</span></span>

<span data-ttu-id="09f44-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="09f44-166">The following is an example of the response.</span></span>

> <span data-ttu-id="09f44-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="09f44-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageVersionsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "outlook2016": 1554, 
      "outlook2013": 64, 
      "outlook2010": 1, 
      "outlook2007": 0, 
      "undetermined": 1259, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getemailappusageversionsusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
