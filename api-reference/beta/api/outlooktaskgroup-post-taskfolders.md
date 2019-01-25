---
title: Erstellen von outlookTaskFolder
description: Erstellen eines Outlook-Aufgabenordner unter einer angegebenen OutlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 734be5578f6319307fabcac9c4e4b591b575858e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529957"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="18af7-103">Erstellen von outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="18af7-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18af7-104">Erstellen eines Outlook-Aufgabenordner unter einer angegebenen [OutlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="18af7-104">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="18af7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18af7-105">Permissions</span></span>
<span data-ttu-id="18af7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18af7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18af7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18af7-108">Permission type</span></span>      | <span data-ttu-id="18af7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18af7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18af7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18af7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18af7-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18af7-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="18af7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18af7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18af7-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18af7-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="18af7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18af7-114">Application</span></span> | <span data-ttu-id="18af7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18af7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18af7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18af7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="18af7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18af7-117">Request headers</span></span>
| <span data-ttu-id="18af7-118">Name</span><span class="sxs-lookup"><span data-stu-id="18af7-118">Name</span></span>       | <span data-ttu-id="18af7-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18af7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="18af7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="18af7-120">Authorization</span></span>  | <span data-ttu-id="18af7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18af7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18af7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18af7-123">Request body</span></span>
<span data-ttu-id="18af7-124">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTaskFolder](../resources/outlooktaskfolder.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="18af7-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="18af7-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="18af7-125">Response</span></span>

<span data-ttu-id="18af7-126">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [OutlookTaskFolder](../resources/outlooktaskfolder.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="18af7-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18af7-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18af7-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18af7-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18af7-128">Request</span></span>
<span data-ttu-id="18af7-129">Das folgende Beispiel erstellt einen Ordner mit dem Vorgang `Cooking` in der Gruppe angegebenen Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="18af7-129">The following example creates a task folder called `Cooking` in the specified task group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskgroups('AAMkADIyAAAhrbe-AAA')/taskfolders 

Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```
<span data-ttu-id="18af7-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTaskFolder](../resources/outlooktaskfolder.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="18af7-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="18af7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="18af7-131">Response</span></span>
<span data-ttu-id="18af7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18af7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPXAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
  "isDefaultFolder": false,
  "name": "Cooking",
  "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-post-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
