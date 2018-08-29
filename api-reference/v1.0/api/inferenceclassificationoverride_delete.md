# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="15b22-101">inferenceClassificationOverride löschen</span><span class="sxs-lookup"><span data-stu-id="15b22-101">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="15b22-102">Mit dieser API können Sie eine Außerkraftsetzung anhand ihrer ID löschen.</span><span class="sxs-lookup"><span data-stu-id="15b22-102">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="15b22-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="15b22-103">Permissions</span></span>
<span data-ttu-id="15b22-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="15b22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="15b22-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15b22-106">Permission type</span></span>      | <span data-ttu-id="15b22-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15b22-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15b22-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15b22-108">Delegated (work or school account)</span></span> | <span data-ttu-id="15b22-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15b22-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="15b22-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15b22-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15b22-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15b22-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="15b22-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15b22-112">Application</span></span> | <span data-ttu-id="15b22-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15b22-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="15b22-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15b22-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="15b22-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15b22-115">Request headers</span></span>
| <span data-ttu-id="15b22-116">Name</span><span class="sxs-lookup"><span data-stu-id="15b22-116">Name</span></span>       | <span data-ttu-id="15b22-117">Typ</span><span class="sxs-lookup"><span data-stu-id="15b22-117">Type</span></span> | <span data-ttu-id="15b22-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15b22-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15b22-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="15b22-119">Authorization</span></span>  | <span data-ttu-id="15b22-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15b22-120">string</span></span>  | <span data-ttu-id="15b22-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15b22-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15b22-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15b22-123">Request body</span></span>
<span data-ttu-id="15b22-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="15b22-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15b22-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="15b22-125">Response</span></span>

<span data-ttu-id="15b22-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15b22-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15b22-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15b22-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15b22-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15b22-129">Request</span></span>
<span data-ttu-id="15b22-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15b22-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="15b22-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="15b22-131">Response</span></span>
<span data-ttu-id="15b22-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15b22-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->