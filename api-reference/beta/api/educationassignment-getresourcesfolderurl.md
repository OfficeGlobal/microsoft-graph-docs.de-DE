---
title: 'EducationAssignment: GetResourcesFolderUrl'
description: 'Diese Funktion gibt die OneDrive-URL, in dem alle dateibasierten Ressourcen (Word, Excel usw.) hochgeladen werden soll.  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 43bef729d2cf37561d0742ebb3adfb21fe4f486e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512031"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="d4d09-103">EducationAssignment: GetResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="d4d09-103">educationAssignment: getResourcesFolderUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4d09-104">Diese Funktion gibt die OneDrive-URL, in dem alle dateibasierten Ressourcen (Word, Excel usw.) hochgeladen werden soll.</span><span class="sxs-lookup"><span data-stu-id="d4d09-104">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="d4d09-105">Beachten Sie, dass Dateien in diesem Ordner gespeichert sein müssen, um als Ressourcen hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d4d09-105">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="d4d09-106">Nur in der Klasse Lehrer kann ermitteln, welche Dateien hochladen.</span><span class="sxs-lookup"><span data-stu-id="d4d09-106">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d4d09-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d4d09-107">Permissions</span></span>
<span data-ttu-id="d4d09-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4d09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4d09-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4d09-110">Permission type</span></span>      | <span data-ttu-id="d4d09-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4d09-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4d09-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4d09-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="d4d09-113">EduAssignments.ReadBasic EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="d4d09-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="d4d09-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4d09-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d4d09-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4d09-115">Not supported.</span></span>  |
|<span data-ttu-id="d4d09-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4d09-116">Application</span></span> | <span data-ttu-id="d4d09-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4d09-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d4d09-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4d09-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="d4d09-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4d09-119">Request headers</span></span>
| <span data-ttu-id="d4d09-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d4d09-120">Header</span></span>       | <span data-ttu-id="d4d09-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d4d09-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4d09-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4d09-122">Authorization</span></span>  | <span data-ttu-id="d4d09-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d4d09-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4d09-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4d09-125">Request body</span></span>
<span data-ttu-id="d4d09-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d4d09-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d4d09-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4d09-127">Response</span></span>
<span data-ttu-id="d4d09-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 Ok` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4d09-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="d4d09-129">Im Textkörper enthält der OneDrive-URL eines Ordners zum Speichern aller dateibasierten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="d4d09-129">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="d4d09-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4d09-130">Example</span></span>
<span data-ttu-id="d4d09-131">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="d4d09-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d4d09-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4d09-132">Request</span></span>
<span data-ttu-id="d4d09-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4d09-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```

##### <a name="response"></a><span data-ttu-id="d4d09-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4d09-134">Response</span></span>
<span data-ttu-id="d4d09-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="d4d09-135">The following is an example of a response.</span></span> 

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Edm.String",
    "value": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-getresourcesfolderurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
