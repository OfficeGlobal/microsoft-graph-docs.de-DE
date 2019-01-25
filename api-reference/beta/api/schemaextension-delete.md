---
title: schemaExtension löschen
description: Dient zum Löschen eines schemaExtension-Objekts.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 2a9bdca6459f19c2d397914a2c4818a2331d68c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526004"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="39e05-103">schemaExtension löschen</span><span class="sxs-lookup"><span data-stu-id="39e05-103">Delete schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39e05-104">Dient zum Löschen eines [schemaExtension](../resources/schemaextension.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="39e05-104">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="39e05-p101">Nur die App, mit der die Schemaerweiterung erstellt wurde (Besitzer-App), kann die Schemaerweiterungsdefinition löschen, und zwar nur, wenn die Erweiterung den Status **InDevelopment** aufweist. Das Löschen einer Schemaerweiterungsdefinition hat keinen Einfluss auf den Zugriff auf benutzerdefinierte Daten, die aufgrund dieser Definition zu Ressourceninstanzen hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="39e05-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="39e05-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="39e05-107">Permissions</span></span>
<span data-ttu-id="39e05-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39e05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="39e05-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39e05-110">Permission type</span></span>      | <span data-ttu-id="39e05-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39e05-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39e05-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39e05-112">Delegated (work or school account)</span></span> | <span data-ttu-id="39e05-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="39e05-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="39e05-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39e05-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39e05-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39e05-115">Not supported.</span></span>    |
|<span data-ttu-id="39e05-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39e05-116">Application</span></span> | <span data-ttu-id="39e05-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39e05-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39e05-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39e05-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="39e05-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39e05-119">Request headers</span></span>
| <span data-ttu-id="39e05-120">Name</span><span class="sxs-lookup"><span data-stu-id="39e05-120">Name</span></span>      |<span data-ttu-id="39e05-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39e05-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39e05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="39e05-122">Authorization</span></span>  | <span data-ttu-id="39e05-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="39e05-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39e05-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39e05-125">Request body</span></span>
<span data-ttu-id="39e05-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="39e05-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39e05-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="39e05-127">Response</span></span>

<span data-ttu-id="39e05-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39e05-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39e05-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39e05-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39e05-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39e05-131">Request</span></span>
<span data-ttu-id="39e05-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39e05-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="39e05-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="39e05-133">Response</span></span>
<span data-ttu-id="39e05-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="39e05-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="39e05-135">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="39e05-135">See also</span></span>

- [<span data-ttu-id="39e05-136">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="39e05-136">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="39e05-137">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="39e05-137">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
