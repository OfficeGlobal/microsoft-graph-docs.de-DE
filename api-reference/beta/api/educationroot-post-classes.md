---
title: EducationClass erstellen
description: Erstellen einer neuen Klasse. Dadurch wird auch eine universelle Gruppe erstellt. Wenn Sie diese API verwenden, um eine Klasse erstellen, wird es spezielle Eigenschaften hinzufügen, wird der Gruppe
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9d6146251bf5f5badd733ab58272adbc0e71dea3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507943"
---
# <a name="create-educationclass"></a><span data-ttu-id="88f68-105">EducationClass erstellen</span><span class="sxs-lookup"><span data-stu-id="88f68-105">Create educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88f68-106">Erstellen einer neuen Klasse.</span><span class="sxs-lookup"><span data-stu-id="88f68-106">Create a new class.</span></span> <span data-ttu-id="88f68-107">Dadurch wird auch eine universelle Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="88f68-107">This will also create a universal group.</span></span> <span data-ttu-id="88f68-108">Wenn Sie diese API zum Erstellen einer Klasse verwenden, werden der Gruppe spezielle Eigenschaften hinzugefügt, wie z. B. Zuweisungen und besondere Behandlung in Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="88f68-108">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="88f68-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="88f68-109">Permissions</span></span>
<span data-ttu-id="88f68-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88f68-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88f68-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="88f68-112">Permission type</span></span>      | <span data-ttu-id="88f68-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="88f68-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88f68-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="88f68-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="88f68-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88f68-115">Not supported.</span></span>  |
|<span data-ttu-id="88f68-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="88f68-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="88f68-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88f68-117">Not supported.</span></span>  |
|<span data-ttu-id="88f68-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="88f68-118">Application</span></span> | <span data-ttu-id="88f68-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88f68-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="88f68-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="88f68-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="88f68-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="88f68-121">Request headers</span></span>
| <span data-ttu-id="88f68-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="88f68-122">Header</span></span>       | <span data-ttu-id="88f68-123">Wert</span><span class="sxs-lookup"><span data-stu-id="88f68-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88f68-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="88f68-124">Authorization</span></span>  | <span data-ttu-id="88f68-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="88f68-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="88f68-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88f68-127">Content-Type</span></span>  | <span data-ttu-id="88f68-128">application/json</span><span class="sxs-lookup"><span data-stu-id="88f68-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88f68-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="88f68-129">Request body</span></span>
<span data-ttu-id="88f68-130">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationClass](../resources/educationclass.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="88f68-130">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="88f68-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="88f68-131">Response</span></span>
<span data-ttu-id="88f68-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="88f68-132">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88f68-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="88f68-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88f68-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="88f68-134">Request</span></span>
<span data-ttu-id="88f68-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="88f68-135">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="88f68-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="88f68-136">Response</span></span>
<span data-ttu-id="88f68-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="88f68-137">The following is an example of the response.</span></span> 

><span data-ttu-id="88f68-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="88f68-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationroot-post-classes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
