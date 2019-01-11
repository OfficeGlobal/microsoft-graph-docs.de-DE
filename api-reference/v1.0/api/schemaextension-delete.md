---
title: schemaExtension löschen
description: Dient zum Löschen eines schemaExtension-Objekts.
localization_priority: Normal
ms.openlocfilehash: 8e9279377810c4895c5327afc64b85f421e8b221
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831600"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="0d4eb-103">schemaExtension löschen</span><span class="sxs-lookup"><span data-stu-id="0d4eb-103">Delete schemaExtension</span></span>

<span data-ttu-id="0d4eb-104">Dient zum Löschen eines [schemaExtension](../resources/schemaextension.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d4eb-104">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="0d4eb-p101">Nur die App, mit der die Schemaerweiterung erstellt wurde (Besitzer-App), kann die Schemaerweiterungsdefinition löschen, und zwar nur, wenn die Erweiterung den Status **InDevelopment** aufweist. Das Löschen einer Schemaerweiterungsdefinition hat keinen Einfluss auf den Zugriff auf benutzerdefinierte Daten, die aufgrund dieser Definition zu Ressourceninstanzen hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="0d4eb-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="0d4eb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0d4eb-107">Permissions</span></span>
<span data-ttu-id="0d4eb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d4eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0d4eb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d4eb-110">Permission type</span></span>      | <span data-ttu-id="0d4eb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d4eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d4eb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d4eb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0d4eb-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d4eb-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d4eb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d4eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d4eb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d4eb-115">Not supported.</span></span>    |
|<span data-ttu-id="0d4eb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d4eb-116">Application</span></span> | <span data-ttu-id="0d4eb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d4eb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d4eb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d4eb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0d4eb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d4eb-119">Request headers</span></span>
| <span data-ttu-id="0d4eb-120">Name</span><span class="sxs-lookup"><span data-stu-id="0d4eb-120">Name</span></span>      |<span data-ttu-id="0d4eb-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d4eb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d4eb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d4eb-122">Authorization</span></span>  | <span data-ttu-id="0d4eb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0d4eb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d4eb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d4eb-125">Request body</span></span>
<span data-ttu-id="0d4eb-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0d4eb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d4eb-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d4eb-127">Response</span></span>

<span data-ttu-id="0d4eb-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d4eb-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d4eb-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d4eb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d4eb-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d4eb-131">Request</span></span>
<span data-ttu-id="0d4eb-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d4eb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="0d4eb-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d4eb-133">Response</span></span>
<span data-ttu-id="0d4eb-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0d4eb-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="0d4eb-135">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="0d4eb-135">See also</span></span>

- [<span data-ttu-id="0d4eb-136">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="0d4eb-136">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0d4eb-137">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="0d4eb-137">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
