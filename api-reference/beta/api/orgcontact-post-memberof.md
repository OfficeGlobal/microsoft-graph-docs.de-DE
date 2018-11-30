---
title: Erstellen von Mitglied
description: Verwenden Sie diese API, um ein neues Mitglied zu erstellen.
ms.openlocfilehash: f753f2e8f14fb60eb23b10512506bfe6e3b95bdd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063306"
---
# <a name="create-memberof"></a><span data-ttu-id="443fe-103">Erstellen von Mitglied</span><span class="sxs-lookup"><span data-stu-id="443fe-103">Create memberOf</span></span>

> <span data-ttu-id="443fe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="443fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="443fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="443fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="443fe-106">Verwenden Sie diese API, um ein neues Mitglied zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="443fe-106">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="443fe-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="443fe-107">Permissions</span></span>
<span data-ttu-id="443fe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="443fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="443fe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="443fe-110">Permission type</span></span>      | <span data-ttu-id="443fe-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="443fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="443fe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="443fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="443fe-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="443fe-113">Not supported.</span></span>    |
|<span data-ttu-id="443fe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="443fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="443fe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="443fe-115">Not supported.</span></span>    |
|<span data-ttu-id="443fe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="443fe-116">Application</span></span> | <span data-ttu-id="443fe-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="443fe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="443fe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="443fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="443fe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="443fe-119">Request headers</span></span>
| <span data-ttu-id="443fe-120">Name</span><span class="sxs-lookup"><span data-stu-id="443fe-120">Name</span></span>       | <span data-ttu-id="443fe-121">Typ</span><span class="sxs-lookup"><span data-stu-id="443fe-121">Type</span></span> | <span data-ttu-id="443fe-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="443fe-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="443fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="443fe-123">Authorization</span></span>  | <span data-ttu-id="443fe-124">string</span><span class="sxs-lookup"><span data-stu-id="443fe-124">string</span></span>  | <span data-ttu-id="443fe-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="443fe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="443fe-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="443fe-127">Request body</span></span>
<span data-ttu-id="443fe-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="443fe-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="443fe-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="443fe-129">Response</span></span>

<span data-ttu-id="443fe-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="443fe-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="443fe-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="443fe-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="443fe-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="443fe-132">Request</span></span>
<span data-ttu-id="443fe-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="443fe-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="443fe-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="443fe-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="443fe-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="443fe-135">Response</span></span>
<span data-ttu-id="443fe-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="443fe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->