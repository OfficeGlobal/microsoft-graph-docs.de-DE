---
title: schemaExtensions auflisten
description: 'Abrufen einer Liste von SchemaExtension-Objekten erstellt mithilfe von apps, die Sie in den aktuellen Mandanten besitzen (das werden kann '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 21e9cb1d202bd76abd71860b14a8c58856132ba1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945167"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="24c57-103">schemaExtensions auflisten</span><span class="sxs-lookup"><span data-stu-id="24c57-103">List schemaExtensions</span></span>

> <span data-ttu-id="24c57-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="24c57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24c57-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24c57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24c57-106">Dient zum Abrufen einer Liste von [schemaExtension](../resources/schemaextension.md)-Objekten, die von beliebigen Apps erstellt wurden, die Sie im aktuellen Mandanten besitzen (kann **InDevelopment**, **Available** oder **Deprecated** sein), sowie aller anderen Schemaerweiterungen im Besitz von anderen Apps, die als **Available** gekennzeichnet sind.</span><span class="sxs-lookup"><span data-stu-id="24c57-106">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="24c57-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="24c57-107">Permissions</span></span>
<span data-ttu-id="24c57-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24c57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="24c57-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24c57-110">Permission type</span></span>      | <span data-ttu-id="24c57-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24c57-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24c57-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24c57-112">Delegated (work or school account)</span></span> | <span data-ttu-id="24c57-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="24c57-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="24c57-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24c57-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24c57-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24c57-115">Not supported.</span></span>    |
|<span data-ttu-id="24c57-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24c57-116">Application</span></span> | <span data-ttu-id="24c57-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="24c57-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24c57-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24c57-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="24c57-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="24c57-119">Optional query parameters</span></span>
<span data-ttu-id="24c57-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24c57-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24c57-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24c57-121">Request headers</span></span>
| <span data-ttu-id="24c57-122">Name</span><span class="sxs-lookup"><span data-stu-id="24c57-122">Name</span></span>      |<span data-ttu-id="24c57-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24c57-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="24c57-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="24c57-124">Authorization</span></span>  | <span data-ttu-id="24c57-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24c57-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24c57-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24c57-127">Content-Type</span></span>   | <span data-ttu-id="24c57-128">application/json</span><span class="sxs-lookup"><span data-stu-id="24c57-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="24c57-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="24c57-129">Request body</span></span>
<span data-ttu-id="24c57-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="24c57-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24c57-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="24c57-131">Response</span></span>

<span data-ttu-id="24c57-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [schemaExtension](../resources/schemaextension.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24c57-132">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24c57-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24c57-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24c57-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24c57-134">Request</span></span>
<span data-ttu-id="24c57-135">Im folgenden Beispiel wird gezeigt, wie Sie unter allen zugänglichen Erweiterungen nach einer bestimmten Erweiterung suchen, indem Sie nach ihrer eindeutigen **ID** filtern.</span><span class="sxs-lookup"><span data-stu-id="24c57-135">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="24c57-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="24c57-136">Response</span></span>
<span data-ttu-id="24c57-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24c57-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 274

{
  "value": [
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
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="24c57-140">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="24c57-140">See also</span></span>

- [<span data-ttu-id="24c57-141">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="24c57-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="24c57-142">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="24c57-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
