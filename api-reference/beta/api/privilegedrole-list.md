---
title: Liste privilegedRoles
description: Abrufen einer Liste von PrivilegedRole-Objekten.
localization_priority: Normal
ms.openlocfilehash: d954cedbaf4b164fe0649a3565ea0212d148c322
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518079"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="e7caf-103">Liste privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="e7caf-103">List privilegedRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7caf-104">Abrufen einer Liste von [PrivilegedRole](../resources/privilegedrole.md) -Objekten.</span><span class="sxs-lookup"><span data-stu-id="e7caf-104">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="e7caf-105">Verwenden Sie zum Filtern der Ergebnisse der Abfrage, die standard-OData ``$filter`` Ausdrücke in die URIs.</span><span class="sxs-lookup"><span data-stu-id="e7caf-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7caf-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e7caf-106">Permissions</span></span>
<span data-ttu-id="e7caf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7caf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e7caf-109">Der Requestor muss eine der folgenden Rollen verfügen: _Berechtigten Rolle Administrators_, _Globaler Administrator_, _Sicherheitsadministrator_oder _Sicherheit Leser_.</span><span class="sxs-lookup"><span data-stu-id="e7caf-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="e7caf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e7caf-110">Permission type</span></span>      | <span data-ttu-id="e7caf-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e7caf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7caf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e7caf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e7caf-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e7caf-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e7caf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e7caf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7caf-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7caf-115">Not supported.</span></span>    |
|<span data-ttu-id="e7caf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e7caf-116">Application</span></span> | <span data-ttu-id="e7caf-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7caf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7caf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7caf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7caf-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e7caf-119">Optional query parameters</span></span>
<span data-ttu-id="e7caf-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e7caf-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7caf-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e7caf-121">Request headers</span></span>
| <span data-ttu-id="e7caf-122">Name</span><span class="sxs-lookup"><span data-stu-id="e7caf-122">Name</span></span>      |<span data-ttu-id="e7caf-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7caf-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e7caf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7caf-124">Authorization</span></span>  | <span data-ttu-id="e7caf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e7caf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7caf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e7caf-127">Request body</span></span>
<span data-ttu-id="e7caf-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e7caf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7caf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7caf-129">Response</span></span>

<span data-ttu-id="e7caf-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [PrivilegedRole](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="e7caf-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="e7caf-131">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="e7caf-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="e7caf-132">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="e7caf-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="e7caf-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e7caf-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7caf-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7caf-134">Request</span></span>
<span data-ttu-id="e7caf-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e7caf-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
##### <a name="response"></a><span data-ttu-id="e7caf-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7caf-136">Response</span></span>
<span data-ttu-id="e7caf-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e7caf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
