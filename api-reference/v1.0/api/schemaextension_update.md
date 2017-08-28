# <a name="update-schemaextension"></a><span data-ttu-id="63f3f-101">schemaExtension aktualisieren</span><span class="sxs-lookup"><span data-stu-id="63f3f-101">Update schemaExtension</span></span>

<span data-ttu-id="63f3f-102">Dient zum Aktualisieren der Eigenschaften in der Definition der angegebenen [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="63f3f-102">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="63f3f-p101">Die Aktualisierung gilt für alle Ressourcen, die in der Eigenschaft **targetTypes** der Erweiterung enthalten sind. Diese Ressourcen gehören zu den [unterstützenden Ressourcentypen](../../../concepts/extensibility_overview.md#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="63f3f-p101">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](../../../concepts/extensibility_overview.md#supported-resources).</span></span>

<span data-ttu-id="63f3f-p102">Nur die App, mit der eine Schemaerweiterung erstellt wurde (Besitzer-App), kann additive Aktualisierungen an der Erweiterung vornehmen, wenn die Erweiterung den Status **InDevelopment** oder **Available** aufweist. Dies bedeutet, dass die App keine benutzerdefinierten Eigenschaften oder Zielressourcentypen aus der Definition entfernen kann. Die App kann jedoch die Beschreibung der Erweiterung ändern.</span><span class="sxs-lookup"><span data-stu-id="63f3f-p102">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="63f3f-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="63f3f-108">Permissions</span></span>
<span data-ttu-id="63f3f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="63f3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="63f3f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="63f3f-111">Permission type</span></span>      | <span data-ttu-id="63f3f-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="63f3f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63f3f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="63f3f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="63f3f-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="63f3f-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="63f3f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="63f3f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63f3f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63f3f-116">Not supported.</span></span>    |
|<span data-ttu-id="63f3f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="63f3f-117">Application</span></span> | <span data-ttu-id="63f3f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63f3f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63f3f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="63f3f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="63f3f-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="63f3f-120">Optional request headers</span></span>

| <span data-ttu-id="63f3f-121">Name</span><span class="sxs-lookup"><span data-stu-id="63f3f-121">Name</span></span>      |<span data-ttu-id="63f3f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63f3f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="63f3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63f3f-123">Authorization</span></span>  | <span data-ttu-id="63f3f-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="63f3f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63f3f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63f3f-126">Content-Type</span></span>   | <span data-ttu-id="63f3f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="63f3f-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="63f3f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="63f3f-128">Request body</span></span>

<span data-ttu-id="63f3f-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="63f3f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="63f3f-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="63f3f-132">Property</span></span>   | <span data-ttu-id="63f3f-133">Typ</span><span class="sxs-lookup"><span data-stu-id="63f3f-133">Type</span></span> |<span data-ttu-id="63f3f-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63f3f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63f3f-135">description</span><span class="sxs-lookup"><span data-stu-id="63f3f-135">description</span></span>|<span data-ttu-id="63f3f-136">String</span><span class="sxs-lookup"><span data-stu-id="63f3f-136">String</span></span>|<span data-ttu-id="63f3f-137">Beschreibung für die Schemaerweiterung.</span><span class="sxs-lookup"><span data-stu-id="63f3f-137">Description for the schema extension.</span></span>|
|<span data-ttu-id="63f3f-138">properties</span><span class="sxs-lookup"><span data-stu-id="63f3f-138">properties</span></span>|<span data-ttu-id="63f3f-139">[extensionSchemaProperty](../resources/extensionschemaproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="63f3f-139">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="63f3f-p106">Die Sammlung von Eigenschaftennamen und Typen, die die Schemaerweiterungsdefinition bilden. Nur additive Änderungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="63f3f-p106">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="63f3f-142">status</span><span class="sxs-lookup"><span data-stu-id="63f3f-142">status</span></span>|<span data-ttu-id="63f3f-143">String</span><span class="sxs-lookup"><span data-stu-id="63f3f-143">String</span></span>|<span data-ttu-id="63f3f-p107">Der Lebenszyklusstatus der Schemaerweiterung. Bei der Erstellung ist der anfängliche Status **InDevelopment**. Mögliche Statusübergänge sind von **InDevelopment** zu **Available**, von **Available** zu **Deprecated** und von **Deprecated** zu **Available**.</span><span class="sxs-lookup"><span data-stu-id="63f3f-p107">The lifecycle state of the schema extension. The initial state upon creation is **InDevelopment**. Possible states transitions are from **InDevelopment** to **Available**, **Available** to **Deprecated** and **Deprecated** to **Available**.</span></span>|
|<span data-ttu-id="63f3f-147">targetTypes</span><span class="sxs-lookup"><span data-stu-id="63f3f-147">targetTypes</span></span>|<span data-ttu-id="63f3f-148">String collection</span><span class="sxs-lookup"><span data-stu-id="63f3f-148">String collection</span></span>|<span data-ttu-id="63f3f-p108">Satz von Microsoft Graph-Typen (die Erweiterungen unterstützen können), auf die die Schemaerweiterung angewendet werden kann.  Nur additive Änderungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="63f3f-p108">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="63f3f-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="63f3f-151">Response</span></span>

<span data-ttu-id="63f3f-152">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63f3f-152">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="63f3f-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="63f3f-153">Example</span></span>

##### <a name="request"></a><span data-ttu-id="63f3f-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63f3f-154">Request</span></span>

<span data-ttu-id="63f3f-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="63f3f-155">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="63f3f-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="63f3f-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="63f3f-157">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="63f3f-157">See also</span></span>

- [<span data-ttu-id="63f3f-158">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="63f3f-158">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="63f3f-159">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="63f3f-159">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->