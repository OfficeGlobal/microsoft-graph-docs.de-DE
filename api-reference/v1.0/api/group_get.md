# <a name="get-group"></a><span data-ttu-id="a8438-101">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="a8438-101">Get group</span></span>
<span data-ttu-id="a8438-102">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Gruppenobjekts.</span><span class="sxs-lookup"><span data-stu-id="a8438-102">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="a8438-103">Standardeigenschaften</span><span class="sxs-lookup"><span data-stu-id="a8438-103">Default properties</span></span>

<span data-ttu-id="a8438-p101">Im Folgenden werden standardmäßige Eigenschaften dargestellt, die beim Abrufen oder beim Auflisten von Gruppen zurückgegeben werden. Diese stellen eine Teilmenge aller verfügbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="a8438-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span> 

* <span data-ttu-id="a8438-106">description</span><span class="sxs-lookup"><span data-stu-id="a8438-106">description</span></span>
* <span data-ttu-id="a8438-107">displayName</span><span class="sxs-lookup"><span data-stu-id="a8438-107">displayName</span></span>
* <span data-ttu-id="a8438-108">groupTypes</span><span class="sxs-lookup"><span data-stu-id="a8438-108">groupTypes</span></span>
* <span data-ttu-id="a8438-109">id</span><span class="sxs-lookup"><span data-stu-id="a8438-109">id</span></span>
* <span data-ttu-id="a8438-110">Mail</span><span class="sxs-lookup"><span data-stu-id="a8438-110">mail</span></span>
* <span data-ttu-id="a8438-111">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="a8438-111">mailEnabled</span></span>
* <span data-ttu-id="a8438-112">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a8438-112">mailNickname</span></span>
* <span data-ttu-id="a8438-113">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a8438-113">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="a8438-114">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="a8438-114">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="a8438-115">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="a8438-115">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="a8438-116">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="a8438-116">proxyAddresses</span></span>
* <span data-ttu-id="a8438-117">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="a8438-117">securityEnabled</span></span>
* <span data-ttu-id="a8438-118">visibility</span><span class="sxs-lookup"><span data-stu-id="a8438-118">visibility</span></span>

<span data-ttu-id="a8438-119">Die folgenden Gruppeneigenschaften werden standardmäßig nicht zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="a8438-119">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="a8438-120">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="a8438-120">allowExternalSenders</span></span>
* <span data-ttu-id="a8438-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="a8438-121">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="a8438-122">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="a8438-122">isSubscribedByMail</span></span>
* <span data-ttu-id="a8438-123">unseenCount</span><span class="sxs-lookup"><span data-stu-id="a8438-123">unseenCount</span></span>

<span data-ttu-id="a8438-p102">Verwenden Sie zum Abrufen dieser Eigenschaften den **$select**-Abfrageparameter. Es folgen Beispiele:</span><span class="sxs-lookup"><span data-stu-id="a8438-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="a8438-126">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a8438-126">Permissions</span></span>
<span data-ttu-id="a8438-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8438-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a8438-129">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8438-129">Permission type</span></span>      | <span data-ttu-id="a8438-130">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8438-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8438-131">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8438-131">Delegated (work or school account)</span></span> | <span data-ttu-id="a8438-132">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8438-132">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a8438-133">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8438-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8438-134">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8438-134">Not supported.</span></span>    |
|<span data-ttu-id="a8438-135">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8438-135">Application</span></span> | <span data-ttu-id="a8438-136">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8438-136">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8438-137">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8438-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8438-138">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a8438-138">Optional query parameters</span></span>
<span data-ttu-id="a8438-139">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a8438-139">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8438-140">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8438-140">Request headers</span></span>
| <span data-ttu-id="a8438-141">Name</span><span class="sxs-lookup"><span data-stu-id="a8438-141">Name</span></span>       | <span data-ttu-id="a8438-142">Typ</span><span class="sxs-lookup"><span data-stu-id="a8438-142">Type</span></span> | <span data-ttu-id="a8438-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8438-143">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a8438-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8438-144">Authorization</span></span>  | <span data-ttu-id="a8438-145">string</span><span class="sxs-lookup"><span data-stu-id="a8438-145">string</span></span>  | <span data-ttu-id="a8438-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8438-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8438-148">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8438-148">Request body</span></span>
<span data-ttu-id="a8438-149">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a8438-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8438-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8438-150">Response</span></span>
<span data-ttu-id="a8438-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [photo](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8438-151">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8438-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8438-152">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a8438-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8438-153">Request</span></span>
<span data-ttu-id="a8438-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8438-154">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="a8438-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8438-155">Response</span></span>
<span data-ttu-id="a8438-156">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a8438-156">Here is an example of the response.</span></span>

><span data-ttu-id="a8438-157">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="a8438-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a8438-158">Von einem tatsächlichen Aufruf werden, wie zuvor beschrieben, die Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8438-158">Note: The response object shown here may be truncated for brevity. The default properties will be returned from an actual call, as described above.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
