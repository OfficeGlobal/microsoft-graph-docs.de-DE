---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Erhalten Sie detaillierte Informationen über Benutzer, die Office 365 aktiviert haben.
ms.openlocfilehash: 1dbbfefc7ea620f0926b037bd138bb04ed362c5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060409"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="b4b04-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="b4b04-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

> <span data-ttu-id="b4b04-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b4b04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4b04-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4b04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b4b04-106">Erhalten Sie detaillierte Informationen über Benutzer, die Office 365 aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="b4b04-106">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="b4b04-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="b4b04-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4b04-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b4b04-108">Permissions</span></span>

<span data-ttu-id="b4b04-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4b04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4b04-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4b04-111">Permission type</span></span>                        | <span data-ttu-id="b4b04-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4b04-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b4b04-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4b04-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4b04-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4b04-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b4b04-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4b04-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4b04-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4b04-116">Not supported.</span></span>                           |
| <span data-ttu-id="b4b04-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4b04-117">Application</span></span>                            | <span data-ttu-id="b4b04-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4b04-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b4b04-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4b04-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="b4b04-120">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b4b04-120">Query parameters</span></span>

<span data-ttu-id="b4b04-121">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4b04-121">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b4b04-122">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="b4b04-122">The default output type is text/csv.</span></span> <span data-ttu-id="b4b04-123">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="b4b04-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4b04-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4b04-124">Request headers</span></span>

| <span data-ttu-id="b4b04-125">Name</span><span class="sxs-lookup"><span data-stu-id="b4b04-125">Name</span></span>          | <span data-ttu-id="b4b04-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4b04-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b4b04-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4b04-127">Authorization</span></span> | <span data-ttu-id="b4b04-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b4b04-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b4b04-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4b04-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b4b04-131">CSV</span><span class="sxs-lookup"><span data-stu-id="b4b04-131">CSV</span></span>

<span data-ttu-id="b4b04-132">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="b4b04-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b4b04-133">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4b04-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b4b04-134">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="b4b04-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b4b04-135">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="b4b04-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b4b04-136">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="b4b04-136">Report Refresh Date</span></span>
- <span data-ttu-id="b4b04-137">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="b4b04-137">User Principal Name</span></span>
- <span data-ttu-id="b4b04-138">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="b4b04-138">Display Name</span></span>
- <span data-ttu-id="b4b04-139">Produkttyp</span><span class="sxs-lookup"><span data-stu-id="b4b04-139">Product Type</span></span>
- <span data-ttu-id="b4b04-140">Datum der letzten Aktivierung</span><span class="sxs-lookup"><span data-stu-id="b4b04-140">Last Activated Date</span></span>
- <span data-ttu-id="b4b04-141">Windows</span><span class="sxs-lookup"><span data-stu-id="b4b04-141">Windows</span></span>
- <span data-ttu-id="b4b04-142">Mac</span><span class="sxs-lookup"><span data-stu-id="b4b04-142">Mac</span></span>
- <span data-ttu-id="b4b04-143">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="b4b04-143">Windows 10 Mobile</span></span>
- <span data-ttu-id="b4b04-144">iOS</span><span class="sxs-lookup"><span data-stu-id="b4b04-144">iOS</span></span>
- <span data-ttu-id="b4b04-145">Android</span><span class="sxs-lookup"><span data-stu-id="b4b04-145">Android</span></span>
- <span data-ttu-id="b4b04-146">Gemeinsam genutzter Computer aktiviert</span><span class="sxs-lookup"><span data-stu-id="b4b04-146">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="b4b04-147">JSON</span><span class="sxs-lookup"><span data-stu-id="b4b04-147">JSON</span></span>

<span data-ttu-id="b4b04-148">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b4b04-148">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="b4b04-149">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="b4b04-149">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="b4b04-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4b04-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b4b04-151">CSV</span><span class="sxs-lookup"><span data-stu-id="b4b04-151">CSV</span></span>

<span data-ttu-id="b4b04-152">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="b4b04-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b4b04-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4b04-153">Request</span></span>

<span data-ttu-id="b4b04-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4b04-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b4b04-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4b04-155">Response</span></span>

<span data-ttu-id="b4b04-156">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4b04-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b4b04-157">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="b4b04-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="b4b04-158">JSON</span><span class="sxs-lookup"><span data-stu-id="b4b04-158">JSON</span></span>

<span data-ttu-id="b4b04-159">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4b04-159">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b4b04-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4b04-160">Request</span></span>

<span data-ttu-id="b4b04-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4b04-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b4b04-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4b04-162">Response</span></span>

<span data-ttu-id="b4b04-163">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4b04-163">The following is an example of the response.</span></span>

> <span data-ttu-id="b4b04-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b4b04-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
