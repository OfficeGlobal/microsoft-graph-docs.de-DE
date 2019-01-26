---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Erhalten Sie detaillierte Informationen über Benutzer, die Office 365 aktiviert haben.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3e5e6841e0c8f37cf9a054bcd5d7276e3b1fd04b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571394"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="88d27-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="88d27-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="88d27-104">Erhalten Sie detaillierte Informationen über Benutzer, die Office 365 aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="88d27-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="88d27-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="88d27-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="88d27-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="88d27-106">Permissions</span></span>

<span data-ttu-id="88d27-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88d27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="88d27-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="88d27-109">Permission type</span></span>                        | <span data-ttu-id="88d27-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="88d27-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="88d27-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="88d27-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="88d27-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="88d27-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="88d27-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="88d27-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88d27-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88d27-114">Not supported.</span></span>                           |
| <span data-ttu-id="88d27-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="88d27-115">Application</span></span>                            | <span data-ttu-id="88d27-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="88d27-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="88d27-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="88d27-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="88d27-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="88d27-118">Request headers</span></span>

| <span data-ttu-id="88d27-119">Name</span><span class="sxs-lookup"><span data-stu-id="88d27-119">Name</span></span>          | <span data-ttu-id="88d27-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88d27-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="88d27-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="88d27-121">Authorization</span></span> | <span data-ttu-id="88d27-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="88d27-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="88d27-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="88d27-124">If-None-Match</span></span> | <span data-ttu-id="88d27-125">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="88d27-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="88d27-126">Optional.</span><span class="sxs-lookup"><span data-stu-id="88d27-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="88d27-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="88d27-127">Response</span></span>

<span data-ttu-id="88d27-128">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="88d27-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="88d27-129">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="88d27-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="88d27-130">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="88d27-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="88d27-131">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="88d27-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="88d27-132">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="88d27-132">Report Refresh Date</span></span>
- <span data-ttu-id="88d27-133">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="88d27-133">User Principal Name</span></span>
- <span data-ttu-id="88d27-134">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="88d27-134">Display Name</span></span>
- <span data-ttu-id="88d27-135">Produkttyp</span><span class="sxs-lookup"><span data-stu-id="88d27-135">Product Type</span></span>
- <span data-ttu-id="88d27-136">Datum der letzten Aktivierung</span><span class="sxs-lookup"><span data-stu-id="88d27-136">Last Activated Date</span></span>
- <span data-ttu-id="88d27-137">Windows</span><span class="sxs-lookup"><span data-stu-id="88d27-137">Windows</span></span>
- <span data-ttu-id="88d27-138">Mac</span><span class="sxs-lookup"><span data-stu-id="88d27-138">Mac</span></span>
- <span data-ttu-id="88d27-139">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="88d27-139">Windows 10 Mobile</span></span>
- <span data-ttu-id="88d27-140">iOS</span><span class="sxs-lookup"><span data-stu-id="88d27-140">iOS</span></span>
- <span data-ttu-id="88d27-141">Android</span><span class="sxs-lookup"><span data-stu-id="88d27-141">Android</span></span>
- <span data-ttu-id="88d27-142">Gemeinsam genutzter Computer aktiviert</span><span class="sxs-lookup"><span data-stu-id="88d27-142">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="88d27-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="88d27-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="88d27-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="88d27-144">Request</span></span>

<span data-ttu-id="88d27-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="88d27-145">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="88d27-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="88d27-146">Response</span></span>

<span data-ttu-id="88d27-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="88d27-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="88d27-148">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="88d27-148">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```
