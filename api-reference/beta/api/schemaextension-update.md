---
title: schemaExtension aktualisieren
description: Dient zum Aktualisieren der Eigenschaften in der Definition der angegebenen schemaExtension.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: f457609af15716ef2ada3945132afd285fd2394c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515538"
---
# <a name="update-schemaextension"></a><span data-ttu-id="60c2c-103">schemaExtension aktualisieren</span><span class="sxs-lookup"><span data-stu-id="60c2c-103">Update schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60c2c-104">Dient zum Aktualisieren der Eigenschaften in der Definition der angegebenen [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="60c2c-104">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="60c2c-p101">Die Aktualisierung gilt für alle Ressourcen, die in der Eigenschaft **targetTypes** der Erweiterung enthalten sind. Diese Ressourcen gehören zu den [unterstützenden Ressourcentypen](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="60c2c-p101">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="60c2c-p102">Nur die App, mit der eine Schemaerweiterung erstellt wurde (Besitzer-App), kann additive Aktualisierungen an der Erweiterung vornehmen, wenn die Erweiterung den Status **InDevelopment** oder **Available** aufweist. Dies bedeutet, dass die App keine benutzerdefinierten Eigenschaften oder Zielressourcentypen aus der Definition entfernen kann. Die App kann jedoch die Beschreibung der Erweiterung ändern.</span><span class="sxs-lookup"><span data-stu-id="60c2c-p102">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="60c2c-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="60c2c-110">Permissions</span></span>

<span data-ttu-id="60c2c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60c2c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="60c2c-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="60c2c-113">Permission type</span></span>      | <span data-ttu-id="60c2c-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="60c2c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60c2c-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="60c2c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="60c2c-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60c2c-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="60c2c-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="60c2c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60c2c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60c2c-118">Not supported.</span></span>    |
|<span data-ttu-id="60c2c-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="60c2c-119">Application</span></span> | <span data-ttu-id="60c2c-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60c2c-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60c2c-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="60c2c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="60c2c-122">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="60c2c-122">Optional request headers</span></span>

| <span data-ttu-id="60c2c-123">Name</span><span class="sxs-lookup"><span data-stu-id="60c2c-123">Name</span></span>      |<span data-ttu-id="60c2c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60c2c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60c2c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="60c2c-125">Authorization</span></span>  | <span data-ttu-id="60c2c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="60c2c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60c2c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60c2c-128">Content-Type</span></span>   | <span data-ttu-id="60c2c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="60c2c-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="60c2c-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="60c2c-130">Request body</span></span>

<span data-ttu-id="60c2c-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="60c2c-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="60c2c-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60c2c-134">Property</span></span>   | <span data-ttu-id="60c2c-135">Typ</span><span class="sxs-lookup"><span data-stu-id="60c2c-135">Type</span></span> |<span data-ttu-id="60c2c-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60c2c-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60c2c-137">description</span><span class="sxs-lookup"><span data-stu-id="60c2c-137">description</span></span>|<span data-ttu-id="60c2c-138">String</span><span class="sxs-lookup"><span data-stu-id="60c2c-138">String</span></span>|<span data-ttu-id="60c2c-139">Beschreibung für die Schemaerweiterung.</span><span class="sxs-lookup"><span data-stu-id="60c2c-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="60c2c-140">properties</span><span class="sxs-lookup"><span data-stu-id="60c2c-140">properties</span></span>|<span data-ttu-id="60c2c-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="60c2c-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="60c2c-p106">Die Sammlung von Eigenschaftennamen und Typen, die die Schemaerweiterungsdefinition bilden. Nur additive Änderungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="60c2c-p106">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="60c2c-144">status</span><span class="sxs-lookup"><span data-stu-id="60c2c-144">status</span></span>|<span data-ttu-id="60c2c-145">String</span><span class="sxs-lookup"><span data-stu-id="60c2c-145">String</span></span>|<span data-ttu-id="60c2c-146">Der Lebenszyklusstatus der Schemaerweiterung.</span><span class="sxs-lookup"><span data-stu-id="60c2c-146">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="60c2c-147">Der Anfangszustand erstellt worden ist **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="60c2c-147">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="60c2c-148">Möglichen Zuständen Übergänge liegen **InDevelopment** bis **verfügbar** und **veraltet** **verfügbar** .</span><span class="sxs-lookup"><span data-stu-id="60c2c-148">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="60c2c-149">targetTypes</span><span class="sxs-lookup"><span data-stu-id="60c2c-149">targetTypes</span></span>|<span data-ttu-id="60c2c-150">String collection</span><span class="sxs-lookup"><span data-stu-id="60c2c-150">String collection</span></span>|<span data-ttu-id="60c2c-p108">Satz von Microsoft Graph-Typen (die Erweiterungen unterstützen können), auf die die Schemaerweiterung angewendet werden kann.  Nur additive Änderungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="60c2c-p108">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="60c2c-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="60c2c-153">Response</span></span>

<span data-ttu-id="60c2c-154">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60c2c-154">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="60c2c-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="60c2c-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="60c2c-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="60c2c-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <a name="response"></a><span data-ttu-id="60c2c-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="60c2c-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="60c2c-158">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="60c2c-158">See also</span></span>

- [<span data-ttu-id="60c2c-159">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="60c2c-159">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="60c2c-160">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="60c2c-160">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
