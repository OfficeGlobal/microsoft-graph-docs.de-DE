---
title: 'reportRoot: getSkypeForBusinessParticipantActivityCounts'
description: Erhalten Sie einen Überblick über die Anzahl und die Art von Konferenzsitzungen, an denen Benutzer aus Ihrer Organisation teilgenommen  haben. Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web und Einwahl/Auswahl (Drittanbieter).
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 89ff6ba99bbd60d16d6cdc0cb23f4ae91bfef76c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530013"
---
# <a name="reportroot-getskypeforbusinessparticipantactivitycounts"></a><span data-ttu-id="44cd8-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="44cd8-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44cd8-105">Erhalten Sie einen Überblick über die Anzahl und die Art von Konferenzsitzungen, an denen Benutzer aus Ihrer Organisation teilgenommen  haben.</span><span class="sxs-lookup"><span data-stu-id="44cd8-105">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="44cd8-106">Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web und Einwahl/Auswahl (Drittanbieter).</span><span class="sxs-lookup"><span data-stu-id="44cd8-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="44cd8-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Konferenzteilnehmeraktivität](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="44cd8-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="44cd8-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="44cd8-108">Permissions</span></span>

<span data-ttu-id="44cd8-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44cd8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44cd8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44cd8-111">Permission type</span></span>                        | <span data-ttu-id="44cd8-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44cd8-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="44cd8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44cd8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="44cd8-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44cd8-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="44cd8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44cd8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44cd8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44cd8-116">Not supported.</span></span>                           |
| <span data-ttu-id="44cd8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44cd8-117">Application</span></span>                            | <span data-ttu-id="44cd8-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44cd8-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="44cd8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44cd8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="44cd8-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="44cd8-120">Function parameters</span></span>

<span data-ttu-id="44cd8-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="44cd8-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="44cd8-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="44cd8-122">Parameter</span></span> | <span data-ttu-id="44cd8-123">Typ</span><span class="sxs-lookup"><span data-stu-id="44cd8-123">Type</span></span>   | <span data-ttu-id="44cd8-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44cd8-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="44cd8-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="44cd8-125">period</span></span>    | <span data-ttu-id="44cd8-126">string</span><span class="sxs-lookup"><span data-stu-id="44cd8-126">string</span></span> | <span data-ttu-id="44cd8-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="44cd8-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="44cd8-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="44cd8-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="44cd8-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="44cd8-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="44cd8-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="44cd8-130">Required.</span></span> |

<span data-ttu-id="44cd8-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44cd8-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="44cd8-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="44cd8-132">The default output type is text/csv.</span></span> <span data-ttu-id="44cd8-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="44cd8-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44cd8-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44cd8-134">Request headers</span></span>

| <span data-ttu-id="44cd8-135">Name</span><span class="sxs-lookup"><span data-stu-id="44cd8-135">Name</span></span>          | <span data-ttu-id="44cd8-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44cd8-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="44cd8-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="44cd8-137">Authorization</span></span> | <span data-ttu-id="44cd8-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="44cd8-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="44cd8-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="44cd8-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="44cd8-141">CSV</span><span class="sxs-lookup"><span data-stu-id="44cd8-141">CSV</span></span>

<span data-ttu-id="44cd8-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="44cd8-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="44cd8-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44cd8-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="44cd8-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="44cd8-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="44cd8-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="44cd8-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="44cd8-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="44cd8-146">Report Refresh Date</span></span>
- <span data-ttu-id="44cd8-147">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="44cd8-147">Report Date</span></span>
- <span data-ttu-id="44cd8-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="44cd8-148">Report Period</span></span>
- <span data-ttu-id="44cd8-149">Chat</span><span class="sxs-lookup"><span data-stu-id="44cd8-149">IM</span></span>
- <span data-ttu-id="44cd8-150">Audio/Video</span><span class="sxs-lookup"><span data-stu-id="44cd8-150">Audio/Video</span></span>
- <span data-ttu-id="44cd8-151">Gemeinsame Nutzung von Anwendungen</span><span class="sxs-lookup"><span data-stu-id="44cd8-151">App Sharing</span></span>
- <span data-ttu-id="44cd8-152">Web</span><span class="sxs-lookup"><span data-stu-id="44cd8-152">Web</span></span>
- <span data-ttu-id="44cd8-153">Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="44cd8-153">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="44cd8-154">JSON</span><span class="sxs-lookup"><span data-stu-id="44cd8-154">JSON</span></span>

<span data-ttu-id="44cd8-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="44cd8-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44cd8-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44cd8-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="44cd8-157">CSV</span><span class="sxs-lookup"><span data-stu-id="44cd8-157">CSV</span></span>

<span data-ttu-id="44cd8-158">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="44cd8-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="44cd8-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44cd8-159">Request</span></span>

<span data-ttu-id="44cd8-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44cd8-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="44cd8-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="44cd8-161">Response</span></span>

<span data-ttu-id="44cd8-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44cd8-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="44cd8-163">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="44cd8-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a><span data-ttu-id="44cd8-164">JSON</span><span class="sxs-lookup"><span data-stu-id="44cd8-164">JSON</span></span>

<span data-ttu-id="44cd8-165">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44cd8-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="44cd8-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44cd8-166">Request</span></span>

<span data-ttu-id="44cd8-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44cd8-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="44cd8-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="44cd8-168">Response</span></span>

<span data-ttu-id="44cd8-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44cd8-169">The following is an example of the response.</span></span>

> <span data-ttu-id="44cd8-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="44cd8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 296

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityCounts)", 
  "value": [
    {
      "im": 162, 
      "audioVideo": 156, 
      "appSharing": 45, 
      "web": 12, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
