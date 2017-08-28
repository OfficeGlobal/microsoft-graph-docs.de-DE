# <a name="create-schemaextension"></a><span data-ttu-id="584b6-101">schemaExtension erstellen</span><span class="sxs-lookup"><span data-stu-id="584b6-101">Create schemaExtension</span></span>

<span data-ttu-id="584b6-102">Erstellen Sie eine neue [schemaExtension](../resources/schemaextension.md)-Definition, um einen [unterstützenden Ressourcentyp](../../../concepts/extensibility_overview.md#supported-resources) zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="584b6-102">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](../../../concepts/extensibility_overview.md#supported-resources).</span></span>

<span data-ttu-id="584b6-p101">Mit Schemaerweiterungen können Sie stark typisierte benutzerdefinierte Daten zu einer Ressource hinzufügen. Die App, die eine Schemaerweiterung erstellt, ist die Besitzer-App. Abhängig vom [Status](../../../concepts/extensibility_overview.md#schema-extensions-lifecycle) der Erweiterung kann die Besitzer-App, und nur die Besitzer-App, die Erweiterung aktualisieren oder löschen.</span><span class="sxs-lookup"><span data-stu-id="584b6-p101">Schema extensions let you add strongly-typed custom data to a resource. The app that creates a schema extension is the owner app. Depending on the [state](../../../concepts/extensibility_overview.md#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="584b6-106">Erfahren Sie anhand von Beispielen, wie Sie [eine Schemaerweiterung definieren, die einen Schulungskurs beschreibt](../../../concepts/extensibility_schema_groups.md#2-register-a-schema-extension-definition-that-describes-a-training-course), die Schemaerweiterungsdefinition zum [Erstellen einer neuen Gruppe mit Schulungskursdaten](../../../concepts/extensibility_schema_groups.md#3-create-a-new-group-with-extended-data) verwenden und [Schulungskursdaten zu einer vorhandenen Gruppe hinzufügen](../../../concepts/extensibility_schema_groups.md#4-add-update-or-remove-custom-data-in-an-existing-group).</span><span class="sxs-lookup"><span data-stu-id="584b6-106">See examples of how to [define a schema extension that describes a training course](../../../concepts/extensibility_schema_groups.md#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](../../../concepts/extensibility_schema_groups.md#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](../../../concepts/extensibility_schema_groups.md#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="584b6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="584b6-107">Permissions</span></span>
<span data-ttu-id="584b6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="584b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="584b6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="584b6-110">Permission type</span></span>      | <span data-ttu-id="584b6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="584b6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="584b6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="584b6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="584b6-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="584b6-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="584b6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="584b6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="584b6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="584b6-115">Not supported.</span></span>    |
|<span data-ttu-id="584b6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="584b6-116">Application</span></span> | <span data-ttu-id="584b6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="584b6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="584b6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="584b6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="584b6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="584b6-119">Request headers</span></span>
| <span data-ttu-id="584b6-120">Name</span><span class="sxs-lookup"><span data-stu-id="584b6-120">Name</span></span>       | <span data-ttu-id="584b6-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="584b6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="584b6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="584b6-122">Authorization</span></span>  | <span data-ttu-id="584b6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="584b6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="584b6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="584b6-125">Content-Type</span></span>  | <span data-ttu-id="584b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="584b6-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="584b6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="584b6-127">Request body</span></span>
<span data-ttu-id="584b6-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines [schemaExtension](../resources/schemaextension.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="584b6-128">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="584b6-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen einer Schemaerweiterung erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="584b6-129">The following table shows the properties that are required when you create a schema extension.</span></span>

| <span data-ttu-id="584b6-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="584b6-130">Parameter</span></span> | <span data-ttu-id="584b6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="584b6-131">Type</span></span> | <span data-ttu-id="584b6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="584b6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="584b6-133">description</span><span class="sxs-lookup"><span data-stu-id="584b6-133">description</span></span>|<span data-ttu-id="584b6-134">String</span><span class="sxs-lookup"><span data-stu-id="584b6-134">String</span></span>|<span data-ttu-id="584b6-135">Beschreibung für die Schemaerweiterung.</span><span class="sxs-lookup"><span data-stu-id="584b6-135">Description for the schema extension.</span></span>|
|<span data-ttu-id="584b6-136">id</span><span class="sxs-lookup"><span data-stu-id="584b6-136">id</span></span>|<span data-ttu-id="584b6-137">String</span><span class="sxs-lookup"><span data-stu-id="584b6-137">String</span></span>|<span data-ttu-id="584b6-138">Der eindeutige Bezeichner für die Schemaerweiterungsdefinition.</span><span class="sxs-lookup"><span data-stu-id="584b6-138">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="584b6-139">Sie können einen Wert mit einer von zwei Methoden zuweisen:</span><span class="sxs-lookup"><span data-stu-id="584b6-139">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="584b6-p104">Verketten Sie den Namen einer Ihrer überprüften Domänen mit einem Namen für die Schemaerweiterung, um eine eindeutige Zeichenfolge in diesem Format zu bilden: \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Beispiel: `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="584b6-p104">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="584b6-p105">Geben Sie einen Schemanamen an, und verwenden Sie diesen Schemanamen in Microsoft Graph zum Vervollständigen der **id**-Zuweisung in diesem Format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Zum Beispiel: `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="584b6-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="584b6-144">Diese Eigenschaft kann nach dem Erstellen nicht mehr geändert werden.</span><span class="sxs-lookup"><span data-stu-id="584b6-144">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="584b6-145">properties</span><span class="sxs-lookup"><span data-stu-id="584b6-145">properties</span></span>|<span data-ttu-id="584b6-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="584b6-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="584b6-147">Die Sammlung von Eigenschaftennamen und Typen, die die Schemaerweiterungsdefinition bilden.</span><span class="sxs-lookup"><span data-stu-id="584b6-147">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="584b6-148">targetTypes</span><span class="sxs-lookup"><span data-stu-id="584b6-148">targetTypes</span></span>|<span data-ttu-id="584b6-149">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="584b6-149">String collection</span></span>|<span data-ttu-id="584b6-150">Ein Satz von Microsoft Graph-Ressourcentypen (die Erweiterungen unterstützen), auf die diese Schemaerweiterungsdefinition angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="584b6-150">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="584b6-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="584b6-151">Response</span></span>

<span data-ttu-id="584b6-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [schemaExtension](../resources/schemaextension.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="584b6-152">If successful, this method returns `201, Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="584b6-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="584b6-153">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="584b6-154">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="584b6-154">Request 1</span></span>

<span data-ttu-id="584b6-p106">Im ersten Beispiel wird veranschaulicht, wie aus einem überprüften Domänennamen, `graphlearn`, und einem Schemanamen, `courses`, eine eindeutige Zeichenfolge für die **id**-Eigenschaft der Schemaerweiterungsdefinition gebildet wird. Die eindeutige Zeichenfolge basiert auf diesem Format: \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span><span class="sxs-lookup"><span data-stu-id="584b6-p106">The first example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition. The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

<span data-ttu-id="584b6-157">Geben Sie im Anforderungstext eine JSON-Darstellung des [schemaExtension](../resources/schemaextension.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="584b6-157">In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json

{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="response-1"></a><span data-ttu-id="584b6-158">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="584b6-158">Response 1</span></span>

<span data-ttu-id="584b6-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="584b6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="584b6-162">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="584b6-162">Request 2</span></span>

<span data-ttu-id="584b6-p108">Im zweiten Beispiel wird lediglich ein Schemaname, `courses`, in der **id**-Eigenschaft in der Anforderung angegeben, zusammen mit der JSON-Darstellung der restlichen Eigenschaften im [schemaExtension](../resources/schemaextension.md)-Objekt. Microsoft Graph weist einen eindeutigen Zeichenfolgenwert zu und gibt ihn in der Antwort zurück.</span><span class="sxs-lookup"><span data-stu-id="584b6-p108">The second example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object. Microsoft Graph will assign and return a unique string value in the response.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json

{
    "id":"courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="584b6-165">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="584b6-165">Response 2</span></span>

<span data-ttu-id="584b6-p109">Die Antwort enthält eine eindeutige Zeichenfolge in der **id**-Eigenschaft, die auf dem in der Anforderung angegebenen Schemanamen zusammen mit dem Rest der neu erstellten Schemadefinition basiert. Der Wert der **id**-Eigenschaft der Antwort basiert auf diesem Format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="584b6-p109">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition. The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "extk9eruy7c_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="584b6-170">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="584b6-170">See also</span></span>

- [<span data-ttu-id="584b6-171">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="584b6-171">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="584b6-172">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="584b6-172">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->