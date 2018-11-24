# <a name="delete-tab-from-channel"></a><span data-ttu-id="93252-101">Registerkarte von Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="93252-101">Delete tab from channel</span></span>



<span data-ttu-id="93252-102">Entfernt (löst) einer Registerkarte aus den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="93252-102">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="93252-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="93252-103">Permissions</span></span>
<span data-ttu-id="93252-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="93252-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="93252-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="93252-106">Permission type</span></span>      | <span data-ttu-id="93252-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="93252-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93252-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="93252-108">Delegated (work or school account)</span></span> | <span data-ttu-id="93252-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93252-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="93252-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="93252-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93252-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93252-111">Not supported.</span></span>    |
|<span data-ttu-id="93252-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="93252-112">Application</span></span> | <span data-ttu-id="93252-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93252-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93252-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93252-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="93252-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93252-115">Request headers</span></span>
| <span data-ttu-id="93252-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="93252-116">Header</span></span>       | <span data-ttu-id="93252-117">Wert</span><span class="sxs-lookup"><span data-stu-id="93252-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93252-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="93252-118">Authorization</span></span>  | <span data-ttu-id="93252-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="93252-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93252-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93252-121">Request body</span></span>
<span data-ttu-id="93252-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="93252-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93252-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="93252-123">Response</span></span>

<span data-ttu-id="93252-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93252-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93252-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93252-126">Example</span></span>
#### <a name="request"></a><span data-ttu-id="93252-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93252-127">Request</span></span>
<span data-ttu-id="93252-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93252-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="93252-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="93252-129">Response</span></span>
<span data-ttu-id="93252-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="93252-130">The following is an example of the response.</span></span> <span data-ttu-id="93252-131">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="93252-131">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="93252-132">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93252-132">All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
