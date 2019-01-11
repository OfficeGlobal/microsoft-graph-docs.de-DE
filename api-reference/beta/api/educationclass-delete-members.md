---
title: Entfernen eines Kursteilnehmers
description: Entfernt einen EducationUser aus einer EducationClass
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 0afab5c80c546a9404ee11fc4d127d15b13a4e9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824151"
---
# <a name="remove-a-student"></a><span data-ttu-id="92b6b-103">Entfernen eines Kursteilnehmers</span><span class="sxs-lookup"><span data-stu-id="92b6b-103">Remove a student</span></span>

> <span data-ttu-id="92b6b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="92b6b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92b6b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92b6b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92b6b-106">Entfernt einen [EducationUser](../resources/educationuser.md) aus einer [EducationClass](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="92b6b-106">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="92b6b-107">**Hinweis:** Lehrkräfte _und_ Kursteilnehmer sind in der **members**-Sammlung der Klasse enthalten.</span><span class="sxs-lookup"><span data-stu-id="92b6b-107">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="92b6b-108">Vergewissern Sie sich vor dem Aufrufen dieser API, dass der zu entfernende **educationUser** kein Lehrer ist.</span><span class="sxs-lookup"><span data-stu-id="92b6b-108">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="92b6b-109">Rufen Sie die Liste der Lehrer mit einem Aufruf von [educationclass_list_teachers](educationclass-list-teachers.md) ab, und stellen Sie sicher, dass die Benutzers-ID des zu entfernenden Benutzers nicht in der zurückgegebenen Lehrerliste enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="92b6b-109">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="92b6b-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="92b6b-110">Permissions</span></span>
<span data-ttu-id="92b6b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92b6b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92b6b-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="92b6b-113">Permission type</span></span>      | <span data-ttu-id="92b6b-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="92b6b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92b6b-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="92b6b-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="92b6b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92b6b-116">Not supported.</span></span>  |
|<span data-ttu-id="92b6b-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="92b6b-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="92b6b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92b6b-118">Not supported.</span></span>  |
|<span data-ttu-id="92b6b-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="92b6b-119">Application</span></span> | <span data-ttu-id="92b6b-120">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92b6b-120">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="92b6b-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="92b6b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="92b6b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="92b6b-122">Request headers</span></span>
| <span data-ttu-id="92b6b-123">Header</span><span class="sxs-lookup"><span data-stu-id="92b6b-123">Header</span></span>       | <span data-ttu-id="92b6b-124">Wert</span><span class="sxs-lookup"><span data-stu-id="92b6b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92b6b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="92b6b-125">Authorization</span></span>  | <span data-ttu-id="92b6b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92b6b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92b6b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="92b6b-128">Request body</span></span>
<span data-ttu-id="92b6b-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="92b6b-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="92b6b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="92b6b-130">Response</span></span>
<span data-ttu-id="92b6b-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein leerer Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92b6b-131">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="92b6b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="92b6b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92b6b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="92b6b-133">Request</span></span>
<span data-ttu-id="92b6b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="92b6b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="92b6b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="92b6b-135">Response</span></span>
<span data-ttu-id="92b6b-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="92b6b-136">The following is an example of the response.</span></span> 
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
