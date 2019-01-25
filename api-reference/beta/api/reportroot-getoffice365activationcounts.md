---
title: 'reportRoot: getOffice365ActivationCounts'
description: Erfahren Sie, wie viele Office 365-Aktivierungen auf Desktops und Geräten durchgeführt wurden.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 88ee061ba61f9a0be4c8faa35f966749bf65ae76
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509413"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="4a04d-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="4a04d-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a04d-104">Erfahren Sie, wie viele Office 365-Aktivierungen auf Desktops und Geräten durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="4a04d-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="4a04d-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="4a04d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a04d-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4a04d-106">Permissions</span></span>

<span data-ttu-id="4a04d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a04d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a04d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a04d-109">Permission type</span></span>                        | <span data-ttu-id="4a04d-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a04d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4a04d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a04d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a04d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a04d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4a04d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a04d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a04d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a04d-114">Not supported.</span></span>                           |
| <span data-ttu-id="4a04d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a04d-115">Application</span></span>                            | <span data-ttu-id="4a04d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a04d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4a04d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a04d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="4a04d-118">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4a04d-118">Query parameters</span></span>

<span data-ttu-id="4a04d-119">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4a04d-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4a04d-120">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="4a04d-120">The default output type is text/csv.</span></span> <span data-ttu-id="4a04d-121">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="4a04d-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a04d-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a04d-122">Request headers</span></span>

| <span data-ttu-id="4a04d-123">Name</span><span class="sxs-lookup"><span data-stu-id="4a04d-123">Name</span></span>          | <span data-ttu-id="4a04d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a04d-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4a04d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a04d-125">Authorization</span></span> | <span data-ttu-id="4a04d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4a04d-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4a04d-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a04d-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4a04d-129">CSV</span><span class="sxs-lookup"><span data-stu-id="4a04d-129">CSV</span></span>

<span data-ttu-id="4a04d-130">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="4a04d-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4a04d-131">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4a04d-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4a04d-132">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="4a04d-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4a04d-133">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="4a04d-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4a04d-134">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="4a04d-134">Report Refresh Date</span></span>
- <span data-ttu-id="4a04d-135">Produkttyp</span><span class="sxs-lookup"><span data-stu-id="4a04d-135">Product Type</span></span>
- <span data-ttu-id="4a04d-136">Windows</span><span class="sxs-lookup"><span data-stu-id="4a04d-136">Windows</span></span>
- <span data-ttu-id="4a04d-137">Mac</span><span class="sxs-lookup"><span data-stu-id="4a04d-137">Mac</span></span>
- <span data-ttu-id="4a04d-138">Android</span><span class="sxs-lookup"><span data-stu-id="4a04d-138">Android</span></span>
- <span data-ttu-id="4a04d-139">iOS</span><span class="sxs-lookup"><span data-stu-id="4a04d-139">iOS</span></span>
- <span data-ttu-id="4a04d-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="4a04d-140">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="4a04d-141">JSON</span><span class="sxs-lookup"><span data-stu-id="4a04d-141">JSON</span></span>

<span data-ttu-id="4a04d-142">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ActivationCounts](../resources/office365activationcounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4a04d-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a04d-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a04d-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4a04d-144">CSV</span><span class="sxs-lookup"><span data-stu-id="4a04d-144">CSV</span></span>

<span data-ttu-id="4a04d-145">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="4a04d-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4a04d-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a04d-146">Request</span></span>

<span data-ttu-id="4a04d-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a04d-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4a04d-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a04d-148">Response</span></span>

<span data-ttu-id="4a04d-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4a04d-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4a04d-150">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="4a04d-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```

### <a name="json"></a><span data-ttu-id="4a04d-151">JSON</span><span class="sxs-lookup"><span data-stu-id="4a04d-151">JSON</span></span>

<span data-ttu-id="4a04d-152">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a04d-152">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4a04d-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a04d-153">Request</span></span>

<span data-ttu-id="4a04d-154">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="4a04d-154">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4a04d-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a04d-155">Response</span></span>

<span data-ttu-id="4a04d-156">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="4a04d-156">The following example shows the response.</span></span>

> <span data-ttu-id="4a04d-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4a04d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
