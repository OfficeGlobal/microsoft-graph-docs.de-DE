---
title: 'EducationAssignment: GetResourcesFolderUrl'
description: 'Diese Funktion gibt die OneDrive-URL, in dem alle dateibasierten Ressourcen (Word, Excel usw.) hochgeladen werden soll.  '
localization_priority: Normal
ms.openlocfilehash: 4352fb051573f91ef93e781a1a06ba984b17a9ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887388"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="687e4-103">EducationAssignment: GetResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="687e4-103">educationAssignment: getResourcesFolderUrl</span></span>

> <span data-ttu-id="687e4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="687e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="687e4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="687e4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="687e4-106">Diese Funktion gibt die OneDrive-URL, in dem alle dateibasierten Ressourcen (Word, Excel usw.) hochgeladen werden soll.</span><span class="sxs-lookup"><span data-stu-id="687e4-106">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="687e4-107">Beachten Sie, dass Dateien in diesem Ordner gespeichert sein müssen, um als Ressourcen hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="687e4-107">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="687e4-108">Nur in der Klasse Lehrer kann ermitteln, welche Dateien hochladen.</span><span class="sxs-lookup"><span data-stu-id="687e4-108">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="687e4-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="687e4-109">Permissions</span></span>
<span data-ttu-id="687e4-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="687e4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="687e4-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="687e4-112">Permission type</span></span>      | <span data-ttu-id="687e4-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="687e4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="687e4-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="687e4-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="687e4-115">EduAssignments.ReadBasic EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="687e4-115">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="687e4-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="687e4-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="687e4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="687e4-117">Not supported.</span></span>  |
|<span data-ttu-id="687e4-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="687e4-118">Application</span></span> | <span data-ttu-id="687e4-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="687e4-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="687e4-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="687e4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="687e4-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="687e4-121">Request headers</span></span>
| <span data-ttu-id="687e4-122">Header</span><span class="sxs-lookup"><span data-stu-id="687e4-122">Header</span></span>       | <span data-ttu-id="687e4-123">Wert</span><span class="sxs-lookup"><span data-stu-id="687e4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="687e4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="687e4-124">Authorization</span></span>  | <span data-ttu-id="687e4-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="687e4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="687e4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="687e4-127">Request body</span></span>
<span data-ttu-id="687e4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="687e4-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="687e4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="687e4-129">Response</span></span>
<span data-ttu-id="687e4-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 Ok` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="687e4-130">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="687e4-131">Im Textkörper enthält der OneDrive-URL eines Ordners zum Speichern aller dateibasierten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="687e4-131">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="687e4-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="687e4-132">Example</span></span>
<span data-ttu-id="687e4-133">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="687e4-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="687e4-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="687e4-134">Request</span></span>
<span data-ttu-id="687e4-135">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="687e4-135">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```

##### <a name="response"></a><span data-ttu-id="687e4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="687e4-136">Response</span></span>
<span data-ttu-id="687e4-137">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="687e4-137">The following is an example of a response.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
