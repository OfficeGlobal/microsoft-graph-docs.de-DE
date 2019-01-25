---
title: Erstellen von Mitglied
description: Verwenden Sie diese API, um ein neues Mitglied zu erstellen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 466074d2d23dc4b991c8c153252028587fd5afcc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518919"
---
# <a name="create-memberof"></a><span data-ttu-id="b1fa0-103">Erstellen von Mitglied</span><span class="sxs-lookup"><span data-stu-id="b1fa0-103">Create memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1fa0-104">Verwenden Sie diese API, um ein neues Mitglied zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="b1fa0-104">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1fa0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b1fa0-105">Permissions</span></span>
<span data-ttu-id="b1fa0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1fa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1fa0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1fa0-108">Permission type</span></span>      | <span data-ttu-id="b1fa0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1fa0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1fa0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1fa0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1fa0-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1fa0-111">Not supported.</span></span>    |
|<span data-ttu-id="b1fa0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1fa0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1fa0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1fa0-113">Not supported.</span></span>    |
|<span data-ttu-id="b1fa0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1fa0-114">Application</span></span> | <span data-ttu-id="b1fa0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1fa0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1fa0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1fa0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="b1fa0-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1fa0-117">Request headers</span></span>
| <span data-ttu-id="b1fa0-118">Name</span><span class="sxs-lookup"><span data-stu-id="b1fa0-118">Name</span></span>       | <span data-ttu-id="b1fa0-119">Typ</span><span class="sxs-lookup"><span data-stu-id="b1fa0-119">Type</span></span> | <span data-ttu-id="b1fa0-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1fa0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b1fa0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1fa0-121">Authorization</span></span>  | <span data-ttu-id="b1fa0-122">string</span><span class="sxs-lookup"><span data-stu-id="b1fa0-122">string</span></span>  | <span data-ttu-id="b1fa0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b1fa0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1fa0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1fa0-125">Request body</span></span>
<span data-ttu-id="b1fa0-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b1fa0-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b1fa0-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1fa0-127">Response</span></span>

<span data-ttu-id="b1fa0-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1fa0-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1fa0-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1fa0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1fa0-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1fa0-130">Request</span></span>
<span data-ttu-id="b1fa0-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1fa0-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/memberOf
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="b1fa0-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b1fa0-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b1fa0-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1fa0-133">Response</span></span>
<span data-ttu-id="b1fa0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1fa0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-post-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
