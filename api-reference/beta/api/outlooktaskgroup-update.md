---
title: Outlooktaskgroup aktualisieren
description: Aktualisieren Sie die schreibbaren Eigenschaften einer Outlook-Aufgabe-Gruppe.
author: angelgolfer-ms
ms.openlocfilehash: 40d146f90bf512ec9afa8790d7f02d4039dd53cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334902"
---
# <a name="update-outlooktaskgroup"></a><span data-ttu-id="1459c-103">Outlooktaskgroup aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1459c-103">Update outlooktaskgroup</span></span>

> <span data-ttu-id="1459c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1459c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1459c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1459c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1459c-106">Aktualisieren Sie die schreibbaren Eigenschaften einer Outlook-Aufgabe-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1459c-106">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="1459c-107">Beachten Sie, dass Sie den Namen der Aufgabe Standardgruppe "Meine Aufgaben" nicht geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="1459c-107">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="1459c-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1459c-108">Permissions</span></span>
<span data-ttu-id="1459c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1459c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1459c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1459c-111">Permission type</span></span>      | <span data-ttu-id="1459c-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1459c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1459c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1459c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1459c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1459c-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1459c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1459c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1459c-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1459c-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1459c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1459c-117">Application</span></span> | <span data-ttu-id="1459c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1459c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1459c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1459c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1459c-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1459c-120">Optional request headers</span></span>
| <span data-ttu-id="1459c-121">Name</span><span class="sxs-lookup"><span data-stu-id="1459c-121">Name</span></span>       | <span data-ttu-id="1459c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1459c-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1459c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1459c-123">Authorization</span></span>  | <span data-ttu-id="1459c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1459c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1459c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1459c-126">Request body</span></span>
<span data-ttu-id="1459c-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="1459c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1459c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1459c-130">Property</span></span>     | <span data-ttu-id="1459c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1459c-131">Type</span></span>   |<span data-ttu-id="1459c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1459c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1459c-133">name</span><span class="sxs-lookup"><span data-stu-id="1459c-133">name</span></span>|<span data-ttu-id="1459c-134">String</span><span class="sxs-lookup"><span data-stu-id="1459c-134">String</span></span>|<span data-ttu-id="1459c-135">Der Name der Aufgabengruppe.</span><span class="sxs-lookup"><span data-stu-id="1459c-135">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="1459c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="1459c-136">Response</span></span>

<span data-ttu-id="1459c-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [OutlookTaskGroup](../resources/outlooktaskgroup.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1459c-137">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1459c-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1459c-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1459c-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1459c-139">Request</span></span>
<span data-ttu-id="1459c-140">Das folgende Beispiel ändert den Namen einer Aufgabengruppe zu "Persönliche Aufgaben".</span><span class="sxs-lookup"><span data-stu-id="1459c-140">The following example changes the name of a task group to "Personal Tasks".</span></span> 
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
##### <a name="response"></a><span data-ttu-id="1459c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="1459c-141">Response</span></span>
<span data-ttu-id="1459c-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1459c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktaskgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->