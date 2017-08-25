# <a name="delete-schemaextension"></a><span data-ttu-id="2bff1-101">schemaExtension löschen</span><span class="sxs-lookup"><span data-stu-id="2bff1-101">Delete schemaExtension</span></span>

<span data-ttu-id="2bff1-102">Dient zum Löschen eines [schemaExtension](../resources/schemaExtension.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2bff1-102">Delete the definition of a [schema extension](../resources/schemaExtension.md).</span></span>

<span data-ttu-id="2bff1-p101">Nur die App, mit der die Schemaerweiterung erstellt wurde (Besitzer-App), kann die Schemaerweiterungsdefinition löschen, und zwar nur, wenn die Erweiterung den Status **InDevelopment** aufweist. Das Löschen einer Schemaerweiterungsdefinition hat keinen Einfluss auf den Zugriff auf benutzerdefinierte Daten, die aufgrund dieser Definition zu Ressourceninstanzen hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="2bff1-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="2bff1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2bff1-105">Permissions</span></span>
<span data-ttu-id="2bff1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2bff1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="2bff1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2bff1-108">Permission type</span></span>      | <span data-ttu-id="2bff1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2bff1-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="2bff1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2bff1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2bff1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2bff1-111">Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="2bff1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2bff1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bff1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2bff1-113">Not supported.</span></span>    | 
|<span data-ttu-id="2bff1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2bff1-114">Application</span></span> | <span data-ttu-id="2bff1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2bff1-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2bff1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2bff1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2bff1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2bff1-117">Request headers</span></span>
| <span data-ttu-id="2bff1-118">Name</span><span class="sxs-lookup"><span data-stu-id="2bff1-118">Name</span></span>      |<span data-ttu-id="2bff1-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2bff1-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2bff1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bff1-120">Authorization</span></span>  | <span data-ttu-id="2bff1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2bff1-p103">Bearer {token}. Required.</span></span> |
 

## <a name="request-body"></a><span data-ttu-id="2bff1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2bff1-123">Request body</span></span>
<span data-ttu-id="2bff1-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2bff1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bff1-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="2bff1-125">Response</span></span>

<span data-ttu-id="2bff1-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2bff1-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bff1-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2bff1-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2bff1-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2bff1-129">Request</span></span>
<span data-ttu-id="2bff1-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2bff1-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="2bff1-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2bff1-131">Response</span></span>
<span data-ttu-id="2bff1-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2bff1-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="2bff1-133">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2bff1-133">See also</span></span>

- [<span data-ttu-id="2bff1-134">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="2bff1-134">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="2bff1-135">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="2bff1-135">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->