---
title: Einen Vorgesetzten zuweisen
description: Verwenden Sie diese API, um den Vorgesetzten eines Benutzers zuzuweisen.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 356c78fb41f641a0736a83ae05e64ad4696921fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931692"
---
# <a name="assign-a-manager"></a><span data-ttu-id="5da01-103">Einen Vorgesetzten zuweisen</span><span class="sxs-lookup"><span data-stu-id="5da01-103">Assign a manager</span></span>

<span data-ttu-id="5da01-104">Verwenden Sie diese API, um den Vorgesetzten eines Benutzers zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="5da01-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="5da01-105">Hinweis: Es ist nicht möglich, direkte Unterstellte zuzuweisen, verwenden Sie stattdessen diese API.</span><span class="sxs-lookup"><span data-stu-id="5da01-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="5da01-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5da01-106">Permissions</span></span>
<span data-ttu-id="5da01-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5da01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5da01-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5da01-109">Permission type</span></span>      | <span data-ttu-id="5da01-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5da01-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5da01-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5da01-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5da01-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5da01-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5da01-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5da01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5da01-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5da01-114">Not supported.</span></span>    |
|<span data-ttu-id="5da01-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5da01-115">Application</span></span> | <span data-ttu-id="5da01-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da01-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5da01-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5da01-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5da01-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5da01-118">Request headers</span></span>
| <span data-ttu-id="5da01-119">Name</span><span class="sxs-lookup"><span data-stu-id="5da01-119">Name</span></span>       | <span data-ttu-id="5da01-120">Typ</span><span class="sxs-lookup"><span data-stu-id="5da01-120">Type</span></span> | <span data-ttu-id="5da01-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5da01-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5da01-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5da01-122">Authorization</span></span>  | <span data-ttu-id="5da01-123">string</span><span class="sxs-lookup"><span data-stu-id="5da01-123">string</span></span>  | <span data-ttu-id="5da01-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5da01-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5da01-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5da01-126">Request body</span></span>
<span data-ttu-id="5da01-127">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="5da01-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="5da01-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="5da01-128">Response</span></span>

<span data-ttu-id="5da01-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5da01-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5da01-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5da01-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5da01-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5da01-132">Request</span></span>
<span data-ttu-id="5da01-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5da01-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="5da01-134">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="5da01-134">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="5da01-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5da01-135">Response</span></span>
<span data-ttu-id="5da01-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5da01-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
