---
title: Erstellen von educationAssignmentResource
description: um anzugeben, welche Art von Ressource OData.Type wird erstellt. Beachten Sie, dass Ressourcen dateibasierten zunächst in die Zuordnungen **Ressourcefolder**hochgeladen werden müssen.
localization_priority: Normal
ms.openlocfilehash: 206e7db8c8e96f230bc0062fa9b080831b1b4e1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854012"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="f56a0-104">Erstellen von educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="f56a0-104">Create educationAssignmentResource</span></span>

> <span data-ttu-id="f56a0-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f56a0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f56a0-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f56a0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f56a0-107">Erstellen Sie eine [Zuordnung Ressource](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="f56a0-107">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="f56a0-108">Die Ressource selbst verfügt über eine @odata.type um anzugeben, welche Art von Ressource erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="f56a0-108">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="f56a0-109">Beachten Sie, dass Ressourcen dateibasierten zunächst in die Zuordnungen **Ressourcefolder**hochgeladen werden müssen.</span><span class="sxs-lookup"><span data-stu-id="f56a0-109">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f56a0-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f56a0-110">Permissions</span></span>
<span data-ttu-id="f56a0-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f56a0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f56a0-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f56a0-113">Permission type</span></span>      | <span data-ttu-id="f56a0-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f56a0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f56a0-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f56a0-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="f56a0-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f56a0-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f56a0-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f56a0-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f56a0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f56a0-118">Not supported.</span></span>  |
|<span data-ttu-id="f56a0-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f56a0-119">Application</span></span> | <span data-ttu-id="f56a0-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f56a0-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f56a0-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f56a0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="f56a0-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f56a0-122">Request headers</span></span>
| <span data-ttu-id="f56a0-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f56a0-123">Header</span></span>       | <span data-ttu-id="f56a0-124">Wert</span><span class="sxs-lookup"><span data-stu-id="f56a0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f56a0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f56a0-125">Authorization</span></span>  | <span data-ttu-id="f56a0-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f56a0-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f56a0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f56a0-128">Content-Type</span></span>  | <span data-ttu-id="f56a0-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f56a0-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f56a0-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f56a0-130">Request body</span></span>
<span data-ttu-id="f56a0-131">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [EducationAssignmentResource](../resources/educationassignmentresource.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f56a0-131">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f56a0-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f56a0-132">Response</span></span>
<span data-ttu-id="f56a0-133">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `201 Created` Antwortcode und eines [EducationAssignmentResource](../resources/educationassignmentresource.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f56a0-133">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f56a0-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f56a0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f56a0-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f56a0-135">Request</span></span>
<span data-ttu-id="f56a0-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f56a0-136">The following is an example of the request.</span></span>
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
<span data-ttu-id="f56a0-137">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [EducationAssignmentResource](../resources/educationassignmentresource.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f56a0-137">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f56a0-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f56a0-138">Response</span></span>
<span data-ttu-id="f56a0-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f56a0-139">The following is an example of the response.</span></span> 

><span data-ttu-id="f56a0-140">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="f56a0-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f56a0-141">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f56a0-141">All of the properties will be returned from an actual call.</span></span>


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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
