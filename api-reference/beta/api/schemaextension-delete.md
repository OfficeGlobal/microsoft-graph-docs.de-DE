---
title: schemaExtension löschen
description: Dient zum Löschen eines schemaExtension-Objekts.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 96b7ab5091d7e8a33bd3e94fea4a9ccc85a686fb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962800"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="1f56c-103">schemaExtension löschen</span><span class="sxs-lookup"><span data-stu-id="1f56c-103">Delete schemaExtension</span></span>

> <span data-ttu-id="1f56c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1f56c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f56c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f56c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f56c-106">Dient zum Löschen eines [schemaExtension](../resources/schemaextension.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f56c-106">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="1f56c-p102">Nur die App, mit der die Schemaerweiterung erstellt wurde (Besitzer-App), kann die Schemaerweiterungsdefinition löschen, und zwar nur, wenn die Erweiterung den Status **InDevelopment** aufweist. Das Löschen einer Schemaerweiterungsdefinition hat keinen Einfluss auf den Zugriff auf benutzerdefinierte Daten, die aufgrund dieser Definition zu Ressourceninstanzen hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="1f56c-p102">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="1f56c-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1f56c-109">Permissions</span></span>
<span data-ttu-id="1f56c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f56c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1f56c-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f56c-112">Permission type</span></span>      | <span data-ttu-id="1f56c-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f56c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f56c-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f56c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1f56c-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1f56c-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1f56c-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f56c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f56c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f56c-117">Not supported.</span></span>    |
|<span data-ttu-id="1f56c-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f56c-118">Application</span></span> | <span data-ttu-id="1f56c-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f56c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f56c-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f56c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1f56c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f56c-121">Request headers</span></span>
| <span data-ttu-id="1f56c-122">Name</span><span class="sxs-lookup"><span data-stu-id="1f56c-122">Name</span></span>      |<span data-ttu-id="1f56c-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f56c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f56c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f56c-124">Authorization</span></span>  | <span data-ttu-id="1f56c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f56c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f56c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f56c-127">Request body</span></span>
<span data-ttu-id="1f56c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1f56c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f56c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f56c-129">Response</span></span>

<span data-ttu-id="1f56c-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f56c-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f56c-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f56c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f56c-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f56c-133">Request</span></span>
<span data-ttu-id="1f56c-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f56c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="1f56c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f56c-135">Response</span></span>
<span data-ttu-id="1f56c-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f56c-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="1f56c-137">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="1f56c-137">See also</span></span>

- [<span data-ttu-id="1f56c-138">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="1f56c-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1f56c-139">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="1f56c-139">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
