---
title: EducationClass abrufen
description: "  Gruppe Administratoren stellen die Lehrer in der Klasse dar. Wenn Sie das delegierte Token verwenden, werden dem Benutzer nur Klassen angezeigt, in denen er Mitglied ist."
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 148725d58d5647a85061f3b781e26cec2cb1c816
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509371"
---
# <a name="get-educationclass"></a><span data-ttu-id="6053c-104">EducationClass abrufen</span><span class="sxs-lookup"><span data-stu-id="6053c-104">Get educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6053c-105">Abrufen einer Klasse aus dem System.</span><span class="sxs-lookup"><span data-stu-id="6053c-105">Retrieve a class from the system.</span></span> <span data-ttu-id="6053c-106">Eine Klasse ist eine universelle Gruppe mit einer speziellen Eigenschaft, die dem System anzeigt, dass die Gruppe eine Klasse darstellt.</span><span class="sxs-lookup"><span data-stu-id="6053c-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="6053c-107">Gruppenmitglieder stellen die Kursteilnehmer dar. Gruppenadministratoren stellen die Lehrer in der Klasse dar.</span><span class="sxs-lookup"><span data-stu-id="6053c-107">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="6053c-108">Wenn Sie das delegierte Token verwenden, werden dem Benutzer nur Klassen angezeigt, in denen er Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="6053c-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="6053c-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6053c-109">Permissions</span></span>
<span data-ttu-id="6053c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6053c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6053c-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6053c-112">Permission type</span></span>      | <span data-ttu-id="6053c-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6053c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6053c-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6053c-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="6053c-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="6053c-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="6053c-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6053c-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6053c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6053c-117">Not supported</span></span>  |
|<span data-ttu-id="6053c-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6053c-118">Application</span></span> | <span data-ttu-id="6053c-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6053c-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6053c-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6053c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6053c-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6053c-121">Optional query parameters</span></span>
<span data-ttu-id="6053c-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6053c-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6053c-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6053c-123">Request headers</span></span>
| <span data-ttu-id="6053c-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6053c-124">Header</span></span>       | <span data-ttu-id="6053c-125">Wert</span><span class="sxs-lookup"><span data-stu-id="6053c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6053c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6053c-126">Authorization</span></span>  | <span data-ttu-id="6053c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6053c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6053c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6053c-129">Request body</span></span>
<span data-ttu-id="6053c-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6053c-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6053c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6053c-131">Response</span></span>
<span data-ttu-id="6053c-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6053c-132">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6053c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6053c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6053c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6053c-134">Request</span></span>
<span data-ttu-id="6053c-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6053c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023
```
##### <a name="response"></a><span data-ttu-id="6053c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6053c-136">Response</span></span>
<span data-ttu-id="6053c-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6053c-137">The following is an example of the response.</span></span> 

><span data-ttu-id="6053c-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6053c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
