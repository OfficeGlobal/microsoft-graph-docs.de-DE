---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Erhalten Sie detaillierte Informationen über Benutzer, die Office 365 aktiviert haben.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: c2cea0affc6cbbc67acbe38271bd9c0ac0fbb742
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529026"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="8b2e1-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="8b2e1-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b2e1-104">Erhalten Sie detaillierte Informationen über Benutzer, die Office 365 aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="8b2e1-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="8b2e1-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="8b2e1-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8b2e1-106">Permissions</span></span>

<span data-ttu-id="8b2e1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b2e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b2e1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b2e1-109">Permission type</span></span>                        | <span data-ttu-id="8b2e1-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b2e1-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8b2e1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b2e1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b2e1-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b2e1-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8b2e1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b2e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b2e1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b2e1-114">Not supported.</span></span>                           |
| <span data-ttu-id="8b2e1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b2e1-115">Application</span></span>                            | <span data-ttu-id="8b2e1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b2e1-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8b2e1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b2e1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="8b2e1-118">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8b2e1-118">Query parameters</span></span>

<span data-ttu-id="8b2e1-119">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-119">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8b2e1-120">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-120">The default output type is text/csv.</span></span> <span data-ttu-id="8b2e1-121">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b2e1-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b2e1-122">Request headers</span></span>

| <span data-ttu-id="8b2e1-123">Name</span><span class="sxs-lookup"><span data-stu-id="8b2e1-123">Name</span></span>          | <span data-ttu-id="8b2e1-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b2e1-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8b2e1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b2e1-125">Authorization</span></span> | <span data-ttu-id="8b2e1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8b2e1-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b2e1-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8b2e1-129">CSV</span><span class="sxs-lookup"><span data-stu-id="8b2e1-129">CSV</span></span>

<span data-ttu-id="8b2e1-130">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8b2e1-131">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8b2e1-132">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8b2e1-133">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8b2e1-134">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="8b2e1-134">Report Refresh Date</span></span>
- <span data-ttu-id="8b2e1-135">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="8b2e1-135">User Principal Name</span></span>
- <span data-ttu-id="8b2e1-136">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="8b2e1-136">Display Name</span></span>
- <span data-ttu-id="8b2e1-137">Produkttyp</span><span class="sxs-lookup"><span data-stu-id="8b2e1-137">Product Type</span></span>
- <span data-ttu-id="8b2e1-138">Datum der letzten Aktivierung</span><span class="sxs-lookup"><span data-stu-id="8b2e1-138">Last Activated Date</span></span>
- <span data-ttu-id="8b2e1-139">Windows</span><span class="sxs-lookup"><span data-stu-id="8b2e1-139">Windows</span></span>
- <span data-ttu-id="8b2e1-140">Mac</span><span class="sxs-lookup"><span data-stu-id="8b2e1-140">Mac</span></span>
- <span data-ttu-id="8b2e1-141">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="8b2e1-141">Windows 10 Mobile</span></span>
- <span data-ttu-id="8b2e1-142">iOS</span><span class="sxs-lookup"><span data-stu-id="8b2e1-142">iOS</span></span>
- <span data-ttu-id="8b2e1-143">Android</span><span class="sxs-lookup"><span data-stu-id="8b2e1-143">Android</span></span>
- <span data-ttu-id="8b2e1-144">Gemeinsam genutzter Computer aktiviert</span><span class="sxs-lookup"><span data-stu-id="8b2e1-144">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="8b2e1-145">JSON</span><span class="sxs-lookup"><span data-stu-id="8b2e1-145">JSON</span></span>

<span data-ttu-id="8b2e1-146">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-146">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="8b2e1-147">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-147">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="8b2e1-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b2e1-148">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8b2e1-149">CSV</span><span class="sxs-lookup"><span data-stu-id="8b2e1-149">CSV</span></span>

<span data-ttu-id="8b2e1-150">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-150">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8b2e1-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b2e1-151">Request</span></span>

<span data-ttu-id="8b2e1-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8b2e1-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b2e1-153">Response</span></span>

<span data-ttu-id="8b2e1-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8b2e1-155">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```

### <a name="json"></a><span data-ttu-id="8b2e1-156">JSON</span><span class="sxs-lookup"><span data-stu-id="8b2e1-156">JSON</span></span>

<span data-ttu-id="8b2e1-157">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-157">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8b2e1-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b2e1-158">Request</span></span>

<span data-ttu-id="8b2e1-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8b2e1-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b2e1-160">Response</span></span>

<span data-ttu-id="8b2e1-161">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-161">The following is an example of the response.</span></span>

> <span data-ttu-id="8b2e1-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8b2e1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "userActivationCounts": [
        {
          "productType": "Project Client", 
          "lastActivatedDate": "2017-08-20", 
          "windows": 5, 
          "mac": 0, 
          "windows10Mobile": 0, 
          "ios": 0, 
          "android": 2,
          "activatedOnSharedComputer": true
        }
      ]
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activationsuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
