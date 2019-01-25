---
title: inferenceClassificationOverride löschen
description: Löschen Sie eine praxisorientierte Posteingang Überschreibung durch seine ID angegebene
localization_priority: Normal
ms.openlocfilehash: 16298ebb02b0540272c0c858abf5b16759de824d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513830"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="0db0a-103">inferenceClassificationOverride löschen</span><span class="sxs-lookup"><span data-stu-id="0db0a-103">Delete inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0db0a-104">Löschen Sie eine [Praxisorientierte Posteingang](../resources/manage-focused-inbox.md) Überschreibung durch seine ID angegebene</span><span class="sxs-lookup"><span data-stu-id="0db0a-104">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="0db0a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0db0a-105">Permissions</span></span>
<span data-ttu-id="0db0a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0db0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0db0a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0db0a-108">Permission type</span></span>      | <span data-ttu-id="0db0a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0db0a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0db0a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0db0a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0db0a-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0db0a-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0db0a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0db0a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0db0a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0db0a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0db0a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0db0a-114">Application</span></span> | <span data-ttu-id="0db0a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0db0a-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0db0a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0db0a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0db0a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0db0a-117">Request headers</span></span>
| <span data-ttu-id="0db0a-118">Name</span><span class="sxs-lookup"><span data-stu-id="0db0a-118">Name</span></span>       | <span data-ttu-id="0db0a-119">Typ</span><span class="sxs-lookup"><span data-stu-id="0db0a-119">Type</span></span> | <span data-ttu-id="0db0a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0db0a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0db0a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0db0a-121">Authorization</span></span>  | <span data-ttu-id="0db0a-122">string</span><span class="sxs-lookup"><span data-stu-id="0db0a-122">string</span></span>  | <span data-ttu-id="0db0a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0db0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0db0a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0db0a-125">Request body</span></span>
<span data-ttu-id="0db0a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0db0a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0db0a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0db0a-127">Response</span></span>

<span data-ttu-id="0db0a-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0db0a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0db0a-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0db0a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0db0a-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0db0a-131">Request</span></span>
<span data-ttu-id="0db0a-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0db0a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="0db0a-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="0db0a-133">Response</span></span>
<span data-ttu-id="0db0a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0db0a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/inferenceclassificationoverride-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
