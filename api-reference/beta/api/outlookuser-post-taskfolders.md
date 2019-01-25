---
title: Erstellen von outlookTaskFolder
description: Erstellen Sie einen Aufgabenordner in der Standardgruppe Aufgabe (`My Tasks`) für das Postfach des Benutzers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 81c77d96b4d7c66cfbc7dde3481a7bfaa8cd6c5f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514446"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="04100-103">Erstellen von outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="04100-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04100-104">Erstellen Sie einen Aufgabenordner in der Standardgruppe Aufgabe (`My Tasks`) für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="04100-104">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="04100-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="04100-105">Permissions</span></span>
<span data-ttu-id="04100-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04100-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04100-108">Permission type</span></span>      | <span data-ttu-id="04100-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04100-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04100-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04100-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04100-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04100-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="04100-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04100-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04100-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04100-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="04100-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04100-114">Application</span></span> | <span data-ttu-id="04100-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04100-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04100-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04100-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="04100-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04100-117">Request headers</span></span>
| <span data-ttu-id="04100-118">Name</span><span class="sxs-lookup"><span data-stu-id="04100-118">Name</span></span>       | <span data-ttu-id="04100-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04100-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="04100-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="04100-120">Authorization</span></span>  | <span data-ttu-id="04100-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="04100-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04100-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04100-123">Request body</span></span>
<span data-ttu-id="04100-124">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTaskFolder](../resources/outlooktaskfolder.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="04100-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="04100-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="04100-125">Response</span></span>

<span data-ttu-id="04100-126">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [OutlookTaskFolder](../resources/outlooktaskfolder.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="04100-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04100-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04100-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04100-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04100-128">Request</span></span>
<span data-ttu-id="04100-129">Das folgende Beispiel erstellt einen Aufgabenordner freiwilliger in der Standardgruppe Task aufgerufen (`My Tasks`) für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="04100-129">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders 
Content-type: application/json
Content-length: 60

{
  "name": "Volunteer"
}
```
<span data-ttu-id="04100-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTaskFolder](../resources/outlooktaskfolder.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="04100-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="04100-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="04100-131">Response</span></span>
<span data-ttu-id="04100-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04100-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGig==",
  "isDefaultFolder": false,
  "name": "Volunteer",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
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
    "Error: /api-reference/beta/api/outlookuser-post-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
