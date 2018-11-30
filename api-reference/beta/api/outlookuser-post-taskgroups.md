---
title: Erstellen von outlookTaskGroup
description: Erstellen eines Outlook-"Task Group" im Postfach des Benutzers an.
ms.openlocfilehash: dc3efc7b663d5eab3d9165b1d72fec5dd187db53
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066068"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="44fa8-103">Erstellen von outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="44fa8-103">Create outlookTaskGroup</span></span>

> <span data-ttu-id="44fa8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="44fa8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44fa8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44fa8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44fa8-106">Erstellen eines Outlook-"Task Group" im Postfach des Benutzers an.</span><span class="sxs-lookup"><span data-stu-id="44fa8-106">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="44fa8-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="44fa8-107">Permissions</span></span>
<span data-ttu-id="44fa8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44fa8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44fa8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44fa8-110">Permission type</span></span>      | <span data-ttu-id="44fa8-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44fa8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44fa8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44fa8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="44fa8-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44fa8-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="44fa8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44fa8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44fa8-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44fa8-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="44fa8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44fa8-116">Application</span></span> | <span data-ttu-id="44fa8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44fa8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44fa8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44fa8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups

```
## <a name="request-headers"></a><span data-ttu-id="44fa8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44fa8-119">Request headers</span></span>
| <span data-ttu-id="44fa8-120">Name</span><span class="sxs-lookup"><span data-stu-id="44fa8-120">Name</span></span>       | <span data-ttu-id="44fa8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44fa8-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="44fa8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="44fa8-122">Authorization</span></span>  | <span data-ttu-id="44fa8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="44fa8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44fa8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44fa8-125">Request body</span></span>
<span data-ttu-id="44fa8-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTaskGroup](../resources/outlooktaskgroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="44fa8-126">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="44fa8-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="44fa8-127">Response</span></span>

<span data-ttu-id="44fa8-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [OutlookTaskGroup](../resources/outlooktaskgroup.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="44fa8-128">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44fa8-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44fa8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44fa8-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44fa8-130">Request</span></span>
<span data-ttu-id="44fa8-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44fa8-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskGroups
Content-type: application/json
Content-length: 40

{
  "name": "Leisure tasks"
}
```
<span data-ttu-id="44fa8-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTaskGroup](../resources/outlooktaskgroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="44fa8-132">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="44fa8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="44fa8-133">Response</span></span>
<span data-ttu-id="44fa8-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44fa8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjg==",
  "isDefaultGroup": false,
  "name": "Leisure tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->