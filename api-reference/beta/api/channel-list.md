---
title: Kanäle auflisten
description: Abrufen der Liste von Kanälen in diesem Team.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 47e284bb5eb89c88a961dc82f802fd6eac083310
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527759"
---
# <a name="list-channels"></a><span data-ttu-id="c2e6b-103">Kanäle auflisten</span><span class="sxs-lookup"><span data-stu-id="c2e6b-103">List channels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2e6b-104">Abrufen der Liste von [Kanälen](../resources/channel.md) in diesem Team.</span><span class="sxs-lookup"><span data-stu-id="c2e6b-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2e6b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c2e6b-105">Permissions</span></span>
<span data-ttu-id="c2e6b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2e6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c2e6b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c2e6b-108">Permission type</span></span>      | <span data-ttu-id="c2e6b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c2e6b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2e6b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c2e6b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2e6b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2e6b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2e6b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c2e6b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2e6b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2e6b-113">Not supported.</span></span>    |
|<span data-ttu-id="c2e6b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c2e6b-114">Application</span></span> | <span data-ttu-id="c2e6b-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2e6b-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="c2e6b-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="c2e6b-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c2e6b-117">Globale Administratoren und Microsoft Teams-Dienstadministratoren können auf Teams zugreifen, in denen sie kein Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="c2e6b-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c2e6b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2e6b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2e6b-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c2e6b-119">Optional query parameters</span></span>
<span data-ttu-id="c2e6b-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) $filter, $select und $expand zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c2e6b-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2e6b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c2e6b-121">Request headers</span></span>
| <span data-ttu-id="c2e6b-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c2e6b-122">Header</span></span>       | <span data-ttu-id="c2e6b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c2e6b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c2e6b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2e6b-124">Authorization</span></span>  | <span data-ttu-id="c2e6b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c2e6b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2e6b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c2e6b-127">Request body</span></span>
<span data-ttu-id="c2e6b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c2e6b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2e6b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2e6b-129">Response</span></span>

<span data-ttu-id="c2e6b-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Channel](../resources/channel.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c2e6b-130">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2e6b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c2e6b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2e6b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2e6b-132">Request</span></span>
<span data-ttu-id="c2e6b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c2e6b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="c2e6b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2e6b-134">Response</span></span>
<span data-ttu-id="c2e6b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c2e6b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
