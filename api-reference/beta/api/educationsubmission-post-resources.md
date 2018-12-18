---
title: Erstellen von educationSubmissionResource
description: 'Fügt eine Ressource zur Ressourcenliste. Diese Aktion nur von den Teilnehmern möglich, dem diese Übermittlung zugewiesen ist. Diese Aktion nicht erfolgreich, wenn das Flag **AllowStudentsToAddResources** nicht festgelegt ist auf "true". Wenn der Aufrufer eine neue Ressource dateibasierten erstellen möchte, muss die Datei dem Ordner Ressourcen hochgeladen werden, die der Übermittlung zugeordnet ist. Die POST-Anforderung schlägt fehl, wenn die Datei nicht vorhanden ist oder nicht in diesem Ordner ist. '
author: dipakboyed
ms.openlocfilehash: 71d06e996213c133ed9c48d5d3e320a785e122ae
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321301"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="4706f-107">Erstellen von educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="4706f-107">Create educationSubmissionResource</span></span>

> <span data-ttu-id="4706f-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4706f-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4706f-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4706f-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4706f-110">Fügt eine Ressource zur Ressourcenliste.</span><span class="sxs-lookup"><span data-stu-id="4706f-110">Adds a resource to the resources list.</span></span> <span data-ttu-id="4706f-111">Diese Aktion nur von den Teilnehmern möglich, dem diese Übermittlung zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="4706f-111">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="4706f-112">Diese Aktion nicht erfolgreich, wenn das Flag **AllowStudentsToAddResources** nicht festgelegt ist auf "true".</span><span class="sxs-lookup"><span data-stu-id="4706f-112">This action will not succeed if the **allowStudentsToAddResources** flag is not set to true.</span></span> <span data-ttu-id="4706f-113">Wenn der Aufrufer eine neue Ressource dateibasierten erstellen möchte, muss die Datei dem Ordner Ressourcen hochgeladen werden, die der Übermittlung zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="4706f-113">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="4706f-114">Die POST-Anforderung schlägt fehl, wenn die Datei nicht vorhanden ist oder nicht in diesem Ordner ist.</span><span class="sxs-lookup"><span data-stu-id="4706f-114">If the file does not exist or is not in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4706f-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4706f-115">Permissions</span></span>
<span data-ttu-id="4706f-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4706f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4706f-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4706f-118">Permission type</span></span>      | <span data-ttu-id="4706f-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4706f-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4706f-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4706f-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="4706f-121">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4706f-121">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4706f-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4706f-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4706f-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4706f-123">Not supported.</span></span>  |
|<span data-ttu-id="4706f-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4706f-124">Application</span></span> | <span data-ttu-id="4706f-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4706f-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4706f-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4706f-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources

```
## <a name="request-headers"></a><span data-ttu-id="4706f-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4706f-127">Request headers</span></span>
| <span data-ttu-id="4706f-128">Header</span><span class="sxs-lookup"><span data-stu-id="4706f-128">Header</span></span>       | <span data-ttu-id="4706f-129">Wert</span><span class="sxs-lookup"><span data-stu-id="4706f-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4706f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="4706f-130">Authorization</span></span>  | <span data-ttu-id="4706f-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4706f-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4706f-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4706f-133">Content-Type</span></span>  | <span data-ttu-id="4706f-134">application/json</span><span class="sxs-lookup"><span data-stu-id="4706f-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4706f-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4706f-135">Request body</span></span>
<span data-ttu-id="4706f-136">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [EducationSubmissionResource](../resources/educationsubmissionresource.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4706f-136">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="4706f-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="4706f-137">Response</span></span>
<span data-ttu-id="4706f-138">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `201 Created` Antwortcode und eines [EducationSubmissionResource](../resources/educationsubmissionresource.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4706f-138">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4706f-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4706f-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4706f-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4706f-140">Request</span></span>
<span data-ttu-id="4706f-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4706f-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationsubmissionresource_from_educationsubmission"
}-->
```
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources
Content-type: application/json
Content-length: 1097

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
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
  },
  "@odata.type": "microsoft.graph.educationResource"
}

```

##### <a name="response"></a><span data-ttu-id="4706f-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="4706f-142">Response</span></span>
<span data-ttu-id="4706f-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4706f-143">The following is an example of the response.</span></span> 

><span data-ttu-id="4706f-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4706f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 201 Created
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
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6",
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->