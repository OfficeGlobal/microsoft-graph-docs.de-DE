# <a name="update-photo"></a><span data-ttu-id="2f594-101">Foto aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2f594-101">Update photo</span></span>

<span data-ttu-id="2f594-102">Mit dieser API können Sie die Eigenschaften von Fotoobjekten aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="2f594-102">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f594-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2f594-103">Permissions</span></span>
<span data-ttu-id="2f594-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f594-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2f594-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f594-106">Permission type</span></span>      | <span data-ttu-id="2f594-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f594-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f594-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f594-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2f594-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f594-109">Not supported.</span></span>    |
|<span data-ttu-id="2f594-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f594-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f594-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f594-111">Not supported.</span></span>    |
|<span data-ttu-id="2f594-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f594-112">Application</span></span> | <span data-ttu-id="2f594-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f594-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f594-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f594-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="2f594-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f594-115">Request headers</span></span>
| <span data-ttu-id="2f594-116">Name</span><span class="sxs-lookup"><span data-stu-id="2f594-116">Name</span></span>       | <span data-ttu-id="2f594-117">Typ</span><span class="sxs-lookup"><span data-stu-id="2f594-117">Type</span></span> | <span data-ttu-id="2f594-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f594-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2f594-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f594-119">Authorization</span></span>  | <span data-ttu-id="2f594-120">string</span><span class="sxs-lookup"><span data-stu-id="2f594-120">string</span></span>  | <span data-ttu-id="2f594-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f594-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f594-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f594-123">Request body</span></span>
<span data-ttu-id="2f594-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="2f594-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2f594-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f594-127">Property</span></span>     | <span data-ttu-id="2f594-128">Typ</span><span class="sxs-lookup"><span data-stu-id="2f594-128">Type</span></span>   |<span data-ttu-id="2f594-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f594-129">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="2f594-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f594-130">Response</span></span>

<span data-ttu-id="2f594-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte  [photo](../resources/photo.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f594-131">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2f594-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f594-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f594-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f594-133">Request</span></span>
<span data-ttu-id="2f594-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f594-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="2f594-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f594-135">Response</span></span>
<span data-ttu-id="2f594-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f594-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
