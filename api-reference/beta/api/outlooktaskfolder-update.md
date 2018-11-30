---
title: Outlooktaskfolder aktualisieren
description: Aktualisieren Sie die schreibbaren Eigenschaften des Ordners eine Outlook-Aufgabe.
ms.openlocfilehash: 8b02f3b8eea104ba0a0cfaa3fddaf286fa41f389
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065024"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="a11c7-103">Outlooktaskfolder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a11c7-103">Update outlooktaskfolder</span></span>

> <span data-ttu-id="a11c7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a11c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a11c7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a11c7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a11c7-106">Aktualisieren Sie die schreibbaren Eigenschaften des Ordners eine Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="a11c7-106">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="a11c7-107">Sie können den **Name** -Eigenschaftswert der Aufgabe Standardordner "Aufgaben" nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="a11c7-107">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="a11c7-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a11c7-108">Permissions</span></span>
<span data-ttu-id="a11c7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a11c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a11c7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a11c7-111">Permission type</span></span>      | <span data-ttu-id="a11c7-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a11c7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a11c7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a11c7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a11c7-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a11c7-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a11c7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a11c7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a11c7-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a11c7-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a11c7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a11c7-117">Application</span></span> | <span data-ttu-id="a11c7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a11c7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a11c7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a11c7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a11c7-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a11c7-120">Optional request headers</span></span>
| <span data-ttu-id="a11c7-121">Name</span><span class="sxs-lookup"><span data-stu-id="a11c7-121">Name</span></span>       | <span data-ttu-id="a11c7-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a11c7-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a11c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a11c7-123">Authorization</span></span>  | <span data-ttu-id="a11c7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a11c7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a11c7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a11c7-126">Request body</span></span>
<span data-ttu-id="a11c7-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="a11c7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a11c7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a11c7-130">Property</span></span>     | <span data-ttu-id="a11c7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a11c7-131">Type</span></span>   |<span data-ttu-id="a11c7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a11c7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a11c7-133">name</span><span class="sxs-lookup"><span data-stu-id="a11c7-133">name</span></span>|<span data-ttu-id="a11c7-134">String</span><span class="sxs-lookup"><span data-stu-id="a11c7-134">String</span></span>|<span data-ttu-id="a11c7-135">Der Name des Aufgabenordners.</span><span class="sxs-lookup"><span data-stu-id="a11c7-135">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="a11c7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a11c7-136">Response</span></span>

<span data-ttu-id="a11c7-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [OutlookTaskFolder](../resources/outlooktaskfolder.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a11c7-137">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a11c7-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a11c7-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a11c7-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a11c7-139">Request</span></span>
<span data-ttu-id="a11c7-140">Das folgende Beispiel ändert den Namen des angegebenen Ordner zu `Charity work`.</span><span class="sxs-lookup"><span data-stu-id="a11c7-140">The following example changes the name of the specified task folder to `Charity work`.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPWAAA=')
Content-type: application/json
Content-length: 31

{
  "name": "Charity work"
}
```
##### <a name="response"></a><span data-ttu-id="a11c7-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="a11c7-141">Response</span></span>
<span data-ttu-id="a11c7-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a11c7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAKfQ==",
  "isDefaultFolder": false,
  "name": "Charity work",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->