---
title: Patch-Kanal
description: Aktualisieren Sie die Eigenschaften des angegebenen Kanals.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f48ca862ba1c058544ead2a21c07f64275f5c5d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528193"
---
# <a name="patch-channel"></a><span data-ttu-id="98080-103">Patch-Kanal</span><span class="sxs-lookup"><span data-stu-id="98080-103">Patch channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98080-104">Aktualisieren Sie die Eigenschaften des angegebenen [DDE-Kanal](../resources/channel.md)an.</span><span class="sxs-lookup"><span data-stu-id="98080-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="98080-105">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="98080-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="98080-106">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="98080-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="98080-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="98080-107">Permissions</span></span>
<span data-ttu-id="98080-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98080-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98080-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="98080-110">Permission type</span></span>      | <span data-ttu-id="98080-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="98080-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98080-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="98080-112">Delegated (work or school account)</span></span> | <span data-ttu-id="98080-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98080-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="98080-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="98080-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98080-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98080-115">Not supported.</span></span>    |
|<span data-ttu-id="98080-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="98080-116">Application</span></span> | <span data-ttu-id="98080-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98080-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="98080-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="98080-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="98080-119">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="98080-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="98080-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="98080-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="98080-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="98080-121">Request headers</span></span>
| <span data-ttu-id="98080-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="98080-122">Header</span></span>       | <span data-ttu-id="98080-123">Wert</span><span class="sxs-lookup"><span data-stu-id="98080-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98080-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="98080-124">Authorization</span></span>  | <span data-ttu-id="98080-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="98080-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="98080-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="98080-127">Content-Type</span></span>  | <span data-ttu-id="98080-128">application/json</span><span class="sxs-lookup"><span data-stu-id="98080-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98080-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="98080-129">Request body</span></span>
<span data-ttu-id="98080-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Channel](../resources/channel.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="98080-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="98080-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="98080-131">Response</span></span>

<span data-ttu-id="98080-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="98080-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="98080-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="98080-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98080-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="98080-134">Request</span></span>
<span data-ttu-id="98080-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="98080-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="98080-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="98080-136">Response</span></span>
<span data-ttu-id="98080-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="98080-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-patch.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
