---
title: Outlooktaskfolder aktualisieren
description: Aktualisieren Sie die schreibbaren Eigenschaften des Ordners eine Outlook-Aufgabe.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af86b85df5529f7f8c15ce2e4977d4b0fe2f00ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925679"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="4b2ef-103">Outlooktaskfolder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4b2ef-103">Update outlooktaskfolder</span></span>

> <span data-ttu-id="4b2ef-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b2ef-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b2ef-106">Aktualisieren Sie die schreibbaren Eigenschaften des Ordners eine Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-106">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="4b2ef-107">Sie können den **Name** -Eigenschaftswert der Aufgabe Standardordner "Aufgaben" nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-107">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="4b2ef-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4b2ef-108">Permissions</span></span>
<span data-ttu-id="4b2ef-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b2ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b2ef-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b2ef-111">Permission type</span></span>      | <span data-ttu-id="4b2ef-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b2ef-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b2ef-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b2ef-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4b2ef-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b2ef-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4b2ef-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b2ef-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b2ef-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b2ef-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4b2ef-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b2ef-117">Application</span></span> | <span data-ttu-id="4b2ef-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b2ef-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b2ef-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b2ef-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4b2ef-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b2ef-120">Optional request headers</span></span>
| <span data-ttu-id="4b2ef-121">Name</span><span class="sxs-lookup"><span data-stu-id="4b2ef-121">Name</span></span>       | <span data-ttu-id="4b2ef-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b2ef-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4b2ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b2ef-123">Authorization</span></span>  | <span data-ttu-id="4b2ef-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b2ef-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b2ef-126">Request body</span></span>
<span data-ttu-id="4b2ef-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4b2ef-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b2ef-130">Property</span></span>     | <span data-ttu-id="4b2ef-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4b2ef-131">Type</span></span>   |<span data-ttu-id="4b2ef-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b2ef-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b2ef-133">name</span><span class="sxs-lookup"><span data-stu-id="4b2ef-133">name</span></span>|<span data-ttu-id="4b2ef-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b2ef-134">String</span></span>|<span data-ttu-id="4b2ef-135">Der Name des Aufgabenordners.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-135">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="4b2ef-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b2ef-136">Response</span></span>

<span data-ttu-id="4b2ef-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [OutlookTaskFolder](../resources/outlooktaskfolder.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-137">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b2ef-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b2ef-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b2ef-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b2ef-139">Request</span></span>
<span data-ttu-id="4b2ef-140">Das folgende Beispiel ändert den Namen des angegebenen Ordner zu `Charity work`.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-140">The following example changes the name of the specified task folder to `Charity work`.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4b2ef-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b2ef-141">Response</span></span>
<span data-ttu-id="4b2ef-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b2ef-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
