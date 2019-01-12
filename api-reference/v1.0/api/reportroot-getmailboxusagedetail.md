---
title: 'reportRoot: getMailboxUsageDetail'
description: Erhalten Sie detaillierte Informationen über die Postfachnutzung.
localization_priority: Priority
ms.prod: reports
ms.openlocfilehash: a4f412d8acdb32648ceb47e4aed6f2b7ff83268d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953483"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="a8ace-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="a8ace-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="a8ace-104">Erhalten Sie detaillierte Informationen über die Postfachnutzung.</span><span class="sxs-lookup"><span data-stu-id="a8ace-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="a8ace-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Postfachnutzung](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="a8ace-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8ace-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a8ace-106">Permissions</span></span>

<span data-ttu-id="a8ace-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8ace-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8ace-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8ace-109">Permission type</span></span>                        | <span data-ttu-id="a8ace-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8ace-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a8ace-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8ace-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8ace-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8ace-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a8ace-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8ace-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8ace-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8ace-114">Not supported.</span></span>                           |
| <span data-ttu-id="a8ace-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8ace-115">Application</span></span>                            | <span data-ttu-id="a8ace-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8ace-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a8ace-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8ace-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a8ace-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="a8ace-118">Function parameters</span></span>

<span data-ttu-id="a8ace-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="a8ace-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a8ace-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="a8ace-120">Parameter</span></span> | <span data-ttu-id="a8ace-121">Typ</span><span class="sxs-lookup"><span data-stu-id="a8ace-121">Type</span></span>   | <span data-ttu-id="a8ace-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8ace-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a8ace-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="a8ace-123">period</span></span>    | <span data-ttu-id="a8ace-124">string</span><span class="sxs-lookup"><span data-stu-id="a8ace-124">string</span></span> | <span data-ttu-id="a8ace-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="a8ace-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a8ace-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="a8ace-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a8ace-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="a8ace-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a8ace-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="a8ace-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a8ace-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8ace-129">Request headers</span></span>

| <span data-ttu-id="a8ace-130">Name</span><span class="sxs-lookup"><span data-stu-id="a8ace-130">Name</span></span>          | <span data-ttu-id="a8ace-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8ace-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a8ace-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8ace-132">Authorization</span></span> | <span data-ttu-id="a8ace-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8ace-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a8ace-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a8ace-135">If-None-Match</span></span> | <span data-ttu-id="a8ace-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8ace-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a8ace-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="a8ace-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a8ace-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8ace-138">Response</span></span>

<span data-ttu-id="a8ace-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="a8ace-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a8ace-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a8ace-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a8ace-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="a8ace-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a8ace-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="a8ace-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a8ace-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="a8ace-143">Report Refresh Date</span></span>
- <span data-ttu-id="a8ace-144">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="a8ace-144">User Principal Name</span></span>
- <span data-ttu-id="a8ace-145">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="a8ace-145">Display Name</span></span>
- <span data-ttu-id="a8ace-146">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="a8ace-146">Is Deleted</span></span>
- <span data-ttu-id="a8ace-147">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="a8ace-147">Deleted Date</span></span>
- <span data-ttu-id="a8ace-148">Erstellungsdatum</span><span class="sxs-lookup"><span data-stu-id="a8ace-148">Created Date</span></span>
- <span data-ttu-id="a8ace-149">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="a8ace-149">Last Activity Date</span></span>
- <span data-ttu-id="a8ace-150">Elementanzahl</span><span class="sxs-lookup"><span data-stu-id="a8ace-150">Item Count</span></span>
- <span data-ttu-id="a8ace-151">Verwendeter Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="a8ace-151">Storage Used (Byte)</span></span>
- <span data-ttu-id="a8ace-152">Kontingent für Problemwarnung (Byte)</span><span class="sxs-lookup"><span data-stu-id="a8ace-152">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="a8ace-153">Kontingent für Senden verbieten (Byte)</span><span class="sxs-lookup"><span data-stu-id="a8ace-153">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="a8ace-154">Kontingent für Senden/Empfangen verbieten (Byte)</span><span class="sxs-lookup"><span data-stu-id="a8ace-154">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="a8ace-155">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="a8ace-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a8ace-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8ace-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a8ace-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8ace-157">Request</span></span>

<span data-ttu-id="a8ace-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8ace-158">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="a8ace-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8ace-159">Response</span></span>

<span data-ttu-id="a8ace-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a8ace-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="a8ace-161">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="a8ace-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
```
