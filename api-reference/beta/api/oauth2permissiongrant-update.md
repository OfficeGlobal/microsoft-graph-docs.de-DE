---
title: OAuth2PermissionGrant aktualisieren
description: Aktualisieren Sie die Eigenschaften des oAuth2PermissionGrant-Objekts.
localization_priority: Normal
ms.openlocfilehash: fb990c56b4d7ae62ac35935a91d69688b96bff28
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522140"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="5ff94-103">OAuth2PermissionGrant aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5ff94-103">Update oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ff94-104">Aktualisieren Sie die Eigenschaften des oAuth2PermissionGrant-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5ff94-104">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ff94-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5ff94-105">Permissions</span></span>

<span data-ttu-id="5ff94-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ff94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5ff94-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5ff94-108">Permission type</span></span>      | <span data-ttu-id="5ff94-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5ff94-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ff94-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5ff94-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5ff94-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5ff94-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5ff94-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5ff94-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ff94-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ff94-113">Not supported.</span></span>    |
|<span data-ttu-id="5ff94-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5ff94-114">Application</span></span> | <span data-ttu-id="5ff94-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff94-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ff94-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ff94-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5ff94-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5ff94-117">Request headers</span></span>
| <span data-ttu-id="5ff94-118">Name</span><span class="sxs-lookup"><span data-stu-id="5ff94-118">Name</span></span>       | <span data-ttu-id="5ff94-119">Typ</span><span class="sxs-lookup"><span data-stu-id="5ff94-119">Type</span></span> | <span data-ttu-id="5ff94-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ff94-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5ff94-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ff94-121">Authorization</span></span>  | <span data-ttu-id="5ff94-122">string</span><span class="sxs-lookup"><span data-stu-id="5ff94-122">string</span></span>  | <span data-ttu-id="5ff94-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5ff94-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ff94-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5ff94-125">Request body</span></span>
<span data-ttu-id="5ff94-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="5ff94-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5ff94-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5ff94-129">Property</span></span>     | <span data-ttu-id="5ff94-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5ff94-130">Type</span></span>   |<span data-ttu-id="5ff94-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ff94-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ff94-132">scope</span><span class="sxs-lookup"><span data-stu-id="5ff94-132">scope</span></span>|<span data-ttu-id="5ff94-133">String</span><span class="sxs-lookup"><span data-stu-id="5ff94-133">String</span></span>| <span data-ttu-id="5ff94-134">Gibt den Wert des Anspruchs Bereich, der die Ressource Anwendung erwarten im Zugriffstoken OAuth 2.0 an.</span><span class="sxs-lookup"><span data-stu-id="5ff94-134">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="5ff94-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ff94-135">Response</span></span>

<span data-ttu-id="5ff94-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5ff94-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ff94-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ff94-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ff94-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ff94-139">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="5ff94-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ff94-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
