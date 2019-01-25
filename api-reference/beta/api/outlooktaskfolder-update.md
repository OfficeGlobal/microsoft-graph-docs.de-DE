---
title: Outlooktaskfolder aktualisieren
description: Aktualisieren Sie die schreibbaren Eigenschaften des Ordners eine Outlook-Aufgabe.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 83b75fb2588f58480e51e4e548bfd5d05b7f941b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530160"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="f7859-103">Outlooktaskfolder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f7859-103">Update outlooktaskfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7859-104">Aktualisieren Sie die schreibbaren Eigenschaften des Ordners eine Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="f7859-104">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="f7859-105">Sie können den **Name** -Eigenschaftswert der Aufgabe Standardordner "Aufgaben" nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="f7859-105">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="f7859-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f7859-106">Permissions</span></span>
<span data-ttu-id="f7859-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7859-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7859-109">Permission type</span></span>      | <span data-ttu-id="f7859-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7859-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7859-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7859-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f7859-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7859-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f7859-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7859-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7859-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7859-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f7859-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7859-115">Application</span></span> | <span data-ttu-id="f7859-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7859-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7859-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7859-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f7859-118">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7859-118">Optional request headers</span></span>
| <span data-ttu-id="f7859-119">Name</span><span class="sxs-lookup"><span data-stu-id="f7859-119">Name</span></span>       | <span data-ttu-id="f7859-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7859-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f7859-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7859-121">Authorization</span></span>  | <span data-ttu-id="f7859-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f7859-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7859-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7859-124">Request body</span></span>
<span data-ttu-id="f7859-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="f7859-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f7859-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7859-128">Property</span></span>     | <span data-ttu-id="f7859-129">Typ</span><span class="sxs-lookup"><span data-stu-id="f7859-129">Type</span></span>   |<span data-ttu-id="f7859-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7859-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7859-131">name</span><span class="sxs-lookup"><span data-stu-id="f7859-131">name</span></span>|<span data-ttu-id="f7859-132">String</span><span class="sxs-lookup"><span data-stu-id="f7859-132">String</span></span>|<span data-ttu-id="f7859-133">Der Name des Aufgabenordners.</span><span class="sxs-lookup"><span data-stu-id="f7859-133">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="f7859-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7859-134">Response</span></span>

<span data-ttu-id="f7859-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [OutlookTaskFolder](../resources/outlooktaskfolder.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f7859-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7859-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7859-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7859-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7859-137">Request</span></span>
<span data-ttu-id="f7859-138">Das folgende Beispiel ändert den Namen des angegebenen Ordner zu `Charity work`.</span><span class="sxs-lookup"><span data-stu-id="f7859-138">The following example changes the name of the specified task folder to `Charity work`.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f7859-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7859-139">Response</span></span>
<span data-ttu-id="f7859-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7859-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
