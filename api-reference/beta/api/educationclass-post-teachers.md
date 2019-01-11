---
title: Lehrer hinzufügen
description: Hinzufügen eines Lehrers zu einer Klasse.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 284c84cc140f0f9c15831396ed5adddaff73fdc6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882986"
---
# <a name="add-teacher"></a><span data-ttu-id="7f49d-103">Lehrer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="7f49d-103">Add teacher</span></span>

> <span data-ttu-id="7f49d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7f49d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f49d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7f49d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f49d-106">Hinzufügen eines Lehrers zu einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="7f49d-106">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f49d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7f49d-107">Permissions</span></span>
<span data-ttu-id="7f49d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f49d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f49d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f49d-110">Permission type</span></span>      | <span data-ttu-id="7f49d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f49d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f49d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f49d-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="7f49d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f49d-113">Not supported.</span></span>  |
|<span data-ttu-id="7f49d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f49d-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7f49d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f49d-115">Not supported.</span></span>  |
|<span data-ttu-id="7f49d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f49d-116">Application</span></span> | <span data-ttu-id="7f49d-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f49d-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7f49d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f49d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7f49d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f49d-119">Request headers</span></span>
| <span data-ttu-id="7f49d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7f49d-120">Header</span></span>       | <span data-ttu-id="7f49d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7f49d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7f49d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f49d-122">Authorization</span></span>  | <span data-ttu-id="7f49d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7f49d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7f49d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f49d-125">Content-Type</span></span>  | <span data-ttu-id="7f49d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f49d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f49d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f49d-127">Request body</span></span>
<span data-ttu-id="7f49d-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationUser](../resources/educationuser.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7f49d-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="7f49d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f49d-129">Response</span></span>
<span data-ttu-id="7f49d-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f49d-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f49d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f49d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f49d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f49d-132">Request</span></span>
<span data-ttu-id="7f49d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f49d-133">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7f49d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f49d-134">Response</span></span>
<span data-ttu-id="7f49d-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7f49d-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="7f49d-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7f49d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
