---
title: schemaExtension abrufen
description: Mit dieser API können Sie die Eigenschaften der angegebenen Definition des Typs schemaExtension abrufen.
ms.openlocfilehash: bbb2b93d7ba66d6d18d854187a89e3dc2ecc22ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017412"
---
# <a name="get-schemaextension"></a><span data-ttu-id="5123b-103">schemaExtension abrufen</span><span class="sxs-lookup"><span data-stu-id="5123b-103">Get schemaExtension</span></span>
<span data-ttu-id="5123b-104">Mit dieser API können Sie die Eigenschaften der angegebenen Definition des Typs [schemaExtension](../resources/schemaextension.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="5123b-104">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="5123b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5123b-105">Permissions</span></span>
<span data-ttu-id="5123b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5123b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5123b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5123b-108">Permission type</span></span>      | <span data-ttu-id="5123b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5123b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5123b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5123b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5123b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5123b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5123b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5123b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5123b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5123b-113">Not supported.</span></span>    |
|<span data-ttu-id="5123b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5123b-114">Application</span></span> | <span data-ttu-id="5123b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5123b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5123b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5123b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5123b-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5123b-117">Optional query parameters</span></span>
<span data-ttu-id="5123b-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5123b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5123b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5123b-119">Request headers</span></span>
| <span data-ttu-id="5123b-120">Name</span><span class="sxs-lookup"><span data-stu-id="5123b-120">Name</span></span>      |<span data-ttu-id="5123b-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5123b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5123b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5123b-122">Authorization</span></span>  | <span data-ttu-id="5123b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5123b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5123b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5123b-125">Content-Type</span></span>   | <span data-ttu-id="5123b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5123b-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5123b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5123b-127">Request body</span></span>
<span data-ttu-id="5123b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5123b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5123b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5123b-129">Response</span></span>

<span data-ttu-id="5123b-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [schemaExtension](../resources/schemaextension.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5123b-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5123b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5123b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5123b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5123b-132">Request</span></span>
<span data-ttu-id="5123b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5123b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="5123b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5123b-134">Response</span></span>
<span data-ttu-id="5123b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5123b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "id":"graphlearn_test",
    "description": "Yet another test schema",
    "targetTypes": [
        "User", "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "testName",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="5123b-138">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5123b-138">See also</span></span>

- [<span data-ttu-id="5123b-139">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5123b-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5123b-140">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="5123b-140">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->