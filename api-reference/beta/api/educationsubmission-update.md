---
title: Educationsubmission aktualisieren
description: Note und Feedback zu einer Übermittlung hinzufügen. Dieser Vorgang können nur Lehrer ausgeführt werden. Beachten Sie, dass die grundlegende Berechtigung hat keinen Zugriff auf die Eigenschaften für die Qualität und daher Note oder Feedback kann nicht geschrieben werden. Diese Aktion wird die Note und ihr Feedback an die Student nicht freigegeben. Lehrer muss eine Aktion explizite Freigabe, für die Qualität Daten zum Schüler zurückgegeben werden soll.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c420d2c6e512d8fed0d713340fea482b0888ca1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526116"
---
# <a name="update-educationsubmission"></a><span data-ttu-id="dff01-107">Educationsubmission aktualisieren</span><span class="sxs-lookup"><span data-stu-id="dff01-107">Update educationsubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dff01-108">Note und Feedback zu einer Übermittlung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="dff01-108">Add a grade and feedback to a submission.</span></span> <span data-ttu-id="dff01-109">Dieser Vorgang können nur Lehrer ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="dff01-109">Only teachers can perform this operation.</span></span> <span data-ttu-id="dff01-110">Beachten Sie, dass die grundlegende Berechtigung hat keinen Zugriff auf die Eigenschaften für die Qualität und daher Note oder Feedback kann nicht geschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="dff01-110">Note that the Basic permission does not have access to the grade properties, and therefore cannot write to grade or feedback.</span></span> <span data-ttu-id="dff01-111">Diese Aktion wird die Note und ihr Feedback an die Student nicht freigegeben.</span><span class="sxs-lookup"><span data-stu-id="dff01-111">This action does not release the grade and feedback to the student.</span></span> <span data-ttu-id="dff01-112">Lehrer muss eine Aktion explizite Freigabe, für die Qualität Daten zum Schüler zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="dff01-112">A teacher must take an explicit release action for the grade data to be returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="dff01-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dff01-113">Permissions</span></span>
<span data-ttu-id="dff01-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dff01-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dff01-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dff01-116">Permission type</span></span>      | <span data-ttu-id="dff01-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dff01-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dff01-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dff01-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="dff01-119">EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dff01-119">EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="dff01-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dff01-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dff01-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dff01-121">Not supported.</span></span>   |
|<span data-ttu-id="dff01-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dff01-122">Application</span></span> | <span data-ttu-id="dff01-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dff01-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dff01-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dff01-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dff01-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dff01-125">Request headers</span></span>
| <span data-ttu-id="dff01-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dff01-126">Header</span></span>       | <span data-ttu-id="dff01-127">Wert</span><span class="sxs-lookup"><span data-stu-id="dff01-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dff01-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="dff01-128">Authorization</span></span>  | <span data-ttu-id="dff01-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dff01-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dff01-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dff01-131">Request body</span></span>
<span data-ttu-id="dff01-132">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="dff01-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dff01-133">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="dff01-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dff01-134">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="dff01-134">For best performance, don't include existing values that haven't changed.</span></span>

<!-- Provide the property descriptions. -->

| <span data-ttu-id="dff01-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dff01-135">Property</span></span>     | <span data-ttu-id="dff01-136">Typ</span><span class="sxs-lookup"><span data-stu-id="dff01-136">Type</span></span>   |<span data-ttu-id="dff01-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dff01-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dff01-138">Feedback</span><span class="sxs-lookup"><span data-stu-id="dff01-138">feedback</span></span>|<span data-ttu-id="dff01-139">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="dff01-139">educationFeedback</span></span>||
|<span data-ttu-id="dff01-140">grade</span><span class="sxs-lookup"><span data-stu-id="dff01-140">grade</span></span>|<span data-ttu-id="dff01-141">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="dff01-141">educationAssignmentGrade</span></span>||

## <a name="response"></a><span data-ttu-id="dff01-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="dff01-142">Response</span></span>
<span data-ttu-id="dff01-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EducationSubmission](../resources/educationsubmission.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dff01-143">If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dff01-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dff01-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dff01-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dff01-145">Request</span></span>
<span data-ttu-id="dff01-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dff01-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_educationsubmission"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7
Content-type: application/json
Content-length: 658

{
  "feedback": {
    "text": {
      "content": "Good work!",
      "contentType": "Text"
    },
    "feedbackDateTime": "2014-01-01T00:00:00Z",
    "feedbackBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
      "@odata.type": "microsoft.graph.identitySet"
    },
    "@odata.type": "microsoft.graph.educationFeedback"
  },
  "grade": {
      "gradedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
      "@odata.type": "microsoft.graph.identitySet"
    },
    "gradedDateTime": "2014-01-01T00:00:00Z",
    "@odata.type": "microsoft.graph.educationAssignmentGrade"
  }
}
```
##### <a name="response"></a><span data-ttu-id="dff01-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="dff01-147">Response</span></span>
<span data-ttu-id="dff01-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dff01-148">The following is an example of the response.</span></span> 

><span data-ttu-id="dff01-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="dff01-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1217

{
  "feedback": {
    "text": {
      "content": "Good work!",
      "contentType": "Text"
    },
    "feedbackDateTime": "2014-01-01T00:00:00Z",
    "feedbackBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      }
    },
    "@odata.type": "microsoft.graph.educationFeedback"
  },
  "grade": {
         "gradedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
          "@odata.type": "microsoft.graph.identitySet"
        },
        "gradedDateTime": "2014-01-01T00:00:00Z",
        "@odata.type": "microsoft.graph.educationAssignmentGrade"
  },
  "id": "850f51b7",
  "recipient": {
    userId:"dsfewsddf",
    "@odata.type": "#microsoft.graph.educationSubmissionRecipient"
  },
  "releasedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    },
  },
  "releasedDateTime": "2014-01-01T00:00:00Z",
  "resourcesFolderUrl": "String",
  "status": "completed",
  "submittedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    },
  },
  "submittedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationsubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
