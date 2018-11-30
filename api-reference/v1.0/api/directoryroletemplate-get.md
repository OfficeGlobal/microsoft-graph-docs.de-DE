---
title: directoryRoleTemplate abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs „directoryroletemplate“ abrufen.
ms.openlocfilehash: 2d5a49f149edfddc8ccc0fd199632a9832c133a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017199"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="9f378-103">directoryRoleTemplate abrufen</span><span class="sxs-lookup"><span data-stu-id="9f378-103">Get directoryRoleTemplate</span></span>

<span data-ttu-id="9f378-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs „directoryroletemplate“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="9f378-104">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f378-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f378-105">Permissions</span></span>
<span data-ttu-id="9f378-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f378-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f378-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f378-108">Permission type</span></span>      | <span data-ttu-id="9f378-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f378-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f378-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f378-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f378-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f378-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f378-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f378-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f378-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f378-113">Not supported.</span></span>    |
|<span data-ttu-id="9f378-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f378-114">Application</span></span> | <span data-ttu-id="9f378-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f378-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f378-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f378-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9f378-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9f378-117">Optional query parameters</span></span>
<span data-ttu-id="9f378-118">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort werden von dieser Methode **nicht** unterstützt (d. h. „$filter“ wird nicht unterstützt).</span><span class="sxs-lookup"><span data-stu-id="9f378-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f378-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f378-119">Request headers</span></span>
| <span data-ttu-id="9f378-120">Name</span><span class="sxs-lookup"><span data-stu-id="9f378-120">Name</span></span>       | <span data-ttu-id="9f378-121">Typ</span><span class="sxs-lookup"><span data-stu-id="9f378-121">Type</span></span> | <span data-ttu-id="9f378-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f378-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9f378-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f378-123">Authorization</span></span>  | <span data-ttu-id="9f378-124">string</span><span class="sxs-lookup"><span data-stu-id="9f378-124">string</span></span>  | <span data-ttu-id="9f378-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f378-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f378-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f378-127">Request body</span></span>
<span data-ttu-id="9f378-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9f378-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f378-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f378-129">Response</span></span>

<span data-ttu-id="9f378-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryRoleTemplate](../resources/directoryroletemplate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f378-130">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f378-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f378-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f378-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f378-132">Request</span></span>
<span data-ttu-id="9f378-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f378-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="9f378-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f378-134">Response</span></span>
<span data-ttu-id="9f378-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f378-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "description": "description-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
