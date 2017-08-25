# <a name="delete-entity"></a><span data-ttu-id="ba8a6-101">Entität löschen</span><span class="sxs-lookup"><span data-stu-id="ba8a6-101">Delete entity</span></span>

<span data-ttu-id="ba8a6-102">Mit dieser API können Sie Entitäten löschen.</span><span class="sxs-lookup"><span data-stu-id="ba8a6-102">Delete entity.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba8a6-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ba8a6-103">Permissions</span></span>
<span data-ttu-id="ba8a6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba8a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ba8a6-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ba8a6-106">Permission type</span></span>      | <span data-ttu-id="ba8a6-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ba8a6-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="ba8a6-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ba8a6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ba8a6-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba8a6-109">Not supported.</span></span>    | 
|<span data-ttu-id="ba8a6-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ba8a6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba8a6-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba8a6-111">Not supported.</span></span>    | 
|<span data-ttu-id="ba8a6-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba8a6-112">Application</span></span> | <span data-ttu-id="ba8a6-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba8a6-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ba8a6-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba8a6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http


```
## <a name="request-headers"></a><span data-ttu-id="ba8a6-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ba8a6-115">Request headers</span></span>
| <span data-ttu-id="ba8a6-116">Name</span><span class="sxs-lookup"><span data-stu-id="ba8a6-116">Name</span></span>       | <span data-ttu-id="ba8a6-117">Typ</span><span class="sxs-lookup"><span data-stu-id="ba8a6-117">Type</span></span> | <span data-ttu-id="ba8a6-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba8a6-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba8a6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba8a6-119">Authorization</span></span>  | <span data-ttu-id="ba8a6-120">string</span><span class="sxs-lookup"><span data-stu-id="ba8a6-120">string</span></span>  | <span data-ttu-id="ba8a6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ba8a6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba8a6-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ba8a6-123">Request body</span></span>
<span data-ttu-id="ba8a6-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ba8a6-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba8a6-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba8a6-125">Response</span></span>

<span data-ttu-id="ba8a6-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ba8a6-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba8a6-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ba8a6-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba8a6-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba8a6-129">Request</span></span>
<span data-ttu-id="ba8a6-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ba8a6-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "delete_entity"
}-->
```http

```
##### <a name="response"></a><span data-ttu-id="ba8a6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba8a6-131">Response</span></span>
<span data-ttu-id="ba8a6-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ba8a6-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete entity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
