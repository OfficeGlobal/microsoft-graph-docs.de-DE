---
title: Einen Vorgesetzten zuweisen
description: Verwenden Sie diese API, um den Vorgesetzten eines Benutzers zuzuweisen.
ms.openlocfilehash: b0e8c9f7c7aa30784497a333d9a92e52749ade73
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063487"
---
# <a name="assign-a-manager"></a><span data-ttu-id="71bab-103">Einen Vorgesetzten zuweisen</span><span class="sxs-lookup"><span data-stu-id="71bab-103">Assign a manager</span></span>

> <span data-ttu-id="71bab-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="71bab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71bab-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71bab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71bab-106">Verwenden Sie diese API, um den Vorgesetzten eines Benutzers zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="71bab-106">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="71bab-107">Hinweis: Es ist nicht möglich, direkte Unterstellte zuzuweisen, verwenden Sie stattdessen diese API.</span><span class="sxs-lookup"><span data-stu-id="71bab-107">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="71bab-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="71bab-108">Permissions</span></span>
<span data-ttu-id="71bab-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71bab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71bab-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71bab-111">Permission type</span></span>      | <span data-ttu-id="71bab-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71bab-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71bab-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71bab-113">Delegated (work or school account)</span></span> | <span data-ttu-id="71bab-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71bab-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71bab-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71bab-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71bab-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71bab-116">Not supported.</span></span>    |
|<span data-ttu-id="71bab-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71bab-117">Application</span></span> | <span data-ttu-id="71bab-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71bab-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71bab-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71bab-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="71bab-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71bab-120">Request headers</span></span>
| <span data-ttu-id="71bab-121">Name</span><span class="sxs-lookup"><span data-stu-id="71bab-121">Name</span></span>       | <span data-ttu-id="71bab-122">Typ</span><span class="sxs-lookup"><span data-stu-id="71bab-122">Type</span></span> | <span data-ttu-id="71bab-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71bab-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71bab-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="71bab-124">Authorization</span></span>  | <span data-ttu-id="71bab-125">string</span><span class="sxs-lookup"><span data-stu-id="71bab-125">string</span></span>  | <span data-ttu-id="71bab-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="71bab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71bab-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71bab-128">Request body</span></span>
<span data-ttu-id="71bab-129">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="71bab-129">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="71bab-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="71bab-130">Response</span></span>

<span data-ttu-id="71bab-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71bab-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71bab-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71bab-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71bab-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71bab-134">Request</span></span>
<span data-ttu-id="71bab-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71bab-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="71bab-136">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="71bab-136">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="71bab-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="71bab-137">Response</span></span>
<span data-ttu-id="71bab-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71bab-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
