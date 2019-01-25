---
title: Aktualisieren der Outlook-Kategorie
description: 'Aktualisieren Sie die schreibbare Eigenschaft, **color**, des angegebenen outlookCategory-Objekts. Die **DisplayName** -Eigenschaft kann nicht geändert werden. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 87c235b670036cb7f4d7e4c20a0e6c700d3843c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523659"
---
# <a name="update-outlook-category"></a><span data-ttu-id="acb05-104">Aktualisieren der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="acb05-104">Update Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acb05-105">Aktualisieren Sie die schreibbare Eigenschaft, **color**, des angegebenen [outlookCategory](../resources/outlookcategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="acb05-105">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="acb05-106">Sie können die **displayName**-Eigenschaft nicht mehr ändern, nachdem die Kategorie erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="acb05-106">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="acb05-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="acb05-107">Permissions</span></span>
<span data-ttu-id="acb05-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acb05-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acb05-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="acb05-110">Permission type</span></span>      | <span data-ttu-id="acb05-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="acb05-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acb05-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="acb05-112">Delegated (work or school account)</span></span> | <span data-ttu-id="acb05-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acb05-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="acb05-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="acb05-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acb05-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acb05-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="acb05-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="acb05-116">Application</span></span> | <span data-ttu-id="acb05-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acb05-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="acb05-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="acb05-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="acb05-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="acb05-119">Request headers</span></span>
| <span data-ttu-id="acb05-120">Name</span><span class="sxs-lookup"><span data-stu-id="acb05-120">Name</span></span>      |<span data-ttu-id="acb05-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acb05-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="acb05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="acb05-122">Authorization</span></span>  | <span data-ttu-id="acb05-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="acb05-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="acb05-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="acb05-125">Request body</span></span>
<span data-ttu-id="acb05-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="acb05-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="acb05-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="acb05-129">Property</span></span>     | <span data-ttu-id="acb05-130">Typ</span><span class="sxs-lookup"><span data-stu-id="acb05-130">Type</span></span>   |<span data-ttu-id="acb05-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acb05-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acb05-132">color</span><span class="sxs-lookup"><span data-stu-id="acb05-132">color</span></span>|<span data-ttu-id="acb05-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="acb05-133">String</span></span>|<span data-ttu-id="acb05-134">Eine voreingestellte Konstante, die eine Kategorie charakterisiert und einer von 25 vordefinierten Farben zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="acb05-134">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="acb05-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="acb05-135">Response</span></span>

<span data-ttu-id="acb05-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [outlookCategory](../resources/outlookcategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acb05-136">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="acb05-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="acb05-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acb05-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="acb05-138">Request</span></span>
<span data-ttu-id="acb05-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="acb05-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/masterCategories('bac262b7-485d-4739-b436-e31467d64fac')
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="acb05-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="acb05-140">Response</span></span>
<span data-ttu-id="acb05-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acb05-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookcategory-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
