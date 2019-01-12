---
title: 'reportRoot: getOffice365ActivationCounts'
description: Erfahren Sie, wie viele Office 365-Aktivierungen auf Desktops und Geräten durchgeführt wurden.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8027cf24c5a79f6d129f9b266cdb80929f2d707a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913758"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="33b99-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="33b99-103">reportRoot: getOffice365ActivationCounts</span></span>

> <span data-ttu-id="33b99-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="33b99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33b99-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33b99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33b99-106">Erfahren Sie, wie viele Office 365-Aktivierungen auf Desktops und Geräten durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="33b99-106">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="33b99-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="33b99-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="33b99-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="33b99-108">Permissions</span></span>

<span data-ttu-id="33b99-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33b99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33b99-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33b99-111">Permission type</span></span>                        | <span data-ttu-id="33b99-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33b99-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="33b99-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33b99-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="33b99-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="33b99-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="33b99-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33b99-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33b99-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33b99-116">Not supported.</span></span>                           |
| <span data-ttu-id="33b99-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33b99-117">Application</span></span>                            | <span data-ttu-id="33b99-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="33b99-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="33b99-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33b99-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="33b99-120">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="33b99-120">Query parameters</span></span>

<span data-ttu-id="33b99-121">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="33b99-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="33b99-122">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="33b99-122">The default output type is text/csv.</span></span> <span data-ttu-id="33b99-123">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="33b99-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33b99-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33b99-124">Request headers</span></span>

| <span data-ttu-id="33b99-125">Name</span><span class="sxs-lookup"><span data-stu-id="33b99-125">Name</span></span>          | <span data-ttu-id="33b99-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33b99-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="33b99-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="33b99-127">Authorization</span></span> | <span data-ttu-id="33b99-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="33b99-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="33b99-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="33b99-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="33b99-131">CSV</span><span class="sxs-lookup"><span data-stu-id="33b99-131">CSV</span></span>

<span data-ttu-id="33b99-132">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="33b99-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="33b99-133">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="33b99-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="33b99-134">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="33b99-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="33b99-135">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="33b99-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="33b99-136">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="33b99-136">Report Refresh Date</span></span>
- <span data-ttu-id="33b99-137">Produkttyp</span><span class="sxs-lookup"><span data-stu-id="33b99-137">Product Type</span></span>
- <span data-ttu-id="33b99-138">Windows</span><span class="sxs-lookup"><span data-stu-id="33b99-138">Windows</span></span>
- <span data-ttu-id="33b99-139">Mac</span><span class="sxs-lookup"><span data-stu-id="33b99-139">Mac</span></span>
- <span data-ttu-id="33b99-140">Android</span><span class="sxs-lookup"><span data-stu-id="33b99-140">Android</span></span>
- <span data-ttu-id="33b99-141">iOS</span><span class="sxs-lookup"><span data-stu-id="33b99-141">iOS</span></span>
- <span data-ttu-id="33b99-142">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="33b99-142">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="33b99-143">JSON</span><span class="sxs-lookup"><span data-stu-id="33b99-143">JSON</span></span>

<span data-ttu-id="33b99-144">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ActivationCounts](../resources/office365activationcounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="33b99-144">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33b99-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33b99-145">Example</span></span>

### <a name="csv"></a><span data-ttu-id="33b99-146">CSV</span><span class="sxs-lookup"><span data-stu-id="33b99-146">CSV</span></span>

<span data-ttu-id="33b99-147">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="33b99-147">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="33b99-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33b99-148">Request</span></span>

<span data-ttu-id="33b99-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33b99-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="33b99-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="33b99-150">Response</span></span>

<span data-ttu-id="33b99-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="33b99-151">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="33b99-152">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="33b99-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="33b99-153">JSON</span><span class="sxs-lookup"><span data-stu-id="33b99-153">JSON</span></span>

<span data-ttu-id="33b99-154">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33b99-154">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="33b99-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33b99-155">Request</span></span>

<span data-ttu-id="33b99-156">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="33b99-156">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="33b99-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="33b99-157">Response</span></span>

<span data-ttu-id="33b99-158">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="33b99-158">The following example shows the response.</span></span>

> <span data-ttu-id="33b99-p106">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="33b99-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
