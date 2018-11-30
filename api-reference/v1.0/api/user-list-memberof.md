---
title: memberOf auflisten
description: 'Dient zum Abrufen von Gruppen- und Verzeichnisrollen, vondenen der Benutzer ein direktes Mitglied ist. '
ms.openlocfilehash: 6d884868be083a3d547002760560816e10984436
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019660"
---
# <a name="list-memberof"></a><span data-ttu-id="e955a-103">memberOf auflisten</span><span class="sxs-lookup"><span data-stu-id="e955a-103">List memberOf</span></span>

<span data-ttu-id="e955a-104">Mit dieser API können Sie die [Gruppen](../resources/group.md) und [Verzeichnisrollen](../resources/directoryrole.md) abrufen, denen ein Benutzer als direktes Mitglied zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="e955a-104">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e955a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e955a-105">Permissions</span></span>
<span data-ttu-id="e955a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e955a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e955a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e955a-108">Permission type</span></span>      | <span data-ttu-id="e955a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e955a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e955a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e955a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e955a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e955a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e955a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e955a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e955a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e955a-113">Not supported.</span></span>    |
|<span data-ttu-id="e955a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e955a-114">Application</span></span> | <span data-ttu-id="e955a-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e955a-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e955a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e955a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e955a-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e955a-117">Optional query parameters</span></span>
<span data-ttu-id="e955a-p102">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort. $filter wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e955a-p102">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response. $filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="e955a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e955a-120">Request headers</span></span>
| <span data-ttu-id="e955a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e955a-121">Header</span></span>       | <span data-ttu-id="e955a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e955a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e955a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e955a-123">Authorization</span></span>  | <span data-ttu-id="e955a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e955a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e955a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e955a-126">Accept</span></span>  | <span data-ttu-id="e955a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e955a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e955a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e955a-128">Request body</span></span>
<span data-ttu-id="e955a-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e955a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e955a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="e955a-130">Response</span></span>

<span data-ttu-id="e955a-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e955a-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e955a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e955a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e955a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e955a-133">Request</span></span>
<span data-ttu-id="e955a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e955a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="e955a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e955a-135">Response</span></span>
<span data-ttu-id="e955a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e955a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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