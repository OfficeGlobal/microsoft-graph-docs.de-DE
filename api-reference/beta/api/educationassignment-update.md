---
title: Educationassignment aktualisieren
description: Aktualisieren Sie das Assignment-Objekt. Nur Lehrer in der Klasse ist dies möglich. Beachten Sie, dass eine Anforderung PATCH zum Ändern des Status einer Zuordnung verwendet werden können. Verwenden Sie die Veröffentlichungsaktion zum Ändern des Zuordnungsstatus.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: f8d79e11628e3a02a20c9ecdcd46bcd1bff05e7f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960350"
---
# <a name="update-educationassignment"></a><span data-ttu-id="abc50-106">Educationassignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="abc50-106">Update educationassignment</span></span>

> <span data-ttu-id="abc50-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="abc50-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abc50-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="abc50-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="abc50-109">Aktualisieren Sie das Assignment-Objekt.</span><span class="sxs-lookup"><span data-stu-id="abc50-109">Update the assignment object.</span></span> <span data-ttu-id="abc50-110">Nur Lehrer in der Klasse ist dies möglich.</span><span class="sxs-lookup"><span data-stu-id="abc50-110">Only teachers in the class can do this.</span></span> <span data-ttu-id="abc50-111">Beachten Sie, dass eine Anforderung PATCH zum Ändern des Status einer Zuordnung verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="abc50-111">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="abc50-112">Verwenden Sie die Aktion [Veröffentlichen](../api/educationassignment-publish.md) , um den Status einer Aufgabe ändern.</span><span class="sxs-lookup"><span data-stu-id="abc50-112">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="abc50-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="abc50-113">Permissions</span></span>
<span data-ttu-id="abc50-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abc50-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abc50-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="abc50-116">Permission type</span></span>      | <span data-ttu-id="abc50-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="abc50-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abc50-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="abc50-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="abc50-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="abc50-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="abc50-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="abc50-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="abc50-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abc50-121">Not supported.</span></span>  |
|<span data-ttu-id="abc50-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="abc50-122">Application</span></span> | <span data-ttu-id="abc50-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abc50-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="abc50-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="abc50-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="abc50-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="abc50-125">Request headers</span></span>
| <span data-ttu-id="abc50-126">Header</span><span class="sxs-lookup"><span data-stu-id="abc50-126">Header</span></span>       | <span data-ttu-id="abc50-127">Wert</span><span class="sxs-lookup"><span data-stu-id="abc50-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="abc50-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="abc50-128">Authorization</span></span>  | <span data-ttu-id="abc50-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="abc50-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="abc50-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="abc50-131">Content-Type</span></span>  | <span data-ttu-id="abc50-132">application/json</span><span class="sxs-lookup"><span data-stu-id="abc50-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="abc50-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="abc50-133">Request body</span></span>
<span data-ttu-id="abc50-134">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="abc50-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="abc50-135">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="abc50-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="abc50-136">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="abc50-136">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="abc50-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="abc50-137">Property</span></span>     | <span data-ttu-id="abc50-138">Typ</span><span class="sxs-lookup"><span data-stu-id="abc50-138">Type</span></span>   |<span data-ttu-id="abc50-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abc50-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abc50-140">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="abc50-140">allowLateSubmissions</span></span>|<span data-ttu-id="abc50-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="abc50-141">Boolean</span></span>| <span data-ttu-id="abc50-142">Gibt an, ob nach dem Fälligkeitsdatum Übermittlungen gesendet werden können.</span><span class="sxs-lookup"><span data-stu-id="abc50-142">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="abc50-143">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="abc50-143">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="abc50-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="abc50-144">Boolean</span></span>| <span data-ttu-id="abc50-145">Gibt an, ob eine Student Ressourcen zu einer Übermittlung hinzufügen kann.</span><span class="sxs-lookup"><span data-stu-id="abc50-145">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="abc50-146">Angegeben, ob die Ressourcenliste Zuordnung der einzige Elemente auf der Übermittlung stammt.</span><span class="sxs-lookup"><span data-stu-id="abc50-146">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="abc50-147">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="abc50-147">assignDateTime</span></span>|<span data-ttu-id="abc50-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abc50-148">DateTimeOffset</span></span>| <span data-ttu-id="abc50-149">Datum, an dem die Zuordnung für Studenten veröffentlicht werden soll.</span><span class="sxs-lookup"><span data-stu-id="abc50-149">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="abc50-150">assignTo</span><span class="sxs-lookup"><span data-stu-id="abc50-150">assignTo</span></span>|<span data-ttu-id="abc50-151">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="abc50-151">educationAssignmentRecipient</span></span>| <span data-ttu-id="abc50-152">Teilnehmer, die die Zuordnung zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="abc50-152">Students who get the assignment.</span></span>|
|<span data-ttu-id="abc50-153">displayName</span><span class="sxs-lookup"><span data-stu-id="abc50-153">displayName</span></span>|<span data-ttu-id="abc50-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="abc50-154">String</span></span>| <span data-ttu-id="abc50-155">Name der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="abc50-155">Name of assignment.</span></span> |
|<span data-ttu-id="abc50-156">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="abc50-156">dueDateTime</span></span>|<span data-ttu-id="abc50-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abc50-157">DateTimeOffset</span></span>| <span data-ttu-id="abc50-158">Datum Aufgabe ist fällig.</span><span class="sxs-lookup"><span data-stu-id="abc50-158">Date assignment is due.</span></span> |
|<span data-ttu-id="abc50-159">Benotung</span><span class="sxs-lookup"><span data-stu-id="abc50-159">grading</span></span>|<span data-ttu-id="abc50-160">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="abc50-160">educationAssignmentGradeType</span></span>| <span data-ttu-id="abc50-161">Wie wird die Zuordnung eingestuft.</span><span class="sxs-lookup"><span data-stu-id="abc50-161">How the assignment will be graded.</span></span>|
|<span data-ttu-id="abc50-162">Anleitung</span><span class="sxs-lookup"><span data-stu-id="abc50-162">instructions</span></span>|<span data-ttu-id="abc50-163">itemBody</span><span class="sxs-lookup"><span data-stu-id="abc50-163">itemBody</span></span>| <span data-ttu-id="abc50-164">Anleitung für die Kursteilnehmer zusammen mit der Zuordnung angegeben.</span><span class="sxs-lookup"><span data-stu-id="abc50-164">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="abc50-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="abc50-165">Response</span></span>
<span data-ttu-id="abc50-166">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EducationAssignment](../resources/educationassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="abc50-166">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="abc50-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="abc50-167">Example</span></span>
##### <a name="request"></a><span data-ttu-id="abc50-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="abc50-168">Request</span></span>
<span data-ttu-id="abc50-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="abc50-169">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="abc50-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="abc50-170">Response</span></span>
<span data-ttu-id="abc50-171">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="abc50-171">The following is an example of the response.</span></span> 

><span data-ttu-id="abc50-172">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="abc50-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="abc50-173">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="abc50-173">All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
