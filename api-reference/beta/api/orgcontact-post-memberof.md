---
title: Erstellen von Mitglied
description: Verwenden Sie diese API, um ein neues Mitglied zu erstellen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ca5aa856f1f2e64f3a3b73ccff15f686c048cfda
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970003"
---
# <a name="create-memberof"></a><span data-ttu-id="5e2e0-103">Erstellen von Mitglied</span><span class="sxs-lookup"><span data-stu-id="5e2e0-103">Create memberOf</span></span>

> <span data-ttu-id="5e2e0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5e2e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e2e0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5e2e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e2e0-106">Verwenden Sie diese API, um ein neues Mitglied zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="5e2e0-106">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e2e0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5e2e0-107">Permissions</span></span>
<span data-ttu-id="5e2e0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e2e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e2e0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5e2e0-110">Permission type</span></span>      | <span data-ttu-id="5e2e0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5e2e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e2e0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5e2e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5e2e0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e2e0-113">Not supported.</span></span>    |
|<span data-ttu-id="5e2e0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5e2e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e2e0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e2e0-115">Not supported.</span></span>    |
|<span data-ttu-id="5e2e0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5e2e0-116">Application</span></span> | <span data-ttu-id="5e2e0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e2e0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e2e0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e2e0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="5e2e0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5e2e0-119">Request headers</span></span>
| <span data-ttu-id="5e2e0-120">Name</span><span class="sxs-lookup"><span data-stu-id="5e2e0-120">Name</span></span>       | <span data-ttu-id="5e2e0-121">Typ</span><span class="sxs-lookup"><span data-stu-id="5e2e0-121">Type</span></span> | <span data-ttu-id="5e2e0-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e2e0-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5e2e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e2e0-123">Authorization</span></span>  | <span data-ttu-id="5e2e0-124">string</span><span class="sxs-lookup"><span data-stu-id="5e2e0-124">string</span></span>  | <span data-ttu-id="5e2e0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5e2e0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e2e0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5e2e0-127">Request body</span></span>
<span data-ttu-id="5e2e0-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5e2e0-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5e2e0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e2e0-129">Response</span></span>

<span data-ttu-id="5e2e0-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5e2e0-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e2e0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5e2e0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e2e0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e2e0-132">Request</span></span>
<span data-ttu-id="5e2e0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5e2e0-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="5e2e0-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5e2e0-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5e2e0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e2e0-135">Response</span></span>
<span data-ttu-id="5e2e0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5e2e0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
