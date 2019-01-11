---
title: EducationAssignmentResource aktualisieren
description: 'Aktualisieren Sie die Eigenschaften der Ressource einer Zuordnung zugeordnet. Zuordnungsfeld Resource-Objekten können nur Lehrer in einer Klasse geändert werden.  '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 91321cc124baa87a82f2f1f5fecc65365cafc18d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879310"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="9f393-104">EducationAssignmentResource aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9f393-104">Update educationAssignmentResource</span></span>

> <span data-ttu-id="9f393-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9f393-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f393-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f393-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f393-107">Aktualisieren Sie die Eigenschaften der Ressource einer Zuordnung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="9f393-107">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="9f393-108">Zuordnungsfeld Resource-Objekten können nur Lehrer in einer Klasse geändert werden.</span><span class="sxs-lookup"><span data-stu-id="9f393-108">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="9f393-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f393-109">Permissions</span></span>
<span data-ttu-id="9f393-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f393-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f393-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f393-112">Permission type</span></span>      | <span data-ttu-id="9f393-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f393-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f393-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f393-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="9f393-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f393-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="9f393-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f393-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9f393-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f393-117">Not supported.</span></span>  |
|<span data-ttu-id="9f393-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f393-118">Application</span></span> | <span data-ttu-id="9f393-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f393-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9f393-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f393-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9f393-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f393-121">Request headers</span></span>
| <span data-ttu-id="9f393-122">Header</span><span class="sxs-lookup"><span data-stu-id="9f393-122">Header</span></span>       | <span data-ttu-id="9f393-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9f393-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f393-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f393-124">Authorization</span></span>  | <span data-ttu-id="9f393-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f393-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9f393-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f393-127">Content-Type</span></span>  | <span data-ttu-id="9f393-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9f393-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f393-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f393-129">Request body</span></span>
<span data-ttu-id="9f393-130">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9f393-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9f393-131">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="9f393-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9f393-132">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="9f393-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9f393-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9f393-133">Property</span></span>     | <span data-ttu-id="9f393-134">Typ</span><span class="sxs-lookup"><span data-stu-id="9f393-134">Type</span></span>   |<span data-ttu-id="9f393-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f393-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f393-136">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="9f393-136">distributeForStudentWork</span></span>|<span data-ttu-id="9f393-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9f393-137">Boolean</span></span>| <span data-ttu-id="9f393-138">Gibt an, ob diese Ressource in jeder Student Resource-Objekt kopiert werden soll, wenn die Zuordnung veröffentlicht wird.</span><span class="sxs-lookup"><span data-stu-id="9f393-138">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="9f393-139">resource</span><span class="sxs-lookup"><span data-stu-id="9f393-139">resource</span></span>|<span data-ttu-id="9f393-140">educationResource</span><span class="sxs-lookup"><span data-stu-id="9f393-140">educationResource</span></span>| <span data-ttu-id="9f393-141">Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="9f393-141">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="9f393-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f393-142">Response</span></span>
<span data-ttu-id="9f393-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EducationAssignmentResource](../resources/educationassignmentresource.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9f393-143">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f393-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f393-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f393-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f393-145">Request</span></span>
<span data-ttu-id="9f393-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f393-146">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="9f393-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f393-147">Response</span></span>
<span data-ttu-id="9f393-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9f393-148">The following is an example of the response.</span></span> 

><span data-ttu-id="9f393-149">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="9f393-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9f393-150">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f393-150">All of the properties will be returned from an actual call.</span></span>


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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
