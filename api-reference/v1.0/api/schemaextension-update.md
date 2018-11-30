---
title: schemaExtension aktualisieren
description: Dient zum Aktualisieren der Eigenschaften in der Definition der angegebenen schemaExtension.
ms.openlocfilehash: a09b3a4e2e48eb550acd5e77c60ab7213cc52de8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018226"
---
# <a name="update-schemaextension"></a><span data-ttu-id="354f2-103">schemaExtension aktualisieren</span><span class="sxs-lookup"><span data-stu-id="354f2-103">Update schemaExtension</span></span>

<span data-ttu-id="354f2-104">Dient zum Aktualisieren der Eigenschaften in der Definition der angegebenen [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="354f2-104">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="354f2-p101">Die Aktualisierung gilt für alle Ressourcen, die in der Eigenschaft **targetTypes** der Erweiterung enthalten sind. Diese Ressourcen gehören zu den [unterstützenden Ressourcentypen](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="354f2-p101">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="354f2-p102">Nur die App, mit der eine Schemaerweiterung erstellt wurde (Besitzer-App), kann additive Aktualisierungen an der Erweiterung vornehmen, wenn die Erweiterung den Status **InDevelopment** oder **Available** aufweist. Dies bedeutet, dass die App keine benutzerdefinierten Eigenschaften oder Zielressourcentypen aus der Definition entfernen kann. Die App kann jedoch die Beschreibung der Erweiterung ändern.</span><span class="sxs-lookup"><span data-stu-id="354f2-p102">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="354f2-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="354f2-110">Permissions</span></span>
<span data-ttu-id="354f2-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="354f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="354f2-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="354f2-113">Permission type</span></span>      | <span data-ttu-id="354f2-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="354f2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="354f2-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="354f2-115">Delegated (work or school account)</span></span> | <span data-ttu-id="354f2-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="354f2-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="354f2-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="354f2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="354f2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="354f2-118">Not supported.</span></span>    |
|<span data-ttu-id="354f2-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="354f2-119">Application</span></span> | <span data-ttu-id="354f2-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="354f2-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="354f2-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="354f2-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="354f2-122">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="354f2-122">Optional request headers</span></span>

| <span data-ttu-id="354f2-123">Name</span><span class="sxs-lookup"><span data-stu-id="354f2-123">Name</span></span>      |<span data-ttu-id="354f2-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="354f2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="354f2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="354f2-125">Authorization</span></span>  | <span data-ttu-id="354f2-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="354f2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="354f2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="354f2-128">Content-Type</span></span>   | <span data-ttu-id="354f2-129">application/json</span><span class="sxs-lookup"><span data-stu-id="354f2-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="354f2-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="354f2-130">Request body</span></span>

<span data-ttu-id="354f2-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="354f2-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="354f2-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="354f2-134">Property</span></span>   | <span data-ttu-id="354f2-135">Typ</span><span class="sxs-lookup"><span data-stu-id="354f2-135">Type</span></span> |<span data-ttu-id="354f2-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="354f2-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="354f2-137">description</span><span class="sxs-lookup"><span data-stu-id="354f2-137">description</span></span>|<span data-ttu-id="354f2-138">String</span><span class="sxs-lookup"><span data-stu-id="354f2-138">String</span></span>|<span data-ttu-id="354f2-139">Beschreibung für die Schemaerweiterung.</span><span class="sxs-lookup"><span data-stu-id="354f2-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="354f2-140">properties</span><span class="sxs-lookup"><span data-stu-id="354f2-140">properties</span></span>|<span data-ttu-id="354f2-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="354f2-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="354f2-p106">Die Sammlung von Eigenschaftennamen und Typen, die die Schemaerweiterungsdefinition bilden. Nur additive Änderungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="354f2-p106">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="354f2-144">status</span><span class="sxs-lookup"><span data-stu-id="354f2-144">status</span></span>|<span data-ttu-id="354f2-145">String</span><span class="sxs-lookup"><span data-stu-id="354f2-145">String</span></span>|<span data-ttu-id="354f2-146">Der Lebenszyklusstatus der Schemaerweiterung.</span><span class="sxs-lookup"><span data-stu-id="354f2-146">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="354f2-147">Der Anfangszustand erstellt worden ist **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="354f2-147">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="354f2-148">Möglichen Zuständen Übergänge liegen **InDevelopment** bis **verfügbar** und **veraltet** **verfügbar** .</span><span class="sxs-lookup"><span data-stu-id="354f2-148">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="354f2-149">targetTypes</span><span class="sxs-lookup"><span data-stu-id="354f2-149">targetTypes</span></span>|<span data-ttu-id="354f2-150">String collection</span><span class="sxs-lookup"><span data-stu-id="354f2-150">String collection</span></span>|<span data-ttu-id="354f2-p108">Satz von Microsoft Graph-Typen (die Erweiterungen unterstützen können), auf die die Schemaerweiterung angewendet werden kann.  Nur additive Änderungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="354f2-p108">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="354f2-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="354f2-153">Response</span></span>

<span data-ttu-id="354f2-154">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="354f2-154">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="354f2-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="354f2-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="354f2-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="354f2-156">Request</span></span>

<span data-ttu-id="354f2-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="354f2-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
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

##### <a name="response"></a><span data-ttu-id="354f2-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="354f2-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="354f2-159">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="354f2-159">See also</span></span>

- [<span data-ttu-id="354f2-160">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="354f2-160">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="354f2-161">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="354f2-161">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->