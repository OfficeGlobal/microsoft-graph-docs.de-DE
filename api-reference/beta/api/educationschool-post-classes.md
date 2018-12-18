---
title: EducationClass zu educationSchool hinzufügen
description: Hinzufügen einer Klasse zu einer Schule.
author: mmast-msft
ms.openlocfilehash: 2ac40545dadb083751192ae516fb131d43cccb64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308848"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="db9c0-103">EducationClass zu educationSchool hinzufügen</span><span class="sxs-lookup"><span data-stu-id="db9c0-103">Add educationClass to educationSchool</span></span>

> <span data-ttu-id="db9c0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="db9c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db9c0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="db9c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db9c0-106">Hinzufügen einer Klasse zu einer Schule.</span><span class="sxs-lookup"><span data-stu-id="db9c0-106">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="db9c0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="db9c0-107">Permissions</span></span>
<span data-ttu-id="db9c0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db9c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db9c0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db9c0-110">Permission type</span></span>      | <span data-ttu-id="db9c0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="db9c0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db9c0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db9c0-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="db9c0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db9c0-113">Not supported.</span></span>  |
|<span data-ttu-id="db9c0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="db9c0-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="db9c0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db9c0-115">Not supported.</span></span>  |
|<span data-ttu-id="db9c0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db9c0-116">Application</span></span> | <span data-ttu-id="db9c0-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db9c0-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="db9c0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db9c0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="db9c0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db9c0-119">Request headers</span></span>
| <span data-ttu-id="db9c0-120">Header</span><span class="sxs-lookup"><span data-stu-id="db9c0-120">Header</span></span>       | <span data-ttu-id="db9c0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="db9c0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="db9c0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db9c0-122">Authorization</span></span>  | <span data-ttu-id="db9c0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="db9c0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="db9c0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db9c0-125">Content-Type</span></span>  | <span data-ttu-id="db9c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db9c0-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db9c0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db9c0-127">Request body</span></span>
<span data-ttu-id="db9c0-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationClass](../resources/educationclass.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="db9c0-128">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="db9c0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="db9c0-129">Response</span></span>
<span data-ttu-id="db9c0-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db9c0-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db9c0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db9c0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db9c0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="db9c0-132">Request</span></span>
<span data-ttu-id="db9c0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="db9c0-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/10002/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/beta/education/classes/11006"
}
```

##### <a name="response"></a><span data-ttu-id="db9c0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="db9c0-134">Response</span></span> 
<span data-ttu-id="db9c0-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="db9c0-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->