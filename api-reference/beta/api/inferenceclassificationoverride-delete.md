---
title: inferenceClassificationOverride löschen
description: Löschen Sie eine praxisorientierte Posteingang Überschreibung durch seine ID angegebene
localization_priority: Normal
ms.openlocfilehash: 7db351e11ccfa8e88fe97ff1ee22173a87242d57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870140"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="0ab36-103">inferenceClassificationOverride löschen</span><span class="sxs-lookup"><span data-stu-id="0ab36-103">Delete inferenceClassificationOverride</span></span>

> <span data-ttu-id="0ab36-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0ab36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ab36-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ab36-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ab36-106">Löschen Sie eine [Praxisorientierte Posteingang](../resources/manage-focused-inbox.md) Überschreibung durch seine ID angegebene</span><span class="sxs-lookup"><span data-stu-id="0ab36-106">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ab36-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0ab36-107">Permissions</span></span>
<span data-ttu-id="0ab36-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ab36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ab36-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0ab36-110">Permission type</span></span>      | <span data-ttu-id="0ab36-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0ab36-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ab36-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0ab36-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0ab36-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ab36-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0ab36-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0ab36-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ab36-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ab36-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0ab36-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0ab36-116">Application</span></span> | <span data-ttu-id="0ab36-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ab36-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ab36-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ab36-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0ab36-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ab36-119">Request headers</span></span>
| <span data-ttu-id="0ab36-120">Name</span><span class="sxs-lookup"><span data-stu-id="0ab36-120">Name</span></span>       | <span data-ttu-id="0ab36-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0ab36-121">Type</span></span> | <span data-ttu-id="0ab36-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ab36-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ab36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ab36-123">Authorization</span></span>  | <span data-ttu-id="0ab36-124">string</span><span class="sxs-lookup"><span data-stu-id="0ab36-124">string</span></span>  | <span data-ttu-id="0ab36-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0ab36-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ab36-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0ab36-127">Request body</span></span>
<span data-ttu-id="0ab36-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0ab36-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ab36-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ab36-129">Response</span></span>

<span data-ttu-id="0ab36-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ab36-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ab36-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ab36-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ab36-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ab36-133">Request</span></span>
<span data-ttu-id="0ab36-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0ab36-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="0ab36-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ab36-135">Response</span></span>
<span data-ttu-id="0ab36-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ab36-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
