---
title: 'Benutzer: ExportPersonalData'
description: Fordert die Daten Richtlinie Vorgang, versucht ein Unternehmensadministrator, eine Organisationseinheit Benutzerdaten exportieren.
localization_priority: Normal
ms.openlocfilehash: d660994868e331fb8c1813bb9ff90aebe4790e9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845339"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="e6045-103">Benutzer: ExportPersonalData</span><span class="sxs-lookup"><span data-stu-id="e6045-103">user: exportPersonalData</span></span>

<span data-ttu-id="e6045-104">Fordert die Daten Richtlinie Vorgang, mit einem Unternehmensadministrator vorgenommenen Änderungen für eine Organisationseinheit Benutzerdaten exportieren.</span><span class="sxs-lookup"><span data-stu-id="e6045-104">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6045-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e6045-105">Permissions</span></span>
<span data-ttu-id="e6045-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6045-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6045-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6045-108">Permission type</span></span>      | <span data-ttu-id="e6045-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6045-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6045-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6045-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e6045-111">User.Export.All und User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6045-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="e6045-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6045-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e6045-113">Nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="e6045-113">Not applicable</span></span>  |
|<span data-ttu-id="e6045-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6045-114">Application</span></span> | <span data-ttu-id="e6045-115">User.Export.All und User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6045-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="e6045-116">**Hinweis:** Export kann nur von einem Unternehmensadministrator ausgeführt werden, wenn die delegierte Berechtigung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e6045-116">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="e6045-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6045-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="e6045-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6045-118">Request headers</span></span>
| <span data-ttu-id="e6045-119">Name</span><span class="sxs-lookup"><span data-stu-id="e6045-119">Name</span></span>       | <span data-ttu-id="e6045-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6045-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e6045-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6045-121">Authorization</span></span>  | <span data-ttu-id="e6045-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e6045-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6045-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6045-123">Request body</span></span>
<span data-ttu-id="e6045-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="e6045-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6045-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="e6045-125">Parameter</span></span>    | <span data-ttu-id="e6045-126">Typ</span><span class="sxs-lookup"><span data-stu-id="e6045-126">Type</span></span>   |<span data-ttu-id="e6045-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6045-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e6045-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="e6045-128">storageLocation</span></span>|<span data-ttu-id="e6045-129">String</span><span class="sxs-lookup"><span data-stu-id="e6045-129">String</span></span>|<span data-ttu-id="e6045-130">Dies ist die URL einer gemeinsamen Zugriff Signatur (SAS) ein Konto Azure-Speicher an, in dem Daten exportiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e6045-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="e6045-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6045-131">Response</span></span>
<span data-ttu-id="e6045-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6045-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="e6045-133">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e6045-133">It does not return anything in the response body.</span></span> <span data-ttu-id="e6045-134">Die Antwort enthält die folgenden Kopfzeilen.</span><span class="sxs-lookup"><span data-stu-id="e6045-134">The response contains the following headers.</span></span>

| <span data-ttu-id="e6045-135">Name</span><span class="sxs-lookup"><span data-stu-id="e6045-135">Name</span></span>       | <span data-ttu-id="e6045-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6045-136">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e6045-137">Location</span><span class="sxs-lookup"><span data-stu-id="e6045-137">Location</span></span>  | <span data-ttu-id="e6045-138">URL, die den Status der Anforderung überprüfen.</span><span class="sxs-lookup"><span data-stu-id="e6045-138">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="e6045-139">Wiederholen Sie den Vorgang nach</span><span class="sxs-lookup"><span data-stu-id="e6045-139">Retry-After</span></span>  | <span data-ttu-id="e6045-140">Der Zeitraum in Sekunden.</span><span class="sxs-lookup"><span data-stu-id="e6045-140">Time period in seconds.</span></span> <span data-ttu-id="e6045-141">Anforderung Maker warten soll lange nach der Übermittlung einer Anforderung an den Status überprüfen.</span><span class="sxs-lookup"><span data-stu-id="e6045-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="e6045-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6045-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6045-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6045-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a><span data-ttu-id="e6045-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6045-144">Response</span></span>

```
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
