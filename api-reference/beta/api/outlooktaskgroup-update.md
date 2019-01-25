---
title: Outlooktaskgroup aktualisieren
description: Aktualisieren Sie die schreibbaren Eigenschaften einer Outlook-Aufgabe-Gruppe.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b109be3bbb0ac485dd4da7778a69a5dddf8342db
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516392"
---
# <a name="update-outlooktaskgroup"></a><span data-ttu-id="d012d-103">Outlooktaskgroup aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d012d-103">Update outlooktaskgroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d012d-104">Aktualisieren Sie die schreibbaren Eigenschaften einer Outlook-Aufgabe-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="d012d-104">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="d012d-105">Beachten Sie, dass Sie den Namen der Standardaufgabengruppe "Meine Aufgaben" nicht ändern können.</span><span class="sxs-lookup"><span data-stu-id="d012d-105">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="d012d-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d012d-106">Permissions</span></span>
<span data-ttu-id="d012d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d012d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d012d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d012d-109">Permission type</span></span>      | <span data-ttu-id="d012d-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d012d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d012d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d012d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d012d-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d012d-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d012d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d012d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d012d-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d012d-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d012d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d012d-115">Application</span></span> | <span data-ttu-id="d012d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d012d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d012d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d012d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d012d-118">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d012d-118">Optional request headers</span></span>
| <span data-ttu-id="d012d-119">Name</span><span class="sxs-lookup"><span data-stu-id="d012d-119">Name</span></span>       | <span data-ttu-id="d012d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d012d-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d012d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d012d-121">Authorization</span></span>  | <span data-ttu-id="d012d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d012d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d012d-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d012d-124">Request body</span></span>
<span data-ttu-id="d012d-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="d012d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d012d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d012d-128">Property</span></span>     | <span data-ttu-id="d012d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d012d-129">Type</span></span>   |<span data-ttu-id="d012d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d012d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d012d-131">name</span><span class="sxs-lookup"><span data-stu-id="d012d-131">name</span></span>|<span data-ttu-id="d012d-132">String</span><span class="sxs-lookup"><span data-stu-id="d012d-132">String</span></span>|<span data-ttu-id="d012d-133">Der Name der Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="d012d-133">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="d012d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d012d-134">Response</span></span>

<span data-ttu-id="d012d-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [OutlookTaskGroup](../resources/outlooktaskgroup.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d012d-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d012d-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d012d-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d012d-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d012d-137">Request</span></span>
<span data-ttu-id="d012d-138">Das folgende Beispiel ändert den Namen einer Aufgabengruppe zu "Persönliche Aufgaben".</span><span class="sxs-lookup"><span data-stu-id="d012d-138">The following example changes the name of a task group to "Personal Tasks".</span></span> 
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskgroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskgroups('AAMkADIyAAAhrbe-AAA=')

Content-type: application/json
Content-length: 28

{
  "name": "Personal Tasks",
}
```
##### <a name="response"></a><span data-ttu-id="d012d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="d012d-139">Response</span></span>
<span data-ttu-id="d012d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d012d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjw==",
  "isDefaultGroup": false,
  "name": "Personal Tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
