---
title: Aktualisieren der Outlook-Kategorie
description: 'Aktualisieren Sie die schreibbare Eigenschaft, **color**, des angegebenen outlookCategory-Objekts. Die **DisplayName** -Eigenschaft kann nicht geändert werden. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f6440708f7083e0b129e48aa0f455b892fd4d157
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965096"
---
# <a name="update-outlook-category"></a><span data-ttu-id="07ce9-104">Aktualisieren der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="07ce9-104">Update Outlook category</span></span>

> <span data-ttu-id="07ce9-105">**Wichtig**: unter der /beta Version von Microsoft Graph-APIs sind in der Vorschau und kann geändert werden.</span><span class="sxs-lookup"><span data-stu-id="07ce9-105">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07ce9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07ce9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07ce9-107">Aktualisieren Sie die schreibbare Eigenschaft, **color**, des angegebenen [outlookCategory](../resources/outlookcategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="07ce9-107">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="07ce9-108">Sie können die **displayName**-Eigenschaft nicht mehr ändern, nachdem die Kategorie erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="07ce9-108">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="07ce9-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07ce9-109">Permissions</span></span>
<span data-ttu-id="07ce9-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07ce9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07ce9-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07ce9-112">Permission type</span></span>      | <span data-ttu-id="07ce9-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07ce9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07ce9-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07ce9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="07ce9-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07ce9-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="07ce9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07ce9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07ce9-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07ce9-117">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="07ce9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07ce9-118">Application</span></span> | <span data-ttu-id="07ce9-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07ce9-119">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="07ce9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07ce9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="07ce9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07ce9-121">Request headers</span></span>
| <span data-ttu-id="07ce9-122">Name</span><span class="sxs-lookup"><span data-stu-id="07ce9-122">Name</span></span>      |<span data-ttu-id="07ce9-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07ce9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07ce9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="07ce9-124">Authorization</span></span>  | <span data-ttu-id="07ce9-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07ce9-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07ce9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07ce9-127">Request body</span></span>
<span data-ttu-id="07ce9-p106">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="07ce9-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="07ce9-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07ce9-131">Property</span></span>     | <span data-ttu-id="07ce9-132">Typ</span><span class="sxs-lookup"><span data-stu-id="07ce9-132">Type</span></span>   |<span data-ttu-id="07ce9-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07ce9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07ce9-134">color</span><span class="sxs-lookup"><span data-stu-id="07ce9-134">color</span></span>|<span data-ttu-id="07ce9-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07ce9-135">String</span></span>|<span data-ttu-id="07ce9-136">Eine voreingestellte Konstante, die eine Kategorie charakterisiert und einer von 25 vordefinierten Farben zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="07ce9-136">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="07ce9-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="07ce9-137">Response</span></span>

<span data-ttu-id="07ce9-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [outlookCategory](../resources/outlookcategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07ce9-138">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07ce9-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07ce9-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07ce9-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07ce9-140">Request</span></span>
<span data-ttu-id="07ce9-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="07ce9-141">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="07ce9-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="07ce9-142">Response</span></span>
<span data-ttu-id="07ce9-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07ce9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
