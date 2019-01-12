---
title: EducationClass erstellen
description: Erstellen einer neuen Klasse. Dadurch wird auch eine universelle Gruppe erstellt. Wenn Sie diese API verwenden, um eine Klasse erstellen, wird es spezielle Eigenschaften hinzufügen, wird der Gruppe
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 6a5097777392184508c6d7be6f19a198c1c5bbd9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965131"
---
# <a name="create-educationclass"></a><span data-ttu-id="c310c-105">EducationClass erstellen</span><span class="sxs-lookup"><span data-stu-id="c310c-105">Create educationClass</span></span>

> <span data-ttu-id="c310c-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c310c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c310c-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c310c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c310c-108">Erstellen einer neuen Klasse.</span><span class="sxs-lookup"><span data-stu-id="c310c-108">Create a new class.</span></span> <span data-ttu-id="c310c-109">Dadurch wird auch eine universelle Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="c310c-109">This will also create a universal group.</span></span> <span data-ttu-id="c310c-110">Wenn Sie diese API zum Erstellen einer Klasse verwenden, werden der Gruppe spezielle Eigenschaften hinzugefügt, wie z. B. Zuweisungen und besondere Behandlung in Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c310c-110">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="c310c-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c310c-111">Permissions</span></span>
<span data-ttu-id="c310c-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c310c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c310c-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c310c-114">Permission type</span></span>      | <span data-ttu-id="c310c-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c310c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c310c-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c310c-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="c310c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c310c-117">Not supported.</span></span>  |
|<span data-ttu-id="c310c-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c310c-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c310c-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c310c-119">Not supported.</span></span>  |
|<span data-ttu-id="c310c-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c310c-120">Application</span></span> | <span data-ttu-id="c310c-121">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c310c-121">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c310c-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c310c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="c310c-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c310c-123">Request headers</span></span>
| <span data-ttu-id="c310c-124">Header</span><span class="sxs-lookup"><span data-stu-id="c310c-124">Header</span></span>       | <span data-ttu-id="c310c-125">Wert</span><span class="sxs-lookup"><span data-stu-id="c310c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c310c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c310c-126">Authorization</span></span>  | <span data-ttu-id="c310c-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c310c-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c310c-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c310c-129">Content-Type</span></span>  | <span data-ttu-id="c310c-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c310c-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c310c-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c310c-131">Request body</span></span>
<span data-ttu-id="c310c-132">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationClass](../resources/educationclass.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c310c-132">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c310c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c310c-133">Response</span></span>
<span data-ttu-id="c310c-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c310c-134">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c310c-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c310c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c310c-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c310c-136">Request</span></span>
<span data-ttu-id="c310c-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c310c-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes
Content-type: application/json
Content-length: 224

{
  "description": "Health Level 1",
  "classCode": "Health 501",
  "displayName": "Health 1",
  "externalId": "11019",
  "externalName": "Health Level 1",
  "externalSource": "sis",
  "mailNickname": "fineartschool.net"
}
```

##### <a name="response"></a><span data-ttu-id="c310c-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="c310c-138">Response</span></span>
<span data-ttu-id="c310c-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c310c-139">The following is an example of the response.</span></span> 

><span data-ttu-id="c310c-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c310c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 224

{
    "id": "11019",
    "description": "Health Level 1",
    "classCode": "Health 501",
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012",
      }
    },
    "displayName": "Health 1",
    "externalId": "11019",
    "externalName": "Health Level 1",
    "externalSource": "sis",
    "mailNickname": "fineartschool.net"
}
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
