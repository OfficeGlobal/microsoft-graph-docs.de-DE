---
title: Abrufen von educationSubmissionResource
description: " Ressourcenliste und sollte in Bearbeitung durch einen Schüler berücksichtigt werden. Diese Ressource mit einem möglichen Zeiger an die Zuordnung Ressource umbrochen werden, wenn es die Zuordnung kopiert wurde."
ms.openlocfilehash: 1bba0b8b4e89b0f3bc564f48187cfe46fc49cf46
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058306"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="93fa9-104">Abrufen von educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="93fa9-104">Get educationSubmissionResource</span></span>

> <span data-ttu-id="93fa9-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="93fa9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93fa9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93fa9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93fa9-107">Ruft die Eigenschaften einer bestimmten Ressource der Übermittlung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="93fa9-107">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="93fa9-108">Diese Ressource ist in der Liste "Working" Ressource und sollte in Bearbeitung durch einen Schüler berücksichtigt werden.</span><span class="sxs-lookup"><span data-stu-id="93fa9-108">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="93fa9-109">Diese Ressource mit einem möglichen Zeiger an die Zuordnung Ressource umbrochen werden, wenn es die Zuordnung kopiert wurde.</span><span class="sxs-lookup"><span data-stu-id="93fa9-109">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="93fa9-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="93fa9-110">Permissions</span></span>
<span data-ttu-id="93fa9-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93fa9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93fa9-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="93fa9-113">Permission type</span></span>      | <span data-ttu-id="93fa9-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="93fa9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93fa9-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="93fa9-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="93fa9-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93fa9-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="93fa9-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="93fa9-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="93fa9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93fa9-118">Not supported.</span></span>  |
|<span data-ttu-id="93fa9-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="93fa9-119">Application</span></span> | <span data-ttu-id="93fa9-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93fa9-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="93fa9-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93fa9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93fa9-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="93fa9-122">Optional query parameters</span></span>
<span data-ttu-id="93fa9-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="93fa9-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93fa9-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93fa9-124">Request headers</span></span>
| <span data-ttu-id="93fa9-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="93fa9-125">Header</span></span>       | <span data-ttu-id="93fa9-126">Wert</span><span class="sxs-lookup"><span data-stu-id="93fa9-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93fa9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="93fa9-127">Authorization</span></span>  | <span data-ttu-id="93fa9-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="93fa9-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93fa9-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93fa9-130">Request body</span></span>
<span data-ttu-id="93fa9-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="93fa9-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="93fa9-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="93fa9-132">Response</span></span>
<span data-ttu-id="93fa9-133">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [EducationSubmissionResource](../resources/educationsubmissionresource.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="93fa9-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93fa9-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93fa9-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93fa9-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93fa9-135">Request</span></span>
<span data-ttu-id="93fa9-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93fa9-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmissionresource"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="93fa9-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="93fa9-137">Response</span></span>
<span data-ttu-id="93fa9-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="93fa9-138">The following is an example of the response.</span></span> 

><span data-ttu-id="93fa9-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="93fa9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1152

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
  "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
  "resource": {
      "@odata.type": "#microsoft.graph.educationWordResource",
      "displayName": "Report.docx",
      "createdDateTime": "2017-10-21T07:52:53.9863696Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
