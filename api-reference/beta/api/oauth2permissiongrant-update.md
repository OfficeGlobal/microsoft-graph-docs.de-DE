---
title: OAuth2PermissionGrant aktualisieren
description: Aktualisieren Sie die Eigenschaften des oAuth2PermissionGrant-Objekts.
localization_priority: Normal
ms.openlocfilehash: 3c01d62dfb7c0c6906ff860656ee87b5f6d40aed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822351"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="0eb04-103">OAuth2PermissionGrant aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0eb04-103">Update oAuth2PermissionGrant</span></span>

> <span data-ttu-id="0eb04-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0eb04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0eb04-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0eb04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0eb04-106">Aktualisieren Sie die Eigenschaften des oAuth2PermissionGrant-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0eb04-106">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0eb04-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0eb04-107">Permissions</span></span>

<span data-ttu-id="0eb04-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eb04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0eb04-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0eb04-110">Permission type</span></span>      | <span data-ttu-id="0eb04-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0eb04-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0eb04-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0eb04-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0eb04-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0eb04-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0eb04-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0eb04-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eb04-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0eb04-115">Not supported.</span></span>    |
|<span data-ttu-id="0eb04-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0eb04-116">Application</span></span> | <span data-ttu-id="0eb04-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eb04-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0eb04-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0eb04-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0eb04-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0eb04-119">Request headers</span></span>
| <span data-ttu-id="0eb04-120">Name</span><span class="sxs-lookup"><span data-stu-id="0eb04-120">Name</span></span>       | <span data-ttu-id="0eb04-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0eb04-121">Type</span></span> | <span data-ttu-id="0eb04-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0eb04-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0eb04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eb04-123">Authorization</span></span>  | <span data-ttu-id="0eb04-124">string</span><span class="sxs-lookup"><span data-stu-id="0eb04-124">string</span></span>  | <span data-ttu-id="0eb04-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0eb04-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0eb04-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0eb04-127">Request body</span></span>
<span data-ttu-id="0eb04-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="0eb04-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0eb04-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0eb04-131">Property</span></span>     | <span data-ttu-id="0eb04-132">Typ</span><span class="sxs-lookup"><span data-stu-id="0eb04-132">Type</span></span>   |<span data-ttu-id="0eb04-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0eb04-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0eb04-134">scope</span><span class="sxs-lookup"><span data-stu-id="0eb04-134">scope</span></span>|<span data-ttu-id="0eb04-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0eb04-135">String</span></span>| <span data-ttu-id="0eb04-136">Gibt den Wert des Anspruchs Bereich, der die Ressource Anwendung erwarten im Zugriffstoken OAuth 2.0 an.</span><span class="sxs-lookup"><span data-stu-id="0eb04-136">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="0eb04-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="0eb04-137">Response</span></span>

<span data-ttu-id="0eb04-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0eb04-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eb04-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0eb04-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0eb04-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0eb04-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_oAuth2Permissiongrant"
}-->
```http
PATCH https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
Content-type: application/json
Content-length: 30

{
  "scope": "scope-value"
}
```
##### <a name="response"></a><span data-ttu-id="0eb04-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="0eb04-142">Response</span></span>

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
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
