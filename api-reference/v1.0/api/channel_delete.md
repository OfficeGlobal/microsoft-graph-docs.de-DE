# <a name="delete-channel"></a><span data-ttu-id="b537e-101">DDE-Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="b537e-101">Delete channel</span></span>



<span data-ttu-id="b537e-102">Löschen Sie den [Kanal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="b537e-102">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="b537e-103">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="b537e-103">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="b537e-104">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](../../../concepts/known_issues.md#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="b537e-104">For details, see the [known issues list](../../../concepts/known_issues.md#application-permissions).</span></span>

> <span data-ttu-id="b537e-105">**Hinweis**: die Daten in der gelöschten Kanäle weiterhin Wochen Teambesitzer Wiederherstellung gelöschter Kanal zulassen gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="b537e-105">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="b537e-106">Während dieser Zeit kann ein neuer Kanal mit der gleichen DisplayName nicht erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="b537e-106">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="b537e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b537e-107">Permissions</span></span>
<span data-ttu-id="b537e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b537e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b537e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b537e-110">Permission type</span></span>      | <span data-ttu-id="b537e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b537e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b537e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b537e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b537e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b537e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b537e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b537e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b537e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b537e-115">Not supported.</span></span>    |
|<span data-ttu-id="b537e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b537e-116">Application</span></span> | <span data-ttu-id="b537e-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b537e-117">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="b537e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b537e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b537e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b537e-119">Request headers</span></span>
| <span data-ttu-id="b537e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b537e-120">Header</span></span>       | <span data-ttu-id="b537e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b537e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b537e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b537e-122">Authorization</span></span>  | <span data-ttu-id="b537e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b537e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b537e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b537e-125">Request body</span></span>
<span data-ttu-id="b537e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b537e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b537e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b537e-127">Response</span></span>

<span data-ttu-id="b537e-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b537e-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b537e-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b537e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b537e-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b537e-131">Request</span></span>
<span data-ttu-id="b537e-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b537e-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="b537e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b537e-133">Response</span></span>

<span data-ttu-id="b537e-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b537e-134">The following is an example of the response.</span></span> 
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
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
