---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: Erhalten Sie Informationen über die Anzahl der eindeutigen Benutzer und die Art der von Benutzern in Ihrer Organisation gehaltenen und organisierten Konferenzsitzungen. Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web, Einwahl/Auswahl Drittanbieter und Einwahl/Auswahl Microsoft.
localization_priority: Normal
ms.openlocfilehash: 6677b6eab3f381ea244bb677c09c2c6ecf361bd2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870970"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="b6077-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="b6077-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

<span data-ttu-id="b6077-105">Erhalten Sie Informationen über die Anzahl der eindeutigen Benutzer und die Art der von Benutzern in Ihrer Organisation gehaltenen und organisierten Konferenzsitzungen.</span><span class="sxs-lookup"><span data-stu-id="b6077-105">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="b6077-106">Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web, Einwahl/Auswahl Drittanbieter und Einwahl/Auswahl Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b6077-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="b6077-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Konferenzorganisationsaktivität](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="b6077-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6077-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b6077-108">Permissions</span></span>

<span data-ttu-id="b6077-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6077-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6077-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b6077-111">Permission type</span></span>                        | <span data-ttu-id="b6077-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b6077-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b6077-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b6077-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6077-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6077-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b6077-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b6077-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6077-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6077-116">Not supported.</span></span>                           |
| <span data-ttu-id="b6077-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b6077-117">Application</span></span>                            | <span data-ttu-id="b6077-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6077-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b6077-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6077-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b6077-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="b6077-120">Function parameters</span></span>

<span data-ttu-id="b6077-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="b6077-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b6077-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="b6077-122">Parameter</span></span> | <span data-ttu-id="b6077-123">Typ</span><span class="sxs-lookup"><span data-stu-id="b6077-123">Type</span></span>   | <span data-ttu-id="b6077-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6077-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b6077-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="b6077-125">period</span></span>    | <span data-ttu-id="b6077-126">string</span><span class="sxs-lookup"><span data-stu-id="b6077-126">string</span></span> | <span data-ttu-id="b6077-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b6077-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b6077-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="b6077-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b6077-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b6077-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b6077-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="b6077-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b6077-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b6077-131">Request headers</span></span>

| <span data-ttu-id="b6077-132">Name</span><span class="sxs-lookup"><span data-stu-id="b6077-132">Name</span></span>          | <span data-ttu-id="b6077-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6077-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b6077-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6077-134">Authorization</span></span> | <span data-ttu-id="b6077-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b6077-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b6077-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b6077-137">If-None-Match</span></span> | <span data-ttu-id="b6077-138">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6077-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b6077-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="b6077-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b6077-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6077-140">Response</span></span>

<span data-ttu-id="b6077-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="b6077-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b6077-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b6077-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b6077-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="b6077-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b6077-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="b6077-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b6077-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="b6077-145">Report Refresh Date</span></span>
- <span data-ttu-id="b6077-146">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="b6077-146">Report Date</span></span>
- <span data-ttu-id="b6077-147">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="b6077-147">Report Period</span></span>
- <span data-ttu-id="b6077-148">Chat</span><span class="sxs-lookup"><span data-stu-id="b6077-148">IM</span></span>
- <span data-ttu-id="b6077-149">Audio/Video</span><span class="sxs-lookup"><span data-stu-id="b6077-149">Audio/Video</span></span>
- <span data-ttu-id="b6077-150">Gemeinsame Nutzung von Anwendungen</span><span class="sxs-lookup"><span data-stu-id="b6077-150">App Sharing</span></span>
- <span data-ttu-id="b6077-151">Web</span><span class="sxs-lookup"><span data-stu-id="b6077-151">Web</span></span>
- <span data-ttu-id="b6077-152">Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="b6077-152">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="b6077-153">Einwahl/Auswahl Microsoft</span><span class="sxs-lookup"><span data-stu-id="b6077-153">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="b6077-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b6077-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b6077-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6077-155">Request</span></span>

<span data-ttu-id="b6077-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b6077-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b6077-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6077-157">Response</span></span>

<span data-ttu-id="b6077-158">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b6077-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="b6077-159">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="b6077-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```
