---
title: memberOf auflisten
description: 'Dient zum Abrufen von Gruppen- und Verzeichnisrollen, vondenen der Benutzer ein direktes Mitglied ist. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 389cbe5a62b75e9396077d9710c0b92a497e8bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962527"
---
# <a name="list-memberof"></a><span data-ttu-id="e83d4-103">memberOf auflisten</span><span class="sxs-lookup"><span data-stu-id="e83d4-103">List memberOf</span></span>

<span data-ttu-id="e83d4-104">Mit dieser API können Sie die [Gruppen](../resources/group.md) und [Verzeichnisrollen](../resources/directoryrole.md) abrufen, denen ein Benutzer als direktes Mitglied zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="e83d4-104">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e83d4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e83d4-105">Permissions</span></span>
<span data-ttu-id="e83d4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e83d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e83d4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e83d4-108">Permission type</span></span>      | <span data-ttu-id="e83d4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e83d4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e83d4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e83d4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e83d4-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e83d4-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e83d4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e83d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e83d4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e83d4-113">Not supported.</span></span>    |
|<span data-ttu-id="e83d4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e83d4-114">Application</span></span> | <span data-ttu-id="e83d4-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e83d4-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e83d4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e83d4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e83d4-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e83d4-117">Optional query parameters</span></span>
<span data-ttu-id="e83d4-p102">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort. $filter wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e83d4-p102">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response. $filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="e83d4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e83d4-120">Request headers</span></span>
| <span data-ttu-id="e83d4-121">Header</span><span class="sxs-lookup"><span data-stu-id="e83d4-121">Header</span></span>       | <span data-ttu-id="e83d4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e83d4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e83d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e83d4-123">Authorization</span></span>  | <span data-ttu-id="e83d4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e83d4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e83d4-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e83d4-126">Accept</span></span>  | <span data-ttu-id="e83d4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e83d4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e83d4-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e83d4-128">Request body</span></span>
<span data-ttu-id="e83d4-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e83d4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e83d4-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="e83d4-130">Response</span></span>

<span data-ttu-id="e83d4-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e83d4-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e83d4-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e83d4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e83d4-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e83d4-133">Request</span></span>
<span data-ttu-id="e83d4-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e83d4-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="e83d4-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e83d4-135">Response</span></span>
<span data-ttu-id="e83d4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e83d4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
