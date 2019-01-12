---
title: EducationClass abrufen
description: "  Gruppe Administratoren stellen die Lehrer in der Klasse dar. Wenn Sie das delegierte Token verwenden, werden dem Benutzer nur Klassen angezeigt, in denen er Mitglied ist."
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: ddf29c9d2a136f8f5cee24b30ef9ab1c0f9643f5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935682"
---
# <a name="get-educationclass"></a><span data-ttu-id="53268-104">EducationClass abrufen</span><span class="sxs-lookup"><span data-stu-id="53268-104">Get educationClass</span></span>

> <span data-ttu-id="53268-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="53268-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53268-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53268-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53268-107">Abrufen einer Klasse aus dem System.</span><span class="sxs-lookup"><span data-stu-id="53268-107">Retrieve a class from the system.</span></span> <span data-ttu-id="53268-108">Eine Klasse ist eine universelle Gruppe mit einer speziellen Eigenschaft, die dem System anzeigt, dass die Gruppe eine Klasse darstellt.</span><span class="sxs-lookup"><span data-stu-id="53268-108">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="53268-109">Gruppenmitglieder stellen die Kursteilnehmer dar. Gruppenadministratoren stellen die Lehrer in der Klasse dar.</span><span class="sxs-lookup"><span data-stu-id="53268-109">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="53268-110">Wenn Sie das delegierte Token verwenden, werden dem Benutzer nur Klassen angezeigt, in denen er Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="53268-110">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="53268-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53268-111">Permissions</span></span>
<span data-ttu-id="53268-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53268-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53268-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53268-114">Permission type</span></span>      | <span data-ttu-id="53268-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53268-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53268-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53268-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="53268-117">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="53268-117">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="53268-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53268-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="53268-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53268-119">Not supported</span></span>  |
|<span data-ttu-id="53268-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53268-120">Application</span></span> | <span data-ttu-id="53268-121">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53268-121">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="53268-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53268-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53268-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="53268-123">Optional query parameters</span></span>
<span data-ttu-id="53268-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53268-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53268-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53268-125">Request headers</span></span>
| <span data-ttu-id="53268-126">Header</span><span class="sxs-lookup"><span data-stu-id="53268-126">Header</span></span>       | <span data-ttu-id="53268-127">Wert</span><span class="sxs-lookup"><span data-stu-id="53268-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53268-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="53268-128">Authorization</span></span>  | <span data-ttu-id="53268-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53268-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53268-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53268-131">Request body</span></span>
<span data-ttu-id="53268-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="53268-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="53268-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="53268-133">Response</span></span>
<span data-ttu-id="53268-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53268-134">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53268-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53268-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53268-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53268-136">Request</span></span>
<span data-ttu-id="53268-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53268-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023
```
##### <a name="response"></a><span data-ttu-id="53268-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="53268-138">Response</span></span>
<span data-ttu-id="53268-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53268-139">The following is an example of the response.</span></span> 

><span data-ttu-id="53268-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="53268-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
