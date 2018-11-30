---
title: schemaExtension abrufen
description: Mit dieser API können Sie die Eigenschaften der angegebenen Definition des Typs schemaExtension abrufen.
ms.openlocfilehash: 32376d6afd0d6171362db1978b708610d9f4d056
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063943"
---
# <a name="get-schemaextension"></a><span data-ttu-id="c7605-103">schemaExtension abrufen</span><span class="sxs-lookup"><span data-stu-id="c7605-103">Get schemaExtension</span></span>

> <span data-ttu-id="c7605-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c7605-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7605-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7605-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7605-106">Mit dieser API können Sie die Eigenschaften der angegebenen Definition des Typs [schemaExtension](../resources/schemaextension.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="c7605-106">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7605-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c7605-107">Permissions</span></span>
<span data-ttu-id="c7605-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7605-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c7605-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7605-110">Permission type</span></span>      | <span data-ttu-id="c7605-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7605-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7605-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7605-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c7605-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c7605-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c7605-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7605-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7605-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7605-115">Not supported.</span></span>    |
|<span data-ttu-id="c7605-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7605-116">Application</span></span> | <span data-ttu-id="c7605-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7605-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7605-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7605-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c7605-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c7605-119">Optional query parameters</span></span>
<span data-ttu-id="c7605-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c7605-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7605-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7605-121">Request headers</span></span>
| <span data-ttu-id="c7605-122">Name</span><span class="sxs-lookup"><span data-stu-id="c7605-122">Name</span></span>      |<span data-ttu-id="c7605-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7605-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7605-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7605-124">Authorization</span></span>  | <span data-ttu-id="c7605-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c7605-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7605-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7605-127">Content-Type</span></span>   | <span data-ttu-id="c7605-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c7605-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7605-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7605-129">Request body</span></span>
<span data-ttu-id="c7605-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c7605-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7605-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7605-131">Response</span></span>

<span data-ttu-id="c7605-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [schemaExtension](../resources/schemaextension.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7605-132">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7605-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7605-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7605-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7605-134">Request</span></span>
<span data-ttu-id="c7605-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7605-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="c7605-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7605-136">Response</span></span>
<span data-ttu-id="c7605-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7605-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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

## <a name="see-also"></a><span data-ttu-id="c7605-140">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="c7605-140">See also</span></span>

- [<span data-ttu-id="c7605-141">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="c7605-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c7605-142">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="c7605-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->