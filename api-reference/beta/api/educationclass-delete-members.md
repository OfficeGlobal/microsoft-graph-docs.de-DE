---
title: Entfernen eines Kursteilnehmers
description: Entfernt einen EducationUser aus einer EducationClass
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ba9d490691b6d717fc1d088408c25a2724eb491a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507908"
---
# <a name="remove-a-student"></a><span data-ttu-id="71433-103">Entfernen eines Kursteilnehmers</span><span class="sxs-lookup"><span data-stu-id="71433-103">Remove a student</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71433-104">Entfernt einen [EducationUser](../resources/educationuser.md) aus einer [EducationClass](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="71433-104">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="71433-105">**Hinweis:** Lehrkräfte _und_ Kursteilnehmer sind in der **members**-Sammlung der Klasse enthalten.</span><span class="sxs-lookup"><span data-stu-id="71433-105">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="71433-106">Vergewissern Sie sich vor dem Aufrufen dieser API, dass der zu entfernende **educationUser** kein Lehrer ist.</span><span class="sxs-lookup"><span data-stu-id="71433-106">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="71433-107">Rufen Sie die Liste der Lehrer mit einem Aufruf von [educationclass_list_teachers](educationclass-list-teachers.md) ab, und stellen Sie sicher, dass die Benutzers-ID des zu entfernenden Benutzers nicht in der zurückgegebenen Lehrerliste enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="71433-107">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="71433-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="71433-108">Permissions</span></span>
<span data-ttu-id="71433-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71433-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71433-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71433-111">Permission type</span></span>      | <span data-ttu-id="71433-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71433-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71433-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71433-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="71433-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71433-114">Not supported.</span></span>  |
|<span data-ttu-id="71433-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71433-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="71433-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71433-116">Not supported.</span></span>  |
|<span data-ttu-id="71433-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71433-117">Application</span></span> | <span data-ttu-id="71433-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71433-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="71433-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71433-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="71433-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71433-120">Request headers</span></span>
| <span data-ttu-id="71433-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="71433-121">Header</span></span>       | <span data-ttu-id="71433-122">Wert</span><span class="sxs-lookup"><span data-stu-id="71433-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71433-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71433-123">Authorization</span></span>  | <span data-ttu-id="71433-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="71433-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71433-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71433-126">Request body</span></span>
<span data-ttu-id="71433-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="71433-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="71433-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="71433-128">Response</span></span>
<span data-ttu-id="71433-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein leerer Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71433-129">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="71433-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71433-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71433-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71433-131">Request</span></span>
<span data-ttu-id="71433-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71433-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="71433-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="71433-133">Response</span></span>
<span data-ttu-id="71433-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="71433-134">The following is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-delete-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
