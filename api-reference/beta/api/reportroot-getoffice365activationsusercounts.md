---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Rufen Sie die Anzahl von Benutzern, die aktiviert sind und die aktiviert das Office-Abonnement auf Desktop- oder Geräte oder Computer freigegeben haben.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a67f54b0c2abc1ef201782525492bed3bab98983
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526893"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="5d667-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="5d667-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d667-104">Rufen Sie die Anzahl von Benutzern, die aktiviert sind und die aktiviert das Office-Abonnement auf Desktop- oder Geräte oder Computer freigegeben haben.</span><span class="sxs-lookup"><span data-stu-id="5d667-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="5d667-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="5d667-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d667-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5d667-106">Permissions</span></span>

<span data-ttu-id="5d667-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d667-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d667-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d667-109">Permission type</span></span>                        | <span data-ttu-id="5d667-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d667-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5d667-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d667-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d667-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d667-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5d667-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d667-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d667-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d667-114">Not supported.</span></span>                           |
| <span data-ttu-id="5d667-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d667-115">Application</span></span>                            | <span data-ttu-id="5d667-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d667-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5d667-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d667-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="query-parameters"></a><span data-ttu-id="5d667-118">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5d667-118">Query parameters</span></span>

<span data-ttu-id="5d667-119">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d667-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5d667-120">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="5d667-120">The default output type is text/csv.</span></span> <span data-ttu-id="5d667-121">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="5d667-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d667-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d667-122">Request headers</span></span>

| <span data-ttu-id="5d667-123">Name</span><span class="sxs-lookup"><span data-stu-id="5d667-123">Name</span></span>          | <span data-ttu-id="5d667-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d667-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5d667-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d667-125">Authorization</span></span> | <span data-ttu-id="5d667-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5d667-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5d667-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d667-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5d667-129">CSV</span><span class="sxs-lookup"><span data-stu-id="5d667-129">CSV</span></span>

<span data-ttu-id="5d667-130">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="5d667-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5d667-131">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d667-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5d667-132">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="5d667-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5d667-133">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="5d667-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5d667-134">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="5d667-134">Report Refresh Date</span></span>
- <span data-ttu-id="5d667-135">Produkttyp</span><span class="sxs-lookup"><span data-stu-id="5d667-135">Product Type</span></span>
- <span data-ttu-id="5d667-136">Zugewiesen</span><span class="sxs-lookup"><span data-stu-id="5d667-136">Assigned</span></span>
- <span data-ttu-id="5d667-137">Aktiviert</span><span class="sxs-lookup"><span data-stu-id="5d667-137">Activated</span></span>
- <span data-ttu-id="5d667-138">Gemeinsam genutzter Computer-Aktivierung</span><span class="sxs-lookup"><span data-stu-id="5d667-138">Shared Computer Activation</span></span>

### <a name="json"></a><span data-ttu-id="5d667-139">JSON</span><span class="sxs-lookup"><span data-stu-id="5d667-139">JSON</span></span>

<span data-ttu-id="5d667-140">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5d667-140">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d667-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d667-141">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5d667-142">CSV</span><span class="sxs-lookup"><span data-stu-id="5d667-142">CSV</span></span>

<span data-ttu-id="5d667-143">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="5d667-143">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5d667-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d667-144">Request</span></span>

<span data-ttu-id="5d667-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d667-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="5d667-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d667-146">Response</span></span>

<span data-ttu-id="5d667-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d667-147">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5d667-148">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="5d667-148">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```

### <a name="json"></a><span data-ttu-id="5d667-149">JSON</span><span class="sxs-lookup"><span data-stu-id="5d667-149">JSON</span></span>

<span data-ttu-id="5d667-150">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d667-150">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5d667-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d667-151">Request</span></span>

<span data-ttu-id="5d667-152">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d667-152">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="5d667-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d667-153">Response</span></span>

<span data-ttu-id="5d667-154">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d667-154">The following example shows the response.</span></span>

> <span data-ttu-id="5d667-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5d667-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "assigned": 2679, 
      "activated": 1710,
      "sharedComputerActivation": 1024
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activationsusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
