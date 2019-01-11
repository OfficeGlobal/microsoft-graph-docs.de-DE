---
title: Erstellen von outlookTaskGroup
description: Erstellen eines Outlook-"Task Group" im Postfach des Benutzers an.
localization_priority: Normal
ms.openlocfilehash: 2640d540c3b5f81c14763f785c565268bb15d689
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851912"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="64ffc-103">Erstellen von outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="64ffc-103">Create outlookTaskGroup</span></span>

> <span data-ttu-id="64ffc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="64ffc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64ffc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64ffc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64ffc-106">Erstellen eines Outlook-"Task Group" im Postfach des Benutzers an.</span><span class="sxs-lookup"><span data-stu-id="64ffc-106">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="64ffc-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="64ffc-107">Permissions</span></span>
<span data-ttu-id="64ffc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64ffc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64ffc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64ffc-110">Permission type</span></span>      | <span data-ttu-id="64ffc-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64ffc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64ffc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64ffc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="64ffc-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64ffc-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="64ffc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64ffc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64ffc-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64ffc-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="64ffc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64ffc-116">Application</span></span> | <span data-ttu-id="64ffc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64ffc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64ffc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64ffc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups

```
## <a name="request-headers"></a><span data-ttu-id="64ffc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64ffc-119">Request headers</span></span>
| <span data-ttu-id="64ffc-120">Name</span><span class="sxs-lookup"><span data-stu-id="64ffc-120">Name</span></span>       | <span data-ttu-id="64ffc-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64ffc-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64ffc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64ffc-122">Authorization</span></span>  | <span data-ttu-id="64ffc-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="64ffc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64ffc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64ffc-125">Request body</span></span>
<span data-ttu-id="64ffc-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTaskGroup](../resources/outlooktaskgroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="64ffc-126">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="64ffc-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="64ffc-127">Response</span></span>

<span data-ttu-id="64ffc-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [OutlookTaskGroup](../resources/outlooktaskgroup.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="64ffc-128">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64ffc-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64ffc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64ffc-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64ffc-130">Request</span></span>
<span data-ttu-id="64ffc-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64ffc-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="64ffc-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTaskGroup](../resources/outlooktaskgroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="64ffc-132">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="64ffc-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="64ffc-133">Response</span></span>
<span data-ttu-id="64ffc-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64ffc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
