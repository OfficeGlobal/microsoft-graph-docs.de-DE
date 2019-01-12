---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Rufen Sie die Anzahl von Benutzern, die aktiviert sind und die aktiviert das Office-Abonnement auf Desktop- oder Geräte oder Computer freigegeben haben.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 9b284793ba4031c9354e9134b81798e738410f38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921122"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="9d787-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="9d787-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="9d787-104">Rufen Sie die Anzahl von Benutzern, die aktiviert sind und die aktiviert das Office-Abonnement auf Desktop- oder Geräte oder Computer freigegeben haben.</span><span class="sxs-lookup"><span data-stu-id="9d787-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="9d787-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="9d787-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="9d787-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9d787-106">Permissions</span></span>

<span data-ttu-id="9d787-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d787-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d787-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d787-109">Permission type</span></span>                        | <span data-ttu-id="9d787-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d787-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9d787-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d787-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d787-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d787-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9d787-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d787-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d787-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d787-114">Not supported.</span></span>                           |
| <span data-ttu-id="9d787-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d787-115">Application</span></span>                            | <span data-ttu-id="9d787-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d787-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9d787-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d787-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="9d787-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d787-118">Request headers</span></span>

| <span data-ttu-id="9d787-119">Name</span><span class="sxs-lookup"><span data-stu-id="9d787-119">Name</span></span>          | <span data-ttu-id="9d787-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d787-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9d787-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d787-121">Authorization</span></span> | <span data-ttu-id="9d787-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9d787-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9d787-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9d787-124">If-None-Match</span></span> | <span data-ttu-id="9d787-125">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d787-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9d787-126">Optional.</span><span class="sxs-lookup"><span data-stu-id="9d787-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9d787-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d787-127">Response</span></span>

<span data-ttu-id="9d787-128">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="9d787-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9d787-129">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9d787-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9d787-130">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="9d787-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9d787-131">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="9d787-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9d787-132">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="9d787-132">Report Refresh Date</span></span>
- <span data-ttu-id="9d787-133">Produkttyp</span><span class="sxs-lookup"><span data-stu-id="9d787-133">Product Type</span></span>
- <span data-ttu-id="9d787-134">Zugewiesen</span><span class="sxs-lookup"><span data-stu-id="9d787-134">Assigned</span></span>
- <span data-ttu-id="9d787-135">Aktiviert</span><span class="sxs-lookup"><span data-stu-id="9d787-135">Activated</span></span>
- <span data-ttu-id="9d787-136">Gemeinsam genutzter Computer-Aktivierung</span><span class="sxs-lookup"><span data-stu-id="9d787-136">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="9d787-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d787-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9d787-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d787-138">Request</span></span>

<span data-ttu-id="9d787-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9d787-139">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```

#### <a name="response"></a><span data-ttu-id="9d787-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d787-140">Response</span></span>

<span data-ttu-id="9d787-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9d787-141">The following is an example of the response.</span></span>

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

<span data-ttu-id="9d787-142">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="9d787-142">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```
