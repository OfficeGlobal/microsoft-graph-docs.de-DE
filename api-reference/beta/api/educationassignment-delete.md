---
title: EducationAssignment löschen
description: Löschen Sie eine vorhandene Zuordnung. Nur Lehrer innerhalb einer Klasse können Arbeitsaufträge löschen.
ms.openlocfilehash: e9965efa458459cff0c3914dbc12b37153a6ab51
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063065"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="77155-104">EducationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="77155-104">Delete educationAssignment</span></span>

> <span data-ttu-id="77155-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="77155-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77155-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77155-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77155-107">Löschen Sie eine vorhandene Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="77155-107">Delete an existing assignment.</span></span> <span data-ttu-id="77155-108">Nur Lehrer innerhalb einer Klasse können Arbeitsaufträge löschen.</span><span class="sxs-lookup"><span data-stu-id="77155-108">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="77155-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="77155-109">Permissions</span></span>
<span data-ttu-id="77155-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77155-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77155-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77155-112">Permission type</span></span>      | <span data-ttu-id="77155-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77155-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77155-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77155-114">Delegated (work or school account)</span></span>| <span data-ttu-id="77155-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77155-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="77155-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77155-116">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="77155-117">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77155-117">Not Supported.</span></span> |
|<span data-ttu-id="77155-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77155-118">Application</span></span> | <span data-ttu-id="77155-119">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77155-119">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="77155-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77155-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignments/<id>
```
## <a name="request-headers"></a><span data-ttu-id="77155-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77155-121">Request headers</span></span>
| <span data-ttu-id="77155-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="77155-122">Header</span></span>       | <span data-ttu-id="77155-123">Wert</span><span class="sxs-lookup"><span data-stu-id="77155-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77155-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77155-124">Authorization</span></span>  | <span data-ttu-id="77155-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77155-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77155-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77155-127">Request body</span></span>
<span data-ttu-id="77155-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="77155-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="77155-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="77155-129">Response</span></span>
<span data-ttu-id="77155-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77155-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77155-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77155-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="77155-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77155-133">Request</span></span>
<span data-ttu-id="77155-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77155-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="77155-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="77155-135">Response</span></span>
<span data-ttu-id="77155-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="77155-136">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->