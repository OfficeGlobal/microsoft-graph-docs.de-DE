---
title: Educationsubmission aktualisieren
description: Note und Feedback zu einer Übermittlung hinzufügen. Dieser Vorgang können nur Lehrer ausgeführt werden. Beachten Sie, dass die grundlegende Berechtigung hat keinen Zugriff auf die Eigenschaften für die Qualität und daher Note oder Feedback kann nicht geschrieben werden. Diese Aktion wird die Note und ihr Feedback an die Student nicht freigegeben. Lehrer muss eine Aktion explizite Freigabe, für die Qualität Daten zum Schüler zurückgegeben werden soll.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 516940f9a6dd43460aa0ceb9b955c41dc89196c6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828784"
---
# <a name="update-educationsubmission"></a><span data-ttu-id="6ff75-107">Educationsubmission aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6ff75-107">Update educationsubmission</span></span>

> <span data-ttu-id="6ff75-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6ff75-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ff75-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ff75-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ff75-110">Note und Feedback zu einer Übermittlung hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="6ff75-110">Add a grade and feedback to a submission.</span></span> <span data-ttu-id="6ff75-111">Dieser Vorgang können nur Lehrer ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="6ff75-111">Only teachers can perform this operation.</span></span> <span data-ttu-id="6ff75-112">Beachten Sie, dass die grundlegende Berechtigung hat keinen Zugriff auf die Eigenschaften für die Qualität und daher Note oder Feedback kann nicht geschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="6ff75-112">Note that the Basic permission does not have access to the grade properties, and therefore cannot write to grade or feedback.</span></span> <span data-ttu-id="6ff75-113">Diese Aktion wird die Note und ihr Feedback an die Student nicht freigegeben.</span><span class="sxs-lookup"><span data-stu-id="6ff75-113">This action does not release the grade and feedback to the student.</span></span> <span data-ttu-id="6ff75-114">Lehrer muss eine Aktion explizite Freigabe, für die Qualität Daten zum Schüler zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="6ff75-114">A teacher must take an explicit release action for the grade data to be returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ff75-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6ff75-115">Permissions</span></span>
<span data-ttu-id="6ff75-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ff75-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ff75-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6ff75-118">Permission type</span></span>      | <span data-ttu-id="6ff75-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6ff75-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ff75-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6ff75-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="6ff75-121">EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ff75-121">EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="6ff75-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6ff75-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ff75-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ff75-123">Not supported.</span></span>   |
|<span data-ttu-id="6ff75-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6ff75-124">Application</span></span> | <span data-ttu-id="6ff75-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ff75-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6ff75-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ff75-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6ff75-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6ff75-127">Request headers</span></span>
| <span data-ttu-id="6ff75-128">Header</span><span class="sxs-lookup"><span data-stu-id="6ff75-128">Header</span></span>       | <span data-ttu-id="6ff75-129">Wert</span><span class="sxs-lookup"><span data-stu-id="6ff75-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6ff75-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ff75-130">Authorization</span></span>  | <span data-ttu-id="6ff75-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6ff75-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6ff75-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6ff75-133">Request body</span></span>
<span data-ttu-id="6ff75-134">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6ff75-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6ff75-135">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="6ff75-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6ff75-136">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="6ff75-136">For best performance, don't include existing values that haven't changed.</span></span>

<!-- Provide the property descriptions. -->

| <span data-ttu-id="6ff75-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ff75-137">Property</span></span>     | <span data-ttu-id="6ff75-138">Typ</span><span class="sxs-lookup"><span data-stu-id="6ff75-138">Type</span></span>   |<span data-ttu-id="6ff75-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ff75-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ff75-140">Feedback</span><span class="sxs-lookup"><span data-stu-id="6ff75-140">feedback</span></span>|<span data-ttu-id="6ff75-141">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="6ff75-141">educationFeedback</span></span>||
|<span data-ttu-id="6ff75-142">grade</span><span class="sxs-lookup"><span data-stu-id="6ff75-142">grade</span></span>|<span data-ttu-id="6ff75-143">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="6ff75-143">educationAssignmentGrade</span></span>||

## <a name="response"></a><span data-ttu-id="6ff75-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ff75-144">Response</span></span>
<span data-ttu-id="6ff75-145">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EducationSubmission](../resources/educationsubmission.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6ff75-145">If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ff75-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6ff75-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ff75-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ff75-147">Request</span></span>
<span data-ttu-id="6ff75-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6ff75-148">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6ff75-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ff75-149">Response</span></span>
<span data-ttu-id="6ff75-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6ff75-150">The following is an example of the response.</span></span> 

><span data-ttu-id="6ff75-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6ff75-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationsubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
