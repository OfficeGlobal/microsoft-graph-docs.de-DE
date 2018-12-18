---
title: directoryRole abrufen
description: Mit dieser API können Sie die Eigenschaften eines Objekts des Typs „directoryRole“ abrufen.
author: lleonard-msft
ms.openlocfilehash: b5f25179c18a28aa3c12dd54c7230b5444dff3f8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305299"
---
# <a name="get-directoryrole"></a><span data-ttu-id="a1e4e-103">directoryRole abrufen</span><span class="sxs-lookup"><span data-stu-id="a1e4e-103">Get directoryRole</span></span>

<span data-ttu-id="a1e4e-104">Mit dieser API können Sie die Eigenschaften eines Objekts des Typs „directoryRole“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="a1e4e-104">Retrieve the properties of a directoryRole object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1e4e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a1e4e-105">Permissions</span></span>
<span data-ttu-id="a1e4e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1e4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1e4e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1e4e-108">Permission type</span></span>      | <span data-ttu-id="a1e4e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1e4e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1e4e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1e4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a1e4e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1e4e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a1e4e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1e4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1e4e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1e4e-113">Not supported.</span></span>    |
|<span data-ttu-id="a1e4e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1e4e-114">Application</span></span> | <span data-ttu-id="a1e4e-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1e4e-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1e4e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1e4e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a1e4e-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a1e4e-117">Optional query parameters</span></span>
<span data-ttu-id="a1e4e-118">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort werden von dieser Methode **nicht** unterstützt (d. h. „$filter“ wird nicht unterstützt).</span><span class="sxs-lookup"><span data-stu-id="a1e4e-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1e4e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1e4e-119">Request headers</span></span>
| <span data-ttu-id="a1e4e-120">Name</span><span class="sxs-lookup"><span data-stu-id="a1e4e-120">Name</span></span>       | <span data-ttu-id="a1e4e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="a1e4e-121">Type</span></span> | <span data-ttu-id="a1e4e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1e4e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a1e4e-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a1e4e-123">Authorization</span></span>  | <span data-ttu-id="a1e4e-124">string</span><span class="sxs-lookup"><span data-stu-id="a1e4e-124">string</span></span>  | <span data-ttu-id="a1e4e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a1e4e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1e4e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1e4e-127">Request body</span></span>
<span data-ttu-id="a1e4e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a1e4e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1e4e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1e4e-129">Response</span></span>

<span data-ttu-id="a1e4e-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1e4e-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1e4e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1e4e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1e4e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1e4e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="a1e4e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1e4e-133">Response</span></span>
<span data-ttu-id="a1e4e-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1e4e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
