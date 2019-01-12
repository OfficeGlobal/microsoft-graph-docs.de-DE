---
title: Entfernen eines Kursteilnehmers
description: Entfernt einen EducationUser aus einer EducationClass
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 38e3a1e5058db04db1c35213c65ec231e6d3a86e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966587"
---
# <a name="remove-a-student"></a><span data-ttu-id="2b7f3-103">Entfernen eines Kursteilnehmers</span><span class="sxs-lookup"><span data-stu-id="2b7f3-103">Remove a student</span></span>

> <span data-ttu-id="2b7f3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2b7f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b7f3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2b7f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b7f3-106">Entfernt einen [EducationUser](../resources/educationuser.md) aus einer [EducationClass](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="2b7f3-106">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="2b7f3-107">**Hinweis:** Lehrkräfte _und_ Kursteilnehmer sind in der **members**-Sammlung der Klasse enthalten.</span><span class="sxs-lookup"><span data-stu-id="2b7f3-107">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="2b7f3-108">Vergewissern Sie sich vor dem Aufrufen dieser API, dass der zu entfernende **educationUser** kein Lehrer ist.</span><span class="sxs-lookup"><span data-stu-id="2b7f3-108">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="2b7f3-109">Rufen Sie die Liste der Lehrer mit einem Aufruf von [educationclass_list_teachers](educationclass-list-teachers.md) ab, und stellen Sie sicher, dass die Benutzers-ID des zu entfernenden Benutzers nicht in der zurückgegebenen Lehrerliste enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="2b7f3-109">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b7f3-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b7f3-110">Permissions</span></span>
<span data-ttu-id="2b7f3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b7f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b7f3-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b7f3-113">Permission type</span></span>      | <span data-ttu-id="2b7f3-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b7f3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b7f3-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b7f3-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="2b7f3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b7f3-116">Not supported.</span></span>  |
|<span data-ttu-id="2b7f3-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b7f3-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2b7f3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b7f3-118">Not supported.</span></span>  |
|<span data-ttu-id="2b7f3-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b7f3-119">Application</span></span> | <span data-ttu-id="2b7f3-120">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7f3-120">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2b7f3-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b7f3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2b7f3-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b7f3-122">Request headers</span></span>
| <span data-ttu-id="2b7f3-123">Header</span><span class="sxs-lookup"><span data-stu-id="2b7f3-123">Header</span></span>       | <span data-ttu-id="2b7f3-124">Wert</span><span class="sxs-lookup"><span data-stu-id="2b7f3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b7f3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b7f3-125">Authorization</span></span>  | <span data-ttu-id="2b7f3-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2b7f3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b7f3-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b7f3-128">Request body</span></span>
<span data-ttu-id="2b7f3-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2b7f3-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2b7f3-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b7f3-130">Response</span></span>
<span data-ttu-id="2b7f3-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein leerer Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b7f3-131">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b7f3-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b7f3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b7f3-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b7f3-133">Request</span></span>
<span data-ttu-id="2b7f3-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2b7f3-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="2b7f3-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b7f3-135">Response</span></span>
<span data-ttu-id="2b7f3-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2b7f3-136">The following is an example of the response.</span></span> 
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
