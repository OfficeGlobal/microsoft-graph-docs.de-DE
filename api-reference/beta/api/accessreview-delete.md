---
title: AccessReview löschen
description: In Azure AD zugreifen auf Berichte-Funktion, löschen Sie ein AccessReview-Objekt zu.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 28848cc047306259248d0ba4663ab3eb3e964224
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527773"
---
# <a name="delete-accessreview"></a><span data-ttu-id="0b4d3-103">AccessReview löschen</span><span class="sxs-lookup"><span data-stu-id="0b4d3-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b4d3-104">Löschen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion ein [AccessReview](../resources/accessreview.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="0b4d3-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b4d3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0b4d3-105">Permissions</span></span>
<span data-ttu-id="0b4d3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b4d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b4d3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b4d3-108">Permission type</span></span>                        | <span data-ttu-id="0b4d3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b4d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b4d3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b4d3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b4d3-111">AccessReview.ReadWrite.All, und sollten auch ProgramControl.ReadWrite.All vollständige Szenario mit einem Aufruf einer ProgramControl löschen</span><span class="sxs-lookup"><span data-stu-id="0b4d3-111">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with a call to delete a programControl</span></span> |
|<span data-ttu-id="0b4d3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b4d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b4d3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b4d3-113">Not supported.</span></span> |
|<span data-ttu-id="0b4d3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b4d3-114">Application</span></span>                            | <span data-ttu-id="0b4d3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b4d3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b4d3-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b4d3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="0b4d3-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b4d3-117">Request headers</span></span>
| <span data-ttu-id="0b4d3-118">Name</span><span class="sxs-lookup"><span data-stu-id="0b4d3-118">Name</span></span>         | <span data-ttu-id="0b4d3-119">Typ</span><span class="sxs-lookup"><span data-stu-id="0b4d3-119">Type</span></span>        | <span data-ttu-id="0b4d3-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b4d3-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0b4d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b4d3-121">Authorization</span></span> | <span data-ttu-id="0b4d3-122">string</span><span class="sxs-lookup"><span data-stu-id="0b4d3-122">string</span></span> | <span data-ttu-id="0b4d3-123">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="0b4d3-123">Bearer \{token\}.</span></span> <span data-ttu-id="0b4d3-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0b4d3-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b4d3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b4d3-125">Request body</span></span>
<span data-ttu-id="0b4d3-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0b4d3-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0b4d3-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b4d3-127">Response</span></span>
<span data-ttu-id="0b4d3-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b4d3-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b4d3-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b4d3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b4d3-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b4d3-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')
```
##### <a name="response"></a><span data-ttu-id="0b4d3-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b4d3-132">Response</span></span>
><span data-ttu-id="0b4d3-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0b4d3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
