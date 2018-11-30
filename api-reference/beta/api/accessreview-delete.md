---
title: AccessReview löschen
description: In Azure AD zugreifen auf Berichte-Funktion, löschen Sie ein AccessReview-Objekt zu.
ms.openlocfilehash: b9578b575705de909eca99ac70f5efbb70d053cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059341"
---
# <a name="delete-accessreview"></a><span data-ttu-id="e72b8-103">AccessReview löschen</span><span class="sxs-lookup"><span data-stu-id="e72b8-103">Delete accessReview</span></span>

> <span data-ttu-id="e72b8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e72b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e72b8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e72b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e72b8-106">Löschen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion ein [AccessReview](../resources/accessreview.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="e72b8-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e72b8-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e72b8-107">Permissions</span></span>
<span data-ttu-id="e72b8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e72b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e72b8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e72b8-110">Permission type</span></span>                        | <span data-ttu-id="e72b8-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e72b8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e72b8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e72b8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e72b8-113">AccessReview.ReadWrite.All, und sollten auch ProgramControl.ReadWrite.All vollständige Szenario mit einem Aufruf einer ProgramControl löschen</span><span class="sxs-lookup"><span data-stu-id="e72b8-113">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with a call to delete a programControl</span></span> |
|<span data-ttu-id="e72b8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e72b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e72b8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e72b8-115">Not supported.</span></span> |
|<span data-ttu-id="e72b8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e72b8-116">Application</span></span>                            | <span data-ttu-id="e72b8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e72b8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e72b8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e72b8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="e72b8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e72b8-119">Request headers</span></span>
| <span data-ttu-id="e72b8-120">Name</span><span class="sxs-lookup"><span data-stu-id="e72b8-120">Name</span></span>         | <span data-ttu-id="e72b8-121">Typ</span><span class="sxs-lookup"><span data-stu-id="e72b8-121">Type</span></span>        | <span data-ttu-id="e72b8-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e72b8-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e72b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e72b8-123">Authorization</span></span> | <span data-ttu-id="e72b8-124">string</span><span class="sxs-lookup"><span data-stu-id="e72b8-124">string</span></span> | <span data-ttu-id="e72b8-125">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="e72b8-125">Bearer \{token\}.</span></span> <span data-ttu-id="e72b8-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e72b8-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e72b8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e72b8-127">Request body</span></span>
<span data-ttu-id="e72b8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e72b8-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e72b8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e72b8-129">Response</span></span>
<span data-ttu-id="e72b8-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e72b8-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e72b8-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e72b8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e72b8-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e72b8-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')
```
##### <a name="response"></a><span data-ttu-id="e72b8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e72b8-134">Response</span></span>
><span data-ttu-id="e72b8-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e72b8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
