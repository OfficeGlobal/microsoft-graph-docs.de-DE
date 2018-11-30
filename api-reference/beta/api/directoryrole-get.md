---
title: directoryRole abrufen
description: Mit dieser API können Sie die Eigenschaften eines Objekts des Typs „directoryRole“ abrufen.
ms.openlocfilehash: 70894d736ee8d7e1f2fda0edf2bb60b9d3654da7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059569"
---
# <a name="get-directoryrole"></a><span data-ttu-id="9bc45-103">directoryRole abrufen</span><span class="sxs-lookup"><span data-stu-id="9bc45-103">Get directoryRole</span></span>

> <span data-ttu-id="9bc45-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9bc45-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bc45-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9bc45-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9bc45-106">Mit dieser API können Sie die Eigenschaften eines Objekts des Typs „directoryRole“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="9bc45-106">Retrieve the properties of a directoryRole object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9bc45-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9bc45-107">Permissions</span></span>
<span data-ttu-id="9bc45-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bc45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bc45-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9bc45-110">Permission type</span></span>      | <span data-ttu-id="9bc45-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9bc45-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bc45-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9bc45-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9bc45-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9bc45-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9bc45-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9bc45-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bc45-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bc45-115">Not supported.</span></span>    |
|<span data-ttu-id="9bc45-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9bc45-116">Application</span></span> | <span data-ttu-id="9bc45-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bc45-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bc45-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bc45-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9bc45-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9bc45-119">Optional query parameters</span></span>
<span data-ttu-id="9bc45-120">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort werden von dieser Methode **nicht** unterstützt (d. h. „$filter“ wird nicht unterstützt).</span><span class="sxs-lookup"><span data-stu-id="9bc45-120">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bc45-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9bc45-121">Request headers</span></span>
| <span data-ttu-id="9bc45-122">Name</span><span class="sxs-lookup"><span data-stu-id="9bc45-122">Name</span></span>       | <span data-ttu-id="9bc45-123">Typ</span><span class="sxs-lookup"><span data-stu-id="9bc45-123">Type</span></span> | <span data-ttu-id="9bc45-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bc45-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9bc45-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bc45-125">Authorization</span></span>  | <span data-ttu-id="9bc45-126">string</span><span class="sxs-lookup"><span data-stu-id="9bc45-126">string</span></span>  | <span data-ttu-id="9bc45-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9bc45-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bc45-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9bc45-129">Request body</span></span>
<span data-ttu-id="9bc45-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9bc45-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bc45-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bc45-131">Response</span></span>

<span data-ttu-id="9bc45-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9bc45-132">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9bc45-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9bc45-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9bc45-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bc45-134">Request</span></span>
<span data-ttu-id="9bc45-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9bc45-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="9bc45-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bc45-136">Response</span></span>
<span data-ttu-id="9bc45-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9bc45-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 142

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
