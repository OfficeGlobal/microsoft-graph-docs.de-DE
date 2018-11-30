---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: Erhalten Sie einen Überblick über die Dauer in Minuten und die Art von Konferenzsitzungen, an denen Benutzer aus Ihrer Organisation teilgenommen  haben. Zu den Arten von Konferenzsitzungen gehören Audio/Video.
ms.openlocfilehash: f62215296e59212aaf9dfef975f08534d2f56c64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017320"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="0a62f-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="0a62f-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="0a62f-105">Erhalten Sie einen Überblick über die Dauer in Minuten und die Art von Konferenzsitzungen, an denen Benutzer aus Ihrer Organisation teilgenommen  haben.</span><span class="sxs-lookup"><span data-stu-id="0a62f-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="0a62f-106">Zu den Arten von Konferenzsitzungen gehören Audio/Video.</span><span class="sxs-lookup"><span data-stu-id="0a62f-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="0a62f-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Konferenzteilnehmeraktivität](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="0a62f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="0a62f-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0a62f-108">Permissions</span></span>

<span data-ttu-id="0a62f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a62f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a62f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a62f-111">Permission type</span></span>                        | <span data-ttu-id="0a62f-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a62f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0a62f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a62f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a62f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a62f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0a62f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a62f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a62f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a62f-116">Not supported.</span></span>                           |
| <span data-ttu-id="0a62f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a62f-117">Application</span></span>                            | <span data-ttu-id="0a62f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a62f-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0a62f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a62f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0a62f-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="0a62f-120">Function parameters</span></span>

<span data-ttu-id="0a62f-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="0a62f-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0a62f-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="0a62f-122">Parameter</span></span> | <span data-ttu-id="0a62f-123">Typ</span><span class="sxs-lookup"><span data-stu-id="0a62f-123">Type</span></span>   | <span data-ttu-id="0a62f-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a62f-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0a62f-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="0a62f-125">period</span></span>    | <span data-ttu-id="0a62f-126">string</span><span class="sxs-lookup"><span data-stu-id="0a62f-126">string</span></span> | <span data-ttu-id="0a62f-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0a62f-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0a62f-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="0a62f-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0a62f-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0a62f-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0a62f-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="0a62f-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0a62f-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a62f-131">Request headers</span></span>

| <span data-ttu-id="0a62f-132">Name</span><span class="sxs-lookup"><span data-stu-id="0a62f-132">Name</span></span>          | <span data-ttu-id="0a62f-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a62f-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0a62f-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a62f-134">Authorization</span></span> | <span data-ttu-id="0a62f-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0a62f-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0a62f-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0a62f-137">If-None-Match</span></span> | <span data-ttu-id="0a62f-138">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a62f-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0a62f-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="0a62f-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0a62f-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a62f-140">Response</span></span>

<span data-ttu-id="0a62f-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="0a62f-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0a62f-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0a62f-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0a62f-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="0a62f-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0a62f-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="0a62f-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0a62f-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="0a62f-145">Report Refresh Date</span></span>
- <span data-ttu-id="0a62f-146">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="0a62f-146">Report Date</span></span>
- <span data-ttu-id="0a62f-147">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="0a62f-147">Report Period</span></span>
- <span data-ttu-id="0a62f-148">Audio/Video</span><span class="sxs-lookup"><span data-stu-id="0a62f-148">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="0a62f-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a62f-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0a62f-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a62f-150">Request</span></span>

<span data-ttu-id="0a62f-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0a62f-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="0a62f-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a62f-152">Response</span></span>

<span data-ttu-id="0a62f-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0a62f-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="0a62f-154">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="0a62f-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
```