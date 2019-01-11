---
title: Erstellen von outlookTaskFolder
description: Erstellen eines Outlook-Aufgabenordner unter einer angegebenen OutlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 4d6d6f103c1dd002f4c01e0dbdd71d1ebd7ddd10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823835"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="dd84e-103">Erstellen von outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="dd84e-103">Create outlookTaskFolder</span></span>

> <span data-ttu-id="dd84e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd84e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd84e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd84e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd84e-106">Erstellen eines Outlook-Aufgabenordner unter einer angegebenen [OutlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="dd84e-106">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="dd84e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dd84e-107">Permissions</span></span>
<span data-ttu-id="dd84e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd84e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd84e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd84e-110">Permission type</span></span>      | <span data-ttu-id="dd84e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd84e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd84e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd84e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dd84e-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd84e-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dd84e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd84e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd84e-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd84e-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dd84e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd84e-116">Application</span></span> | <span data-ttu-id="dd84e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd84e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd84e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd84e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="dd84e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd84e-119">Request headers</span></span>
| <span data-ttu-id="dd84e-120">Name</span><span class="sxs-lookup"><span data-stu-id="dd84e-120">Name</span></span>       | <span data-ttu-id="dd84e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd84e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dd84e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd84e-122">Authorization</span></span>  | <span data-ttu-id="dd84e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dd84e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd84e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd84e-125">Request body</span></span>
<span data-ttu-id="dd84e-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTaskFolder](../resources/outlooktaskfolder.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd84e-126">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dd84e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd84e-127">Response</span></span>

<span data-ttu-id="dd84e-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [OutlookTaskFolder](../resources/outlooktaskfolder.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dd84e-128">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd84e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd84e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd84e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd84e-130">Request</span></span>
<span data-ttu-id="dd84e-131">Das folgende Beispiel erstellt einen Ordner mit dem Vorgang `Cooking` in der Gruppe angegebenen Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="dd84e-131">The following example creates a task folder called `Cooking` in the specified task group.</span></span>
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
<span data-ttu-id="dd84e-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTaskFolder](../resources/outlooktaskfolder.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd84e-132">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dd84e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd84e-133">Response</span></span>
<span data-ttu-id="dd84e-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd84e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
