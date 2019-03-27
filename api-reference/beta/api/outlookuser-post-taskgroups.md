---
title: Outlook Task Group erstellen
description: Erstellen Sie eine Outlook-Aufgabengruppe im Postfach des Benutzers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 364510c3d866b193012763d17dbc22f2e1d7c8f7
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869260"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="50172-103">Outlook Task Group erstellen</span><span class="sxs-lookup"><span data-stu-id="50172-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50172-104">Erstellen Sie eine Outlook-Aufgabengruppe im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="50172-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="50172-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="50172-105">Permissions</span></span>
<span data-ttu-id="50172-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50172-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50172-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50172-108">Permission type</span></span>      | <span data-ttu-id="50172-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50172-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50172-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50172-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50172-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50172-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="50172-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50172-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50172-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50172-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="50172-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50172-114">Application</span></span> | <span data-ttu-id="50172-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50172-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50172-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50172-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="50172-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50172-117">Request headers</span></span>
| <span data-ttu-id="50172-118">Name</span><span class="sxs-lookup"><span data-stu-id="50172-118">Name</span></span>       | <span data-ttu-id="50172-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50172-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="50172-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="50172-120">Authorization</span></span>  | <span data-ttu-id="50172-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="50172-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50172-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50172-123">Request body</span></span>
<span data-ttu-id="50172-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [Outlook Task Group](../resources/outlooktaskgroup.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="50172-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="50172-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="50172-125">Response</span></span>

<span data-ttu-id="50172-126">Bei erfolgreicher Ausführung gibt diese Methode `201 Created` den Antwortcode und das [Outlook Task Group](../resources/outlooktaskgroup.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="50172-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50172-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50172-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50172-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50172-128">Request</span></span>
<span data-ttu-id="50172-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50172-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="50172-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [Outlook Task Group](../resources/outlooktaskgroup.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="50172-130">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="50172-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="50172-131">Response</span></span>
<span data-ttu-id="50172-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50172-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-taskgroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
