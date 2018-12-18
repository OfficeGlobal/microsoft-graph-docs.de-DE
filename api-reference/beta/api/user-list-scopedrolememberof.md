---
title: scopedAdministratorOf auflisten
description: Abrufen einer Liste der ScopedRoleMembership für den Benutzer.
author: dkershaw10
ms.openlocfilehash: 48aead850e7f7b90a38229da1016007aeec40a9d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357344"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="23077-103">scopedAdministratorOf auflisten</span><span class="sxs-lookup"><span data-stu-id="23077-103">List scopedAdministratorOf</span></span>

> <span data-ttu-id="23077-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23077-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23077-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23077-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23077-106">Abrufen einer Liste der [ScopedRoleMembership](../resources/scopedrolemembership.md) für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="23077-106">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="23077-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="23077-107">Permissions</span></span>
<span data-ttu-id="23077-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23077-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="23077-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23077-110">Permission type</span></span>      | <span data-ttu-id="23077-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23077-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23077-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23077-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23077-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23077-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="23077-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23077-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23077-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23077-115">Not supported.</span></span>    |
|<span data-ttu-id="23077-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23077-116">Application</span></span> | <span data-ttu-id="23077-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23077-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23077-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23077-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedAdministratorOf
GET /users/{id}/scopedAdministratorOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="23077-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="23077-119">Optional query parameters</span></span>
<span data-ttu-id="23077-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="23077-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23077-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23077-121">Request headers</span></span>
| <span data-ttu-id="23077-122">Header</span><span class="sxs-lookup"><span data-stu-id="23077-122">Header</span></span>       | <span data-ttu-id="23077-123">Wert</span><span class="sxs-lookup"><span data-stu-id="23077-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="23077-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="23077-124">Authorization</span></span>  | <span data-ttu-id="23077-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23077-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="23077-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23077-127">Request body</span></span>
<span data-ttu-id="23077-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="23077-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23077-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="23077-129">Response</span></span>

<span data-ttu-id="23077-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [ScopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="23077-130">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23077-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23077-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23077-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23077-132">Request</span></span>
<span data-ttu-id="23077-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="23077-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```http
GET https://graph.microsoft.com/beta/me/scopedAdministratorOf
```
##### <a name="response"></a><span data-ttu-id="23077-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="23077-134">Response</span></span>
<span data-ttu-id="23077-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23077-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      },
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List scopedAdministratorOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->