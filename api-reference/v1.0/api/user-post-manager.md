---
title: Einen Vorgesetzten zuweisen
description: Verwenden Sie diese API, um den Vorgesetzten eines Benutzers zuzuweisen.
ms.openlocfilehash: ab48d0546b533fcc137d31cdc889072abf48fcfe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018088"
---
# <a name="assign-a-manager"></a><span data-ttu-id="cdfd4-103">Einen Vorgesetzten zuweisen</span><span class="sxs-lookup"><span data-stu-id="cdfd4-103">Assign a manager</span></span>

<span data-ttu-id="cdfd4-104">Verwenden Sie diese API, um den Vorgesetzten eines Benutzers zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="cdfd4-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="cdfd4-105">Hinweis: Es ist nicht möglich, direkte Unterstellte zuzuweisen, verwenden Sie stattdessen diese API.</span><span class="sxs-lookup"><span data-stu-id="cdfd4-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdfd4-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cdfd4-106">Permissions</span></span>
<span data-ttu-id="cdfd4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdfd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdfd4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cdfd4-109">Permission type</span></span>      | <span data-ttu-id="cdfd4-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cdfd4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdfd4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cdfd4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cdfd4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cdfd4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cdfd4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cdfd4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdfd4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cdfd4-114">Not supported.</span></span>    |
|<span data-ttu-id="cdfd4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cdfd4-115">Application</span></span> | <span data-ttu-id="cdfd4-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdfd4-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdfd4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cdfd4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="cdfd4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cdfd4-118">Request headers</span></span>
| <span data-ttu-id="cdfd4-119">Name</span><span class="sxs-lookup"><span data-stu-id="cdfd4-119">Name</span></span>       | <span data-ttu-id="cdfd4-120">Typ</span><span class="sxs-lookup"><span data-stu-id="cdfd4-120">Type</span></span> | <span data-ttu-id="cdfd4-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cdfd4-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cdfd4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdfd4-122">Authorization</span></span>  | <span data-ttu-id="cdfd4-123">string</span><span class="sxs-lookup"><span data-stu-id="cdfd4-123">string</span></span>  | <span data-ttu-id="cdfd4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cdfd4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdfd4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cdfd4-126">Request body</span></span>
<span data-ttu-id="cdfd4-127">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="cdfd4-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="cdfd4-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="cdfd4-128">Response</span></span>

<span data-ttu-id="cdfd4-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cdfd4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdfd4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cdfd4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdfd4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cdfd4-132">Request</span></span>
<span data-ttu-id="cdfd4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cdfd4-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="cdfd4-134">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="cdfd4-134">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="cdfd4-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cdfd4-135">Response</span></span>
<span data-ttu-id="cdfd4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cdfd4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
