---
title: 'reportRoot: getOffice365ActivationCounts'
description: Erfahren Sie, wie viele Office 365-Aktivierungen auf Desktops und Geräten durchgeführt wurden.
localization_priority: Normal
ms.openlocfilehash: a8447c0a8b98b9bf26bf7e8efd728a6ef120813d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890552"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="f90c4-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="f90c4-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="f90c4-104">Erfahren Sie, wie viele Office 365-Aktivierungen auf Desktops und Geräten durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="f90c4-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="f90c4-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="f90c4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="f90c4-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f90c4-106">Permissions</span></span>

<span data-ttu-id="f90c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f90c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f90c4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f90c4-109">Permission type</span></span>                        | <span data-ttu-id="f90c4-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f90c4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f90c4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f90c4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f90c4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f90c4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f90c4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f90c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f90c4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f90c4-114">Not supported.</span></span>                           |
| <span data-ttu-id="f90c4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f90c4-115">Application</span></span>                            | <span data-ttu-id="f90c4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f90c4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f90c4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f90c4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="f90c4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f90c4-118">Request headers</span></span>

| <span data-ttu-id="f90c4-119">Name</span><span class="sxs-lookup"><span data-stu-id="f90c4-119">Name</span></span>          | <span data-ttu-id="f90c4-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f90c4-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f90c4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f90c4-121">Authorization</span></span> | <span data-ttu-id="f90c4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f90c4-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f90c4-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f90c4-124">If-None-Match</span></span> | <span data-ttu-id="f90c4-125">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f90c4-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f90c4-126">Optional.</span><span class="sxs-lookup"><span data-stu-id="f90c4-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f90c4-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f90c4-127">Response</span></span>

<span data-ttu-id="f90c4-128">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="f90c4-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f90c4-129">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f90c4-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f90c4-130">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="f90c4-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f90c4-131">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="f90c4-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f90c4-132">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="f90c4-132">Report Refresh Date</span></span>
- <span data-ttu-id="f90c4-133">Produkttyp</span><span class="sxs-lookup"><span data-stu-id="f90c4-133">Product Type</span></span>
- <span data-ttu-id="f90c4-134">Windows</span><span class="sxs-lookup"><span data-stu-id="f90c4-134">Windows</span></span>
- <span data-ttu-id="f90c4-135">Mac</span><span class="sxs-lookup"><span data-stu-id="f90c4-135">Mac</span></span>
- <span data-ttu-id="f90c4-136">Android</span><span class="sxs-lookup"><span data-stu-id="f90c4-136">Android</span></span>
- <span data-ttu-id="f90c4-137">iOS</span><span class="sxs-lookup"><span data-stu-id="f90c4-137">iOS</span></span>
- <span data-ttu-id="f90c4-138">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="f90c4-138">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="f90c4-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f90c4-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f90c4-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f90c4-140">Request</span></span>

<span data-ttu-id="f90c4-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f90c4-141">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```

#### <a name="response"></a><span data-ttu-id="f90c4-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="f90c4-142">Response</span></span>

<span data-ttu-id="f90c4-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f90c4-143">The following is an example of the response.</span></span>

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

<span data-ttu-id="f90c4-144">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="f90c4-144">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```
