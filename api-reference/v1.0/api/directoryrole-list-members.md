---
title: Mitglieder auflisten
description: Dient zum Abrufen einer Liste der Benutzer, die der Verzeichnisrolle zugeordnet sind.  Nur Benutzer können einer Verzeichnisrolle zugewiesen werden.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: c1e58a7705abeafa56acde7e1d069a346ac3881a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805481"
---
# <a name="list-members"></a><span data-ttu-id="6977e-104">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="6977e-104">List members</span></span>

<span data-ttu-id="6977e-p102">Dient zum Abrufen einer Liste der Benutzer, die der Verzeichnisrolle zugeordnet sind.  Nur Benutzer können einer Verzeichnisrolle zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="6977e-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="6977e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6977e-107">Permissions</span></span>
<span data-ttu-id="6977e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6977e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6977e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6977e-110">Permission type</span></span>      | <span data-ttu-id="6977e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6977e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6977e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6977e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6977e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6977e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6977e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6977e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6977e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6977e-115">Not supported.</span></span>    |
|<span data-ttu-id="6977e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6977e-116">Application</span></span> | <span data-ttu-id="6977e-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6977e-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6977e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6977e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6977e-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6977e-119">Optional query parameters</span></span>
<span data-ttu-id="6977e-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6977e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6977e-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6977e-121">Request headers</span></span>
| <span data-ttu-id="6977e-122">Name</span><span class="sxs-lookup"><span data-stu-id="6977e-122">Name</span></span>       | <span data-ttu-id="6977e-123">Typ</span><span class="sxs-lookup"><span data-stu-id="6977e-123">Type</span></span> | <span data-ttu-id="6977e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6977e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6977e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6977e-125">Authorization</span></span>  | <span data-ttu-id="6977e-126">string</span><span class="sxs-lookup"><span data-stu-id="6977e-126">string</span></span>  | <span data-ttu-id="6977e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6977e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6977e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6977e-129">Request body</span></span>
<span data-ttu-id="6977e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6977e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6977e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6977e-131">Response</span></span>

<span data-ttu-id="6977e-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6977e-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6977e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6977e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6977e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6977e-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="6977e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6977e-135">Response</span></span>
<span data-ttu-id="6977e-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6977e-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
