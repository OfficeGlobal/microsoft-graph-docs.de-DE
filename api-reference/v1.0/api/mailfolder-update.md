---
title: mailfolder aktualisieren
description: Mit dieser API können Sie Eigenschaften eines Objekts des Typs „mailfolder“ aktualisieren.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: e2ce809c75a911b7d68ed80692a14a537c659d37
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871631"
---
# <a name="update-mailfolder"></a><span data-ttu-id="3b19d-103">mailfolder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3b19d-103">Update mailfolder</span></span>

<span data-ttu-id="3b19d-104">Mit dieser API können Sie Eigenschaften eines Objekts des Typs „mailfolder“ aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="3b19d-104">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b19d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3b19d-105">Permissions</span></span>
<span data-ttu-id="3b19d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b19d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b19d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b19d-108">Permission type</span></span>      | <span data-ttu-id="3b19d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b19d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b19d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b19d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3b19d-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b19d-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3b19d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b19d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b19d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b19d-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3b19d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b19d-114">Application</span></span> | <span data-ttu-id="3b19d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b19d-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b19d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b19d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3b19d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b19d-117">Request headers</span></span>
| <span data-ttu-id="3b19d-118">Header</span><span class="sxs-lookup"><span data-stu-id="3b19d-118">Header</span></span>       | <span data-ttu-id="3b19d-119">Wert</span><span class="sxs-lookup"><span data-stu-id="3b19d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b19d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b19d-120">Authorization</span></span>  | <span data-ttu-id="3b19d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b19d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3b19d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b19d-123">Content-Type</span></span>  | <span data-ttu-id="3b19d-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="3b19d-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b19d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b19d-126">Request body</span></span>
<span data-ttu-id="3b19d-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="3b19d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3b19d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b19d-130">Property</span></span>     | <span data-ttu-id="3b19d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3b19d-131">Type</span></span>   |<span data-ttu-id="3b19d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b19d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b19d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3b19d-133">displayName</span></span>|<span data-ttu-id="3b19d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b19d-134">String</span></span>|<span data-ttu-id="3b19d-135">Der Anzeigename des mailFolder-Elements.</span><span class="sxs-lookup"><span data-stu-id="3b19d-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="3b19d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b19d-136">Response</span></span>

<span data-ttu-id="3b19d-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [mailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b19d-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b19d-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b19d-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b19d-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b19d-139">Request</span></span>
<span data-ttu-id="3b19d-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b19d-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/{id}
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
##### <a name="response"></a><span data-ttu-id="3b19d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b19d-141">Response</span></span>
<span data-ttu-id="3b19d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b19d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
