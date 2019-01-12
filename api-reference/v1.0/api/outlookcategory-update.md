---
title: Aktualisieren der Outlook-Kategorie
description: 'Aktualisieren Sie die schreibbare Eigenschaft, **color**, des angegebenen outlookCategory-Objekts. Die **DisplayName** -Eigenschaft kann nicht geändert werden. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 65763a0bffa6536cffe755b6f0435a1d8d666937
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912092"
---
# <a name="update-outlook-category"></a><span data-ttu-id="18321-104">Aktualisieren der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="18321-104">Update Outlook category</span></span>


<span data-ttu-id="18321-105">Aktualisieren Sie die schreibbare Eigenschaft, **color**, des angegebenen [outlookCategory](../resources/outlookcategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="18321-105">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="18321-106">Sie können die **displayName**-Eigenschaft nicht mehr ändern, nachdem die Kategorie erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="18321-106">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="18321-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18321-107">Permissions</span></span>
<span data-ttu-id="18321-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18321-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18321-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18321-110">Permission type</span></span>      | <span data-ttu-id="18321-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18321-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18321-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18321-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18321-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18321-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="18321-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18321-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18321-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18321-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="18321-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18321-116">Application</span></span> | <span data-ttu-id="18321-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18321-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="18321-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18321-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="18321-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18321-119">Request headers</span></span>
| <span data-ttu-id="18321-120">Name</span><span class="sxs-lookup"><span data-stu-id="18321-120">Name</span></span>      |<span data-ttu-id="18321-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18321-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="18321-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18321-122">Authorization</span></span>  | <span data-ttu-id="18321-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18321-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18321-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18321-125">Request body</span></span>
<span data-ttu-id="18321-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="18321-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="18321-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="18321-129">Property</span></span>     | <span data-ttu-id="18321-130">Typ</span><span class="sxs-lookup"><span data-stu-id="18321-130">Type</span></span>   |<span data-ttu-id="18321-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18321-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18321-132">color</span><span class="sxs-lookup"><span data-stu-id="18321-132">color</span></span>|<span data-ttu-id="18321-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="18321-133">String</span></span>|<span data-ttu-id="18321-134">Eine voreingestellte Konstante, die eine Kategorie charakterisiert und einer von 25 vordefinierten Farben zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="18321-134">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="18321-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="18321-135">Response</span></span>

<span data-ttu-id="18321-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [outlookCategory](../resources/outlookcategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18321-136">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18321-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18321-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18321-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18321-138">Request</span></span>
<span data-ttu-id="18321-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18321-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["bac262b7-485d-4739-b436-e31467d64fac"],
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="18321-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="18321-140">Response</span></span>
<span data-ttu-id="18321-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18321-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
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
