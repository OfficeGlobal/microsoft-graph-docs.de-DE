# <a name="update-outlook-category"></a><span data-ttu-id="c9ff9-101">Aktualisieren der Outlook-Kategorie</span><span class="sxs-lookup"><span data-stu-id="c9ff9-101">Update Outlook category</span></span>


<span data-ttu-id="c9ff9-102">Aktualisieren Sie die schreibbare Eigenschaft, **color**, des angegebenen [outlookCategory](../resources/outlookCategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9ff9-102">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookCategory.md) object.</span></span> <span data-ttu-id="c9ff9-103">Sie können die **displayName**-Eigenschaft nicht mehr ändern, nachdem die Kategorie erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="c9ff9-103">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9ff9-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c9ff9-104">Permissions</span></span>
<span data-ttu-id="c9ff9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c9ff9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c9ff9-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9ff9-107">Permission type</span></span>      | <span data-ttu-id="c9ff9-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9ff9-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9ff9-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9ff9-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c9ff9-110">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9ff9-110">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c9ff9-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9ff9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9ff9-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9ff9-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c9ff9-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9ff9-113">Application</span></span> | <span data-ttu-id="c9ff9-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9ff9-114">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9ff9-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9ff9-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c9ff9-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c9ff9-116">Optional query parameters</span></span>
<span data-ttu-id="c9ff9-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c9ff9-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9ff9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9ff9-118">Request headers</span></span>
| <span data-ttu-id="c9ff9-119">Name</span><span class="sxs-lookup"><span data-stu-id="c9ff9-119">Name</span></span>      |<span data-ttu-id="c9ff9-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9ff9-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c9ff9-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c9ff9-121">Authorization</span></span>  | <span data-ttu-id="c9ff9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c9ff9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9ff9-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9ff9-124">Request body</span></span>
<span data-ttu-id="c9ff9-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="c9ff9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c9ff9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9ff9-128">Property</span></span>     | <span data-ttu-id="c9ff9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c9ff9-129">Type</span></span>   |<span data-ttu-id="c9ff9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9ff9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9ff9-131">color</span><span class="sxs-lookup"><span data-stu-id="c9ff9-131">color</span></span>|<span data-ttu-id="c9ff9-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9ff9-132">String</span></span>|<span data-ttu-id="c9ff9-133">Eine voreingestellte Konstante, die eine Kategorie charakterisiert und einer von 25 vordefinierten Farben zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="c9ff9-133">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="c9ff9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9ff9-134">Response</span></span>

<span data-ttu-id="c9ff9-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [outlookCategory](../resources/outlookCategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9ff9-135">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookCategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9ff9-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9ff9-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9ff9-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9ff9-137">Request</span></span>
<span data-ttu-id="c9ff9-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9ff9-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["bac262b7-485d-4739-b436-e31467d64fac"],
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="c9ff9-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9ff9-139">Response</span></span>
<span data-ttu-id="c9ff9-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9ff9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->