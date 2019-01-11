---
title: onenoteOperation abrufen
description: 'Dient zum Abrufen des Status eines lange dauernden OneNote-Vorgangs. Dies gilt für Vorgänge, die den Header **Operation-Location** in der Antwort zurückgeben, z. B. `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.   '
localization_priority: Normal
ms.openlocfilehash: b62f83266560f217d9569c6ee7ca39dd53198bb7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824766"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="7598c-104">onenoteOperation abrufen</span><span class="sxs-lookup"><span data-stu-id="7598c-104">Get onenoteOperation</span></span>

> <span data-ttu-id="7598c-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7598c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7598c-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7598c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7598c-p103">Dient zum Abrufen des Status eines lange dauernden OneNote-Vorgangs. Dies gilt für Vorgänge, die den Header **Operation-Location** in der Antwort zurückgeben, z. B. `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span><span class="sxs-lookup"><span data-stu-id="7598c-p103">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="7598c-109">Sie können den Operation-Location-Endpunkt abfragen, bis die Eigenschaft `status` `completed` oder `failed` zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="7598c-109">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="7598c-110">Wenn der Status `completed` lautet, enthält die Eigenschaft `resourceLocation` den URI des Ressourcenendpunkts.</span><span class="sxs-lookup"><span data-stu-id="7598c-110">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="7598c-111">Wenn der Status `failed` lautet, finden Sie Fehlerinformationen in den Eigenschaften „error“ und `@api.diagnostics`.</span><span class="sxs-lookup"><span data-stu-id="7598c-111">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="7598c-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7598c-112">Permissions</span></span>
<span data-ttu-id="7598c-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7598c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7598c-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7598c-115">Permission type</span></span>      | <span data-ttu-id="7598c-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7598c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7598c-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7598c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7598c-118">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7598c-118">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7598c-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7598c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7598c-120">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7598c-120">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7598c-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7598c-121">Application</span></span> | <span data-ttu-id="7598c-122">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7598c-122">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7598c-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7598c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7598c-124">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7598c-124">Optional query parameters</span></span>
<span data-ttu-id="7598c-125">Keine.</span><span class="sxs-lookup"><span data-stu-id="7598c-125">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7598c-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7598c-126">Request headers</span></span>
| <span data-ttu-id="7598c-127">Name</span><span class="sxs-lookup"><span data-stu-id="7598c-127">Name</span></span>       | <span data-ttu-id="7598c-128">Typ</span><span class="sxs-lookup"><span data-stu-id="7598c-128">Type</span></span> | <span data-ttu-id="7598c-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7598c-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7598c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="7598c-130">Authorization</span></span>  | <span data-ttu-id="7598c-131">string</span><span class="sxs-lookup"><span data-stu-id="7598c-131">string</span></span>  | <span data-ttu-id="7598c-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7598c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7598c-134">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7598c-134">Accept</span></span> | <span data-ttu-id="7598c-135">string</span><span class="sxs-lookup"><span data-stu-id="7598c-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7598c-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7598c-136">Request body</span></span>
<span data-ttu-id="7598c-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7598c-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7598c-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="7598c-138">Response</span></span>

<span data-ttu-id="7598c-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [onenoteOperation](../resources/onenoteoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7598c-139">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7598c-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7598c-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7598c-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7598c-141">Request</span></span>
<span data-ttu-id="7598c-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7598c-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="7598c-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="7598c-143">Response</span></span>
<span data-ttu-id="7598c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7598c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
