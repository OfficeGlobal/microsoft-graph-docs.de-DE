---
title: onenoteOperation abrufen
description: 'Dient zum Abrufen des Status eines lange dauernden OneNote-Vorgangs. Dies gilt für Vorgänge, die den Header **Operation-Location** in der Antwort zurückgeben, z. B. `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.   '
ms.openlocfilehash: 67f11fb29d34b0d8cd2968cdc1dd5addabb3c0a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018817"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="6de7c-104">onenoteOperation abrufen</span><span class="sxs-lookup"><span data-stu-id="6de7c-104">Get onenoteOperation</span></span>

<span data-ttu-id="6de7c-p102">Dient zum Abrufen des Status eines lange dauernden OneNote-Vorgangs. Dies gilt für Vorgänge, die den Header **Operation-Location** in der Antwort zurückgeben, z. B. `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span><span class="sxs-lookup"><span data-stu-id="6de7c-p102">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="6de7c-107">Sie können den Operation-Location-Endpunkt abfragen, bis die Eigenschaft `status` `completed` oder `failed` zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="6de7c-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="6de7c-108">Wenn der Status `completed` lautet, enthält die Eigenschaft `resourceLocation` den URI des Ressourcenendpunkts.</span><span class="sxs-lookup"><span data-stu-id="6de7c-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="6de7c-109">Wenn der Status `failed` lautet, finden Sie Fehlerinformationen in den Eigenschaften „error“ und `@api.diagnostics`.</span><span class="sxs-lookup"><span data-stu-id="6de7c-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="6de7c-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6de7c-110">Permissions</span></span>
<span data-ttu-id="6de7c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6de7c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6de7c-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6de7c-113">Permission type</span></span>      | <span data-ttu-id="6de7c-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6de7c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6de7c-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6de7c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6de7c-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6de7c-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6de7c-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6de7c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6de7c-118">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6de7c-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6de7c-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6de7c-119">Application</span></span> | <span data-ttu-id="6de7c-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6de7c-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6de7c-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6de7c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6de7c-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6de7c-122">Optional query parameters</span></span>
<span data-ttu-id="6de7c-123">Keine.</span><span class="sxs-lookup"><span data-stu-id="6de7c-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6de7c-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6de7c-124">Request headers</span></span>
| <span data-ttu-id="6de7c-125">Name</span><span class="sxs-lookup"><span data-stu-id="6de7c-125">Name</span></span>       | <span data-ttu-id="6de7c-126">Typ</span><span class="sxs-lookup"><span data-stu-id="6de7c-126">Type</span></span> | <span data-ttu-id="6de7c-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6de7c-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6de7c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6de7c-128">Authorization</span></span>  | <span data-ttu-id="6de7c-129">string</span><span class="sxs-lookup"><span data-stu-id="6de7c-129">string</span></span>  | <span data-ttu-id="6de7c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6de7c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6de7c-132">Accept</span><span class="sxs-lookup"><span data-stu-id="6de7c-132">Accept</span></span> | <span data-ttu-id="6de7c-133">string</span><span class="sxs-lookup"><span data-stu-id="6de7c-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="6de7c-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6de7c-134">Request body</span></span>
<span data-ttu-id="6de7c-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6de7c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6de7c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6de7c-136">Response</span></span>

<span data-ttu-id="6de7c-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [onenoteOperation](../resources/onenoteoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6de7c-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6de7c-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6de7c-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6de7c-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6de7c-139">Request</span></span>
<span data-ttu-id="6de7c-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6de7c-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="6de7c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="6de7c-141">Response</span></span>
<span data-ttu-id="6de7c-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6de7c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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