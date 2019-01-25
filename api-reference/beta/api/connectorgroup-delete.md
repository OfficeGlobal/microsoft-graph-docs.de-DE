---
title: ConnectorGroup löschen
description: Löschen einer ConnectorGroup.
localization_priority: Normal
ms.openlocfilehash: a0fd138281b8337df49388f4a10dc34cc02da18d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516028"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="5d619-103">ConnectorGroup löschen</span><span class="sxs-lookup"><span data-stu-id="5d619-103">Delete connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d619-104">Löschen einer ConnectorGroup.</span><span class="sxs-lookup"><span data-stu-id="5d619-104">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d619-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5d619-105">Permissions</span></span>
<span data-ttu-id="5d619-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d619-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5d619-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d619-108">Permission type</span></span>      | <span data-ttu-id="5d619-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d619-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d619-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d619-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5d619-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d619-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5d619-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d619-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d619-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d619-113">Not supported.</span></span>    |
|<span data-ttu-id="5d619-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d619-114">Application</span></span> | <span data-ttu-id="5d619-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d619-115">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="5d619-116">**Hinweis:** Die Gruppe Connectors darf keine Connectors zugeordnet haben.</span><span class="sxs-lookup"><span data-stu-id="5d619-116">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="5d619-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d619-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5d619-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d619-118">Request headers</span></span>
| <span data-ttu-id="5d619-119">Name</span><span class="sxs-lookup"><span data-stu-id="5d619-119">Name</span></span>       | <span data-ttu-id="5d619-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d619-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5d619-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d619-121">Authorization</span></span>  | <span data-ttu-id="5d619-122">Bearer </span><span class="sxs-lookup"><span data-stu-id="5d619-122">Bearer.</span></span> <span data-ttu-id="5d619-123">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="5d619-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d619-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d619-124">Request body</span></span>
<span data-ttu-id="5d619-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5d619-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d619-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d619-126">Response</span></span>

<span data-ttu-id="5d619-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d619-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d619-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d619-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d619-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d619-130">Request</span></span>
<span data-ttu-id="5d619-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d619-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="5d619-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d619-132">Response</span></span>
<span data-ttu-id="5d619-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d619-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
