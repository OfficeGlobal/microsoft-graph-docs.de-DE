---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: Erhalten Sie Informationen über die Anzahl der eindeutigen Benutzer und die Art der in Ihrem Unternehmen gehaltenen Peer-to-Peer-Sitzungen. Zu den Sitzungsarten gehören Chat, Audio, Video, Anwendungsfreigabe und Dateiübertragung in Peer-to-Peer-Sitzungen.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 98eadcbee3d2465446c3fe6b581da004f0c54ed4
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574607"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="6e4f2-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="6e4f2-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

<span data-ttu-id="6e4f2-105">Erhalten Sie Informationen über die Anzahl der eindeutigen Benutzer und die Art der in Ihrem Unternehmen gehaltenen Peer-to-Peer-Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-105">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="6e4f2-106">Zu den Sitzungsarten gehören Chat, Audio, Video, Anwendungsfreigabe und Dateiübertragung in Peer-to-Peer-Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-106">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="6e4f2-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Peer-to-Peer-Aktivität](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="6e4f2-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e4f2-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6e4f2-108">Permissions</span></span>

<span data-ttu-id="6e4f2-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e4f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e4f2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6e4f2-111">Permission type</span></span>                        | <span data-ttu-id="6e4f2-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6e4f2-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6e4f2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6e4f2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e4f2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e4f2-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6e4f2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6e4f2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e4f2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e4f2-116">Not supported.</span></span>                           |
| <span data-ttu-id="6e4f2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6e4f2-117">Application</span></span>                            | <span data-ttu-id="6e4f2-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e4f2-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6e4f2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e4f2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6e4f2-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="6e4f2-120">Function parameters</span></span>

<span data-ttu-id="6e4f2-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6e4f2-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="6e4f2-122">Parameter</span></span> | <span data-ttu-id="6e4f2-123">Typ</span><span class="sxs-lookup"><span data-stu-id="6e4f2-123">Type</span></span>   | <span data-ttu-id="6e4f2-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e4f2-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6e4f2-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="6e4f2-125">period</span></span>    | <span data-ttu-id="6e4f2-126">string</span><span class="sxs-lookup"><span data-stu-id="6e4f2-126">string</span></span> | <span data-ttu-id="6e4f2-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6e4f2-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6e4f2-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6e4f2-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="6e4f2-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6e4f2-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6e4f2-131">Request headers</span></span>

| <span data-ttu-id="6e4f2-132">Name</span><span class="sxs-lookup"><span data-stu-id="6e4f2-132">Name</span></span>          | <span data-ttu-id="6e4f2-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e4f2-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6e4f2-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e4f2-134">Authorization</span></span> | <span data-ttu-id="6e4f2-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6e4f2-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6e4f2-137">If-None-Match</span></span> | <span data-ttu-id="6e4f2-138">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6e4f2-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6e4f2-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e4f2-140">Response</span></span>

<span data-ttu-id="6e4f2-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6e4f2-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6e4f2-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6e4f2-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6e4f2-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="6e4f2-145">Report Refresh Date</span></span>
- <span data-ttu-id="6e4f2-146">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="6e4f2-146">Report Date</span></span>
- <span data-ttu-id="6e4f2-147">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="6e4f2-147">Report Period</span></span>
- <span data-ttu-id="6e4f2-148">Chat</span><span class="sxs-lookup"><span data-stu-id="6e4f2-148">IM</span></span>
- <span data-ttu-id="6e4f2-149">Audio</span><span class="sxs-lookup"><span data-stu-id="6e4f2-149">Audio</span></span>
- <span data-ttu-id="6e4f2-150">Video</span><span class="sxs-lookup"><span data-stu-id="6e4f2-150">Video</span></span>
- <span data-ttu-id="6e4f2-151">Gemeinsame Nutzung von Anwendungen</span><span class="sxs-lookup"><span data-stu-id="6e4f2-151">App Sharing</span></span>
- <span data-ttu-id="6e4f2-152">Dateiübertragung</span><span class="sxs-lookup"><span data-stu-id="6e4f2-152">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="6e4f2-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6e4f2-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6e4f2-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e4f2-154">Request</span></span>

<span data-ttu-id="6e4f2-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="6e4f2-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e4f2-156">Response</span></span>

<span data-ttu-id="6e4f2-157">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="6e4f2-158">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="6e4f2-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```
