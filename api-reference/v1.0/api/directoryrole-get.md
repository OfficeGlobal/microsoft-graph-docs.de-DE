---
title: directoryRole abrufen
description: Mit dieser API können Sie die Eigenschaften eines Objekts des Typs „directoryRole“ abrufen.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: f8ff306359675f7bc2c569f507dbcb3baf33b384
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832228"
---
# <a name="get-directoryrole"></a><span data-ttu-id="e4406-103">directoryRole abrufen</span><span class="sxs-lookup"><span data-stu-id="e4406-103">Get directoryRole</span></span>

<span data-ttu-id="e4406-104">Mit dieser API können Sie die Eigenschaften eines Objekts des Typs „directoryRole“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="e4406-104">Retrieve the properties of a directoryRole object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4406-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e4406-105">Permissions</span></span>
<span data-ttu-id="e4406-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4406-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4406-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4406-108">Permission type</span></span>      | <span data-ttu-id="e4406-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4406-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4406-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4406-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4406-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e4406-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e4406-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4406-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4406-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4406-113">Not supported.</span></span>    |
|<span data-ttu-id="e4406-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4406-114">Application</span></span> | <span data-ttu-id="e4406-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4406-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4406-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4406-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e4406-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e4406-117">Optional query parameters</span></span>
<span data-ttu-id="e4406-118">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort werden von dieser Methode **nicht** unterstützt (d. h. „$filter“ wird nicht unterstützt).</span><span class="sxs-lookup"><span data-stu-id="e4406-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4406-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4406-119">Request headers</span></span>
| <span data-ttu-id="e4406-120">Name</span><span class="sxs-lookup"><span data-stu-id="e4406-120">Name</span></span>       | <span data-ttu-id="e4406-121">Typ</span><span class="sxs-lookup"><span data-stu-id="e4406-121">Type</span></span> | <span data-ttu-id="e4406-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4406-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e4406-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4406-123">Authorization</span></span>  | <span data-ttu-id="e4406-124">string</span><span class="sxs-lookup"><span data-stu-id="e4406-124">string</span></span>  | <span data-ttu-id="e4406-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4406-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4406-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4406-127">Request body</span></span>
<span data-ttu-id="e4406-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e4406-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4406-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4406-129">Response</span></span>

<span data-ttu-id="e4406-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4406-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4406-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4406-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4406-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4406-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="e4406-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4406-133">Response</span></span>
<span data-ttu-id="e4406-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4406-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
