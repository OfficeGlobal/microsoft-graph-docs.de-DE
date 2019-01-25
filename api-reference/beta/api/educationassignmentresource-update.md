---
title: EducationAssignmentResource aktualisieren
description: 'Aktualisieren Sie die Eigenschaften der Ressource einer Zuordnung zugeordnet. Zuordnungsfeld Resource-Objekten können nur Lehrer in einer Klasse geändert werden.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 34b1c05937f57fe46d5d854d21a7c2e0b68240d2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527955"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="ef665-104">EducationAssignmentResource aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ef665-104">Update educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef665-105">Aktualisieren Sie die Eigenschaften der Ressource einer Zuordnung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="ef665-105">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="ef665-106">Zuordnungsfeld Resource-Objekten können nur Lehrer in einer Klasse geändert werden.</span><span class="sxs-lookup"><span data-stu-id="ef665-106">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="ef665-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ef665-107">Permissions</span></span>
<span data-ttu-id="ef665-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef665-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef665-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef665-110">Permission type</span></span>      | <span data-ttu-id="ef665-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef665-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef665-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef665-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="ef665-113">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef665-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="ef665-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef665-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ef665-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef665-115">Not supported.</span></span>  |
|<span data-ttu-id="ef665-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef665-116">Application</span></span> | <span data-ttu-id="ef665-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef665-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ef665-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef665-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ef665-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef665-119">Request headers</span></span>
| <span data-ttu-id="ef665-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ef665-120">Header</span></span>       | <span data-ttu-id="ef665-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ef665-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ef665-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef665-122">Authorization</span></span>  | <span data-ttu-id="ef665-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ef665-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ef665-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef665-125">Content-Type</span></span>  | <span data-ttu-id="ef665-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef665-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ef665-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef665-127">Request body</span></span>
<span data-ttu-id="ef665-128">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ef665-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ef665-129">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="ef665-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ef665-130">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="ef665-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ef665-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ef665-131">Property</span></span>     | <span data-ttu-id="ef665-132">Typ</span><span class="sxs-lookup"><span data-stu-id="ef665-132">Type</span></span>   |<span data-ttu-id="ef665-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef665-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef665-134">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="ef665-134">distributeForStudentWork</span></span>|<span data-ttu-id="ef665-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ef665-135">Boolean</span></span>| <span data-ttu-id="ef665-136">Gibt an, ob diese Ressource in jeder Student Resource-Objekt kopiert werden soll, wenn die Zuordnung veröffentlicht wird.</span><span class="sxs-lookup"><span data-stu-id="ef665-136">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="ef665-137">resource</span><span class="sxs-lookup"><span data-stu-id="ef665-137">resource</span></span>|<span data-ttu-id="ef665-138">educationResource</span><span class="sxs-lookup"><span data-stu-id="ef665-138">educationResource</span></span>| <span data-ttu-id="ef665-139">Resource-Objekt</span><span class="sxs-lookup"><span data-stu-id="ef665-139">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="ef665-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef665-140">Response</span></span>
<span data-ttu-id="ef665-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EducationAssignmentResource](../resources/educationassignmentresource.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ef665-141">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ef665-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef665-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef665-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef665-143">Request</span></span>
<span data-ttu-id="ef665-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef665-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_educationassignmentresource"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/850f51b7-1df9-4ec0-bd62-64a0214b9cbf
Content-type: application/json
Content-length: 822

{
  "distributeForStudentWork": "false"
}
```
##### <a name="response"></a><span data-ttu-id="ef665-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef665-145">Response</span></span>
<span data-ttu-id="ef665-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ef665-146">The following is an example of the response.</span></span> 

><span data-ttu-id="ef665-147">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="ef665-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ef665-148">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef665-148">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 832

{
  "distributeForStudentWork": false,
  "resource": {
      "@odata.type": "#microsoft.graph.educationLinkResource",
      "displayName": "Microsoft Homepage",
      "createdDateTime": "2017-10-21T07:52:45.5675913Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "link": "https://www.microsoft.com"
  },
  "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignmentresource-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
