# <a name="update-nameditem"></a><span data-ttu-id="f03ae-101">nameditem aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f03ae-101">Update nameditem</span></span>

<span data-ttu-id="f03ae-102">Dient zum Aktualisieren der Eigenschaften des nameditem-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f03ae-102">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f03ae-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f03ae-103">Permissions</span></span>
<span data-ttu-id="f03ae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f03ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f03ae-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f03ae-106">Permission type</span></span>      | <span data-ttu-id="f03ae-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f03ae-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f03ae-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f03ae-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f03ae-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f03ae-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f03ae-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f03ae-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f03ae-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f03ae-111">Not supported.</span></span>    |
|<span data-ttu-id="f03ae-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f03ae-112">Application</span></span> | <span data-ttu-id="f03ae-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f03ae-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f03ae-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f03ae-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="f03ae-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f03ae-115">Optional request headers</span></span>
| <span data-ttu-id="f03ae-116">Name</span><span class="sxs-lookup"><span data-stu-id="f03ae-116">Name</span></span>       | <span data-ttu-id="f03ae-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f03ae-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f03ae-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="f03ae-118">Authorization</span></span>  | <span data-ttu-id="f03ae-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f03ae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f03ae-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f03ae-121">Request body</span></span>
<span data-ttu-id="f03ae-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="f03ae-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f03ae-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f03ae-125">Property</span></span>     | <span data-ttu-id="f03ae-126">Typ</span><span class="sxs-lookup"><span data-stu-id="f03ae-126">Type</span></span>   |<span data-ttu-id="f03ae-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f03ae-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f03ae-128">visible</span><span class="sxs-lookup"><span data-stu-id="f03ae-128">visible</span></span>|<span data-ttu-id="f03ae-129">boolean</span><span class="sxs-lookup"><span data-stu-id="f03ae-129">boolean</span></span>|<span data-ttu-id="f03ae-130">Gibt an, ob das Objekt sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="f03ae-130">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="f03ae-131">comment</span><span class="sxs-lookup"><span data-stu-id="f03ae-131">comment</span></span>|   <span data-ttu-id="f03ae-132">string</span><span class="sxs-lookup"><span data-stu-id="f03ae-132">string</span></span>  |<span data-ttu-id="f03ae-133">Stellt den Kommentar dar, der mit diesem Namen verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="f03ae-133">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="f03ae-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f03ae-134">Response</span></span>

<span data-ttu-id="f03ae-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [NamedItem](../resources/nameditem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f03ae-135">If successful, this method returns a `200 OK` response code and updated [NamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f03ae-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f03ae-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f03ae-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f03ae-137">Request</span></span>
<span data-ttu-id="f03ae-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f03ae-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="f03ae-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="f03ae-139">Response</span></span>
<span data-ttu-id="f03ae-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f03ae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
