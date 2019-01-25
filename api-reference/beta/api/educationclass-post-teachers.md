---
title: Lehrer hinzufügen
description: Hinzufügen eines Lehrers zu einer Klasse.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 959b873dba3f88665b170f52da4e4063adb200ae
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507803"
---
# <a name="add-teacher"></a><span data-ttu-id="7113c-103">Lehrer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="7113c-103">Add teacher</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7113c-104">Hinzufügen eines Lehrers zu einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="7113c-104">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="7113c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7113c-105">Permissions</span></span>
<span data-ttu-id="7113c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7113c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7113c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7113c-108">Permission type</span></span>      | <span data-ttu-id="7113c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7113c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7113c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7113c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7113c-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7113c-111">Not supported.</span></span>  |
|<span data-ttu-id="7113c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7113c-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7113c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7113c-113">Not supported.</span></span>  |
|<span data-ttu-id="7113c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7113c-114">Application</span></span> | <span data-ttu-id="7113c-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7113c-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7113c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7113c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7113c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7113c-117">Request headers</span></span>
| <span data-ttu-id="7113c-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7113c-118">Header</span></span>       | <span data-ttu-id="7113c-119">Wert</span><span class="sxs-lookup"><span data-stu-id="7113c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7113c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7113c-120">Authorization</span></span>  | <span data-ttu-id="7113c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7113c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7113c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7113c-123">Content-Type</span></span>  | <span data-ttu-id="7113c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7113c-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7113c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7113c-125">Request body</span></span>
<span data-ttu-id="7113c-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationUser](../resources/educationuser.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7113c-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="7113c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7113c-127">Response</span></span>
<span data-ttu-id="7113c-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7113c-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7113c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7113c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7113c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7113c-130">Request</span></span>
<span data-ttu-id="7113c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7113c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11017/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14011"
}
```

##### <a name="response"></a><span data-ttu-id="7113c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7113c-132">Response</span></span>
<span data-ttu-id="7113c-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7113c-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="7113c-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7113c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-post-teachers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
