# <a name="delete-conversation"></a><span data-ttu-id="bb64e-101">Unterhaltung löschen</span><span class="sxs-lookup"><span data-stu-id="bb64e-101">Delete conversation</span></span>
<span data-ttu-id="bb64e-102">Löschen eines [conversation](../resources/conversation.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb64e-102">Delete conversation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb64e-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bb64e-103">Permissions</span></span>
<span data-ttu-id="bb64e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb64e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bb64e-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bb64e-106">Permission type</span></span>      | <span data-ttu-id="bb64e-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bb64e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb64e-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bb64e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bb64e-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb64e-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb64e-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bb64e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb64e-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb64e-111">Not supported.</span></span>    |
|<span data-ttu-id="bb64e-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb64e-112">Application</span></span> | <span data-ttu-id="bb64e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb64e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb64e-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb64e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bb64e-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bb64e-115">Request headers</span></span>
| <span data-ttu-id="bb64e-116">Name</span><span class="sxs-lookup"><span data-stu-id="bb64e-116">Name</span></span>       | <span data-ttu-id="bb64e-117">Typ</span><span class="sxs-lookup"><span data-stu-id="bb64e-117">Type</span></span> | <span data-ttu-id="bb64e-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb64e-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bb64e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb64e-119">Authorization</span></span>  | <span data-ttu-id="bb64e-120">string</span><span class="sxs-lookup"><span data-stu-id="bb64e-120">string</span></span>  | <span data-ttu-id="bb64e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bb64e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb64e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bb64e-123">Request body</span></span>
<span data-ttu-id="bb64e-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bb64e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb64e-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb64e-125">Response</span></span>
<span data-ttu-id="bb64e-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb64e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb64e-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bb64e-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bb64e-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb64e-129">Request</span></span>
<span data-ttu-id="bb64e-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bb64e-130">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="bb64e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb64e-131">Response</span></span>
<span data-ttu-id="bb64e-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bb64e-132">Here is an example of the response.</span></span> 
><span data-ttu-id="bb64e-133">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="bb64e-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bb64e-134">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="bb64e-134">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->