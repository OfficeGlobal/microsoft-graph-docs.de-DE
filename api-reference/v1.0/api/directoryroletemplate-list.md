---
title: directoryRoleTemplates auflisten
description: Mit dieser API können Sie eine Liste von Objekten des Typs „directoryRoleTemplate“ abrufen.
author: lleonard-msft
ms.openlocfilehash: 0e43bdb3217827c8369ebe226a9aacea54996be2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301526"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="68717-103">directoryRoleTemplates auflisten</span><span class="sxs-lookup"><span data-stu-id="68717-103">List directoryRoleTemplates</span></span>

<span data-ttu-id="68717-104">Mit dieser API können Sie eine Liste von Objekten des Typs „directoryRoleTemplate“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="68717-104">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="68717-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="68717-105">Permissions</span></span>
<span data-ttu-id="68717-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68717-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="68717-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="68717-108">Permission type</span></span>      | <span data-ttu-id="68717-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="68717-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68717-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="68717-110">Delegated (work or school account)</span></span> | <span data-ttu-id="68717-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="68717-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="68717-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="68717-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68717-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68717-113">Not supported.</span></span>    |
|<span data-ttu-id="68717-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="68717-114">Application</span></span> | <span data-ttu-id="68717-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68717-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68717-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="68717-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="68717-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="68717-117">Optional query parameters</span></span>
<span data-ttu-id="68717-118">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort werden von dieser Methode **nicht** unterstützt (d. h. „$filter“ wird nicht unterstützt).</span><span class="sxs-lookup"><span data-stu-id="68717-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="68717-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="68717-119">Request headers</span></span>
| <span data-ttu-id="68717-120">Name</span><span class="sxs-lookup"><span data-stu-id="68717-120">Name</span></span>       | <span data-ttu-id="68717-121">Typ</span><span class="sxs-lookup"><span data-stu-id="68717-121">Type</span></span> | <span data-ttu-id="68717-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68717-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="68717-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="68717-123">Authorization</span></span>  | <span data-ttu-id="68717-124">string</span><span class="sxs-lookup"><span data-stu-id="68717-124">string</span></span>  | <span data-ttu-id="68717-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="68717-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68717-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="68717-127">Request body</span></span>
<span data-ttu-id="68717-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="68717-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68717-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="68717-129">Response</span></span>

<span data-ttu-id="68717-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryRoleTemplate](../resources/directoryroletemplate.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68717-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="68717-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="68717-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68717-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="68717-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
##### <a name="response"></a><span data-ttu-id="68717-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="68717-133">Response</span></span>
<span data-ttu-id="68717-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68717-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
