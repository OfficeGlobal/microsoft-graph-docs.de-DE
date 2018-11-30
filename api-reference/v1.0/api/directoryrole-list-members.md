---
title: Mitglieder auflisten
description: Dient zum Abrufen einer Liste der Benutzer, die der Verzeichnisrolle zugeordnet sind.  Nur Benutzer können einer Verzeichnisrolle zugewiesen werden.
ms.openlocfilehash: 52ba5ccf1bc7bbd502c53a659978b12faf129f9c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016559"
---
# <a name="list-members"></a><span data-ttu-id="b59c7-104">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="b59c7-104">List members</span></span>

<span data-ttu-id="b59c7-p102">Dient zum Abrufen einer Liste der Benutzer, die der Verzeichnisrolle zugeordnet sind.  Nur Benutzer können einer Verzeichnisrolle zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="b59c7-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="b59c7-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b59c7-107">Permissions</span></span>
<span data-ttu-id="b59c7-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b59c7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b59c7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b59c7-110">Permission type</span></span>      | <span data-ttu-id="b59c7-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b59c7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b59c7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b59c7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b59c7-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b59c7-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b59c7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b59c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b59c7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b59c7-115">Not supported.</span></span>    |
|<span data-ttu-id="b59c7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b59c7-116">Application</span></span> | <span data-ttu-id="b59c7-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b59c7-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b59c7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b59c7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b59c7-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b59c7-119">Optional query parameters</span></span>
<span data-ttu-id="b59c7-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b59c7-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b59c7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b59c7-121">Request headers</span></span>
| <span data-ttu-id="b59c7-122">Name</span><span class="sxs-lookup"><span data-stu-id="b59c7-122">Name</span></span>       | <span data-ttu-id="b59c7-123">Typ</span><span class="sxs-lookup"><span data-stu-id="b59c7-123">Type</span></span> | <span data-ttu-id="b59c7-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b59c7-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b59c7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b59c7-125">Authorization</span></span>  | <span data-ttu-id="b59c7-126">string</span><span class="sxs-lookup"><span data-stu-id="b59c7-126">string</span></span>  | <span data-ttu-id="b59c7-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b59c7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b59c7-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b59c7-129">Request body</span></span>
<span data-ttu-id="b59c7-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b59c7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b59c7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b59c7-131">Response</span></span>

<span data-ttu-id="b59c7-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b59c7-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b59c7-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b59c7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b59c7-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b59c7-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="b59c7-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="b59c7-135">Response</span></span>
<span data-ttu-id="b59c7-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b59c7-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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