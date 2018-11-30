---
title: EducationClass abrufen
description: "  Gruppe Administratoren stellen die Lehrer in der Klasse dar. Wenn Sie das delegierte Token verwenden, werden dem Benutzer nur Klassen angezeigt, in denen er Mitglied ist."
ms.openlocfilehash: 931c47a0885d8b82411410721fb0729aa250a422
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063069"
---
# <a name="get-educationclass"></a><span data-ttu-id="8d05e-104">EducationClass abrufen</span><span class="sxs-lookup"><span data-stu-id="8d05e-104">Get educationClass</span></span>

> <span data-ttu-id="8d05e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8d05e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d05e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d05e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d05e-107">Abrufen einer Klasse aus dem System.</span><span class="sxs-lookup"><span data-stu-id="8d05e-107">Retrieve a class from the system.</span></span> <span data-ttu-id="8d05e-108">Eine Klasse ist eine universelle Gruppe mit einer speziellen Eigenschaft, die dem System anzeigt, dass die Gruppe eine Klasse darstellt.</span><span class="sxs-lookup"><span data-stu-id="8d05e-108">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="8d05e-109">Gruppenmitglieder stellen die Kursteilnehmer dar. Gruppenadministratoren stellen die Lehrer in der Klasse dar.</span><span class="sxs-lookup"><span data-stu-id="8d05e-109">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="8d05e-110">Wenn Sie das delegierte Token verwenden, werden dem Benutzer nur Klassen angezeigt, in denen er Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="8d05e-110">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d05e-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8d05e-111">Permissions</span></span>
<span data-ttu-id="8d05e-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d05e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d05e-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d05e-114">Permission type</span></span>      | <span data-ttu-id="8d05e-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d05e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d05e-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d05e-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="8d05e-117">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="8d05e-117">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="8d05e-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d05e-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8d05e-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d05e-119">Not supported</span></span>  |
|<span data-ttu-id="8d05e-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d05e-120">Application</span></span> | <span data-ttu-id="8d05e-121">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d05e-121">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8d05e-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d05e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8d05e-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8d05e-123">Optional query parameters</span></span>
<span data-ttu-id="8d05e-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8d05e-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d05e-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d05e-125">Request headers</span></span>
| <span data-ttu-id="8d05e-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8d05e-126">Header</span></span>       | <span data-ttu-id="8d05e-127">Wert</span><span class="sxs-lookup"><span data-stu-id="8d05e-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d05e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d05e-128">Authorization</span></span>  | <span data-ttu-id="8d05e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8d05e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d05e-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d05e-131">Request body</span></span>
<span data-ttu-id="8d05e-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8d05e-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8d05e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d05e-133">Response</span></span>
<span data-ttu-id="8d05e-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d05e-134">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8d05e-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d05e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d05e-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d05e-136">Request</span></span>
<span data-ttu-id="8d05e-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d05e-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023
```
##### <a name="response"></a><span data-ttu-id="8d05e-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d05e-138">Response</span></span>
<span data-ttu-id="8d05e-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8d05e-139">The following is an example of the response.</span></span> 

><span data-ttu-id="8d05e-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8d05e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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