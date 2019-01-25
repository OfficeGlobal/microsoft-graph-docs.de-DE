---
title: Educationassignment aktualisieren
description: Aktualisieren Sie das Assignment-Objekt. Nur Lehrer in der Klasse ist dies möglich. Beachten Sie, dass eine Anforderung PATCH zum Ändern des Status einer Zuordnung verwendet werden können. Verwenden Sie die Veröffentlichungsaktion zum Ändern des Zuordnungsstatus.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: eb5762f86e1572f9a9d5876199c945154a25293b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524961"
---
# <a name="update-educationassignment"></a><span data-ttu-id="3a82e-106">Educationassignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3a82e-106">Update educationassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a82e-107">Aktualisieren Sie das Assignment-Objekt.</span><span class="sxs-lookup"><span data-stu-id="3a82e-107">Update the assignment object.</span></span> <span data-ttu-id="3a82e-108">Nur Lehrer in der Klasse ist dies möglich.</span><span class="sxs-lookup"><span data-stu-id="3a82e-108">Only teachers in the class can do this.</span></span> <span data-ttu-id="3a82e-109">Beachten Sie, dass eine Anforderung PATCH zum Ändern des Status einer Zuordnung verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="3a82e-109">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="3a82e-110">Verwenden Sie die Aktion [Veröffentlichen](../api/educationassignment-publish.md) , um den Status einer Aufgabe ändern.</span><span class="sxs-lookup"><span data-stu-id="3a82e-110">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a82e-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3a82e-111">Permissions</span></span>
<span data-ttu-id="3a82e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a82e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a82e-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a82e-114">Permission type</span></span>      | <span data-ttu-id="3a82e-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a82e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a82e-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a82e-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="3a82e-117">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a82e-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="3a82e-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a82e-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3a82e-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a82e-119">Not supported.</span></span>  |
|<span data-ttu-id="3a82e-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a82e-120">Application</span></span> | <span data-ttu-id="3a82e-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a82e-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3a82e-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a82e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3a82e-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a82e-123">Request headers</span></span>
| <span data-ttu-id="3a82e-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3a82e-124">Header</span></span>       | <span data-ttu-id="3a82e-125">Wert</span><span class="sxs-lookup"><span data-stu-id="3a82e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a82e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a82e-126">Authorization</span></span>  | <span data-ttu-id="3a82e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a82e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3a82e-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a82e-129">Content-Type</span></span>  | <span data-ttu-id="3a82e-130">application/json</span><span class="sxs-lookup"><span data-stu-id="3a82e-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a82e-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a82e-131">Request body</span></span>
<span data-ttu-id="3a82e-132">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="3a82e-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3a82e-133">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="3a82e-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3a82e-134">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="3a82e-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3a82e-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3a82e-135">Property</span></span>     | <span data-ttu-id="3a82e-136">Typ</span><span class="sxs-lookup"><span data-stu-id="3a82e-136">Type</span></span>   |<span data-ttu-id="3a82e-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a82e-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a82e-138">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="3a82e-138">allowLateSubmissions</span></span>|<span data-ttu-id="3a82e-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3a82e-139">Boolean</span></span>| <span data-ttu-id="3a82e-140">Gibt an, ob nach dem Fälligkeitsdatum Übermittlungen gesendet werden können.</span><span class="sxs-lookup"><span data-stu-id="3a82e-140">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="3a82e-141">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="3a82e-141">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="3a82e-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3a82e-142">Boolean</span></span>| <span data-ttu-id="3a82e-143">Gibt an, ob eine Student Ressourcen zu einer Übermittlung hinzufügen kann.</span><span class="sxs-lookup"><span data-stu-id="3a82e-143">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="3a82e-144">Angegeben, ob die Ressourcenliste Zuordnung der einzige Elemente auf der Übermittlung stammt.</span><span class="sxs-lookup"><span data-stu-id="3a82e-144">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="3a82e-145">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="3a82e-145">assignDateTime</span></span>|<span data-ttu-id="3a82e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a82e-146">DateTimeOffset</span></span>| <span data-ttu-id="3a82e-147">Datum, an dem die Zuordnung für Studenten veröffentlicht werden soll.</span><span class="sxs-lookup"><span data-stu-id="3a82e-147">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="3a82e-148">assignTo</span><span class="sxs-lookup"><span data-stu-id="3a82e-148">assignTo</span></span>|<span data-ttu-id="3a82e-149">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="3a82e-149">educationAssignmentRecipient</span></span>| <span data-ttu-id="3a82e-150">Teilnehmer, die die Zuordnung zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="3a82e-150">Students who get the assignment.</span></span>|
|<span data-ttu-id="3a82e-151">displayName</span><span class="sxs-lookup"><span data-stu-id="3a82e-151">displayName</span></span>|<span data-ttu-id="3a82e-152">String</span><span class="sxs-lookup"><span data-stu-id="3a82e-152">String</span></span>| <span data-ttu-id="3a82e-153">Name der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="3a82e-153">Name of assignment.</span></span> |
|<span data-ttu-id="3a82e-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="3a82e-154">dueDateTime</span></span>|<span data-ttu-id="3a82e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a82e-155">DateTimeOffset</span></span>| <span data-ttu-id="3a82e-156">Datum Aufgabe ist fällig.</span><span class="sxs-lookup"><span data-stu-id="3a82e-156">Date assignment is due.</span></span> |
|<span data-ttu-id="3a82e-157">Benotung</span><span class="sxs-lookup"><span data-stu-id="3a82e-157">grading</span></span>|<span data-ttu-id="3a82e-158">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="3a82e-158">educationAssignmentGradeType</span></span>| <span data-ttu-id="3a82e-159">Wie wird die Zuordnung eingestuft.</span><span class="sxs-lookup"><span data-stu-id="3a82e-159">How the assignment will be graded.</span></span>|
|<span data-ttu-id="3a82e-160">Anweisungen</span><span class="sxs-lookup"><span data-stu-id="3a82e-160">instructions</span></span>|<span data-ttu-id="3a82e-161">itemBody</span><span class="sxs-lookup"><span data-stu-id="3a82e-161">itemBody</span></span>| <span data-ttu-id="3a82e-162">Anleitung für die Kursteilnehmer zusammen mit der Zuordnung angegeben.</span><span class="sxs-lookup"><span data-stu-id="3a82e-162">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="3a82e-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a82e-163">Response</span></span>
<span data-ttu-id="3a82e-164">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EducationAssignment](../resources/educationassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3a82e-164">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a82e-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a82e-165">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a82e-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a82e-166">Request</span></span>
<span data-ttu-id="3a82e-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a82e-167">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002
Content-type: application/json
Content-length: 279

{
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z"
}
```
##### <a name="response"></a><span data-ttu-id="3a82e-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a82e-168">Response</span></span>
<span data-ttu-id="3a82e-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3a82e-169">The following is an example of the response.</span></span> 

><span data-ttu-id="3a82e-170">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="3a82e-170">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3a82e-171">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a82e-171">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "classId": "11021",
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
