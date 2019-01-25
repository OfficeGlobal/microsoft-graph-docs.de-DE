---
title: Erstellen von educationAssignmentResource
description: um anzugeben, welche Art von Ressource OData.Type wird erstellt. Beachten Sie, dass Ressourcen dateibasierten zunächst in die Zuordnungen **Ressourcefolder**hochgeladen werden müssen.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 34e8740336acbef056ec0b3703547de51fdc42ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527990"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="53fe5-104">Erstellen von educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="53fe5-104">Create educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53fe5-105">Erstellen Sie eine [Zuordnung Ressource](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="53fe5-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="53fe5-106">Die Ressource selbst verfügt über eine @odata.type um anzugeben, welche Art von Ressource erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="53fe5-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="53fe5-107">Beachten Sie, dass Ressourcen dateibasierten zunächst in die Zuordnungen **Ressourcefolder**hochgeladen werden müssen.</span><span class="sxs-lookup"><span data-stu-id="53fe5-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="53fe5-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53fe5-108">Permissions</span></span>
<span data-ttu-id="53fe5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53fe5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53fe5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53fe5-111">Permission type</span></span>      | <span data-ttu-id="53fe5-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53fe5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53fe5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53fe5-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="53fe5-114">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53fe5-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="53fe5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53fe5-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="53fe5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53fe5-116">Not supported.</span></span>  |
|<span data-ttu-id="53fe5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53fe5-117">Application</span></span> | <span data-ttu-id="53fe5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53fe5-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="53fe5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53fe5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="53fe5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53fe5-120">Request headers</span></span>
| <span data-ttu-id="53fe5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="53fe5-121">Header</span></span>       | <span data-ttu-id="53fe5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="53fe5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53fe5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53fe5-123">Authorization</span></span>  | <span data-ttu-id="53fe5-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53fe5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="53fe5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53fe5-126">Content-Type</span></span>  | <span data-ttu-id="53fe5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="53fe5-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53fe5-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53fe5-128">Request body</span></span>
<span data-ttu-id="53fe5-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [EducationAssignmentResource](../resources/educationassignmentresource.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="53fe5-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="53fe5-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="53fe5-130">Response</span></span>
<span data-ttu-id="53fe5-131">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `201 Created` Antwortcode und eines [EducationAssignmentResource](../resources/educationassignmentresource.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="53fe5-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53fe5-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53fe5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53fe5-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53fe5-133">Request</span></span>
<span data-ttu-id="53fe5-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53fe5-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationassignmentresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources
Content-type: application/json
Content-length: 212

{
  "distributeForStudentWork": "false",
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<span data-ttu-id="53fe5-135">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [EducationAssignmentResource](../resources/educationassignmentresource.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="53fe5-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="53fe5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="53fe5-136">Response</span></span>
<span data-ttu-id="53fe5-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53fe5-137">The following is an example of the response.</span></span> 

><span data-ttu-id="53fe5-138">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="53fe5-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="53fe5-139">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53fe5-139">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 229

{
  "id": "122333",
  "distributeForStudentWork": false,
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-post-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
