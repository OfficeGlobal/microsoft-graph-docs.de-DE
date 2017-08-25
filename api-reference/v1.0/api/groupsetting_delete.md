# <a name="delete-a-group-setting"></a><span data-ttu-id="481f8-101">Löschen einer Gruppeneinstellung</span><span class="sxs-lookup"><span data-stu-id="481f8-101">Delete a group setting</span></span>

<span data-ttu-id="481f8-102">Mit dieser API können Sie Gruppeneinstellungen löschen.</span><span class="sxs-lookup"><span data-stu-id="481f8-102">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="481f8-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="481f8-103">Permissions</span></span>

<span data-ttu-id="481f8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="481f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="481f8-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="481f8-106">Permission type</span></span>      | <span data-ttu-id="481f8-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="481f8-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="481f8-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="481f8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="481f8-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="481f8-109">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="481f8-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="481f8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="481f8-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="481f8-111">Not supported.</span></span>    | 
|<span data-ttu-id="481f8-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="481f8-112">Application</span></span> | <span data-ttu-id="481f8-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="481f8-113">Directory.ReadWrite.All</span></span> | 


## <a name="http-request"></a><span data-ttu-id="481f8-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="481f8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="481f8-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="481f8-115">Request headers</span></span>

| <span data-ttu-id="481f8-116">Name</span><span class="sxs-lookup"><span data-stu-id="481f8-116">Name</span></span> | <span data-ttu-id="481f8-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="481f8-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="481f8-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="481f8-118">Authorization</span></span>  | <span data-ttu-id="481f8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="481f8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="481f8-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="481f8-121">Content-Type</span></span>  | <span data-ttu-id="481f8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="481f8-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="481f8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="481f8-123">Request body</span></span>
<span data-ttu-id="481f8-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="481f8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="481f8-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="481f8-125">Response</span></span>

<span data-ttu-id="481f8-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="481f8-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="481f8-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="481f8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="481f8-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="481f8-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="481f8-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="481f8-130">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->