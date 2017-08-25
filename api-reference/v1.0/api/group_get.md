# <a name="get-group"></a><span data-ttu-id="4ab6a-101">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="4ab6a-101">Get group</span></span>

<span data-ttu-id="4ab6a-102">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Gruppenobjekts.</span><span class="sxs-lookup"><span data-stu-id="4ab6a-102">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="4ab6a-103">Standardeigenschaften</span><span class="sxs-lookup"><span data-stu-id="4ab6a-103">Default properties</span></span>

<span data-ttu-id="4ab6a-p101">Im Folgenden werden standardmäßige Eigenschaften dargestellt, die beim Abrufen oder beim Auflisten von Gruppen zurückgegeben werden. Diese stellen eine Teilmenge aller verfügbaren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="4ab6a-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span> 

* <span data-ttu-id="4ab6a-106">description</span><span class="sxs-lookup"><span data-stu-id="4ab6a-106">description</span></span>
* <span data-ttu-id="4ab6a-107">displayName</span><span class="sxs-lookup"><span data-stu-id="4ab6a-107">displayName</span></span>
* <span data-ttu-id="4ab6a-108">groupTypes</span><span class="sxs-lookup"><span data-stu-id="4ab6a-108">groupTypes</span></span>
* <span data-ttu-id="4ab6a-109">id</span><span class="sxs-lookup"><span data-stu-id="4ab6a-109">id</span></span>
* <span data-ttu-id="4ab6a-110">Mail</span><span class="sxs-lookup"><span data-stu-id="4ab6a-110">mail</span></span>
* <span data-ttu-id="4ab6a-111">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="4ab6a-111">mailEnabled</span></span>
* <span data-ttu-id="4ab6a-112">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4ab6a-112">mailNickname</span></span>
* <span data-ttu-id="4ab6a-113">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab6a-113">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="4ab6a-114">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="4ab6a-114">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="4ab6a-115">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="4ab6a-115">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="4ab6a-116">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="4ab6a-116">proxyAddresses</span></span>
* <span data-ttu-id="4ab6a-117">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="4ab6a-117">securityEnabled</span></span>
* <span data-ttu-id="4ab6a-118">visibility</span><span class="sxs-lookup"><span data-stu-id="4ab6a-118">visibility</span></span>

<span data-ttu-id="4ab6a-119">Die folgenden Gruppeneigenschaften werden standardmäßig nicht zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="4ab6a-119">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="4ab6a-120">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="4ab6a-120">allowExternalSenders</span></span>
* <span data-ttu-id="4ab6a-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="4ab6a-121">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="4ab6a-122">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="4ab6a-122">isSubscribedByMail</span></span>
* <span data-ttu-id="4ab6a-123">unseenCount</span><span class="sxs-lookup"><span data-stu-id="4ab6a-123">unseenCount</span></span>

<span data-ttu-id="4ab6a-p102">Verwenden Sie zum Abrufen dieser Eigenschaften den **$select**-Abfrageparameter. Hier einige Beispiele:</span><span class="sxs-lookup"><span data-stu-id="4ab6a-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="4ab6a-126">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4ab6a-126">Permissions</span></span>
<span data-ttu-id="4ab6a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4ab6a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4ab6a-129">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ab6a-129">Permission type</span></span>      | <span data-ttu-id="4ab6a-130">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ab6a-130">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4ab6a-131">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ab6a-131">Delegated (work or school account)</span></span> | <span data-ttu-id="4ab6a-132">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ab6a-132">Group.Read.All, Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4ab6a-133">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ab6a-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ab6a-134">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ab6a-134">Not supported.</span></span>    | 
|<span data-ttu-id="4ab6a-135">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ab6a-135">Application</span></span> | <span data-ttu-id="4ab6a-136">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ab6a-136">Group.Read.All, Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4ab6a-137">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ab6a-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ab6a-138">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4ab6a-138">Optional query parameters</span></span>
<span data-ttu-id="4ab6a-139">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4ab6a-139">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4ab6a-140">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ab6a-140">Request headers</span></span>
| <span data-ttu-id="4ab6a-141">Name</span><span class="sxs-lookup"><span data-stu-id="4ab6a-141">Name</span></span>       | <span data-ttu-id="4ab6a-142">Typ</span><span class="sxs-lookup"><span data-stu-id="4ab6a-142">Type</span></span> | <span data-ttu-id="4ab6a-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ab6a-143">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4ab6a-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ab6a-144">Authorization</span></span>  | <span data-ttu-id="4ab6a-145">string</span><span class="sxs-lookup"><span data-stu-id="4ab6a-145">string</span></span>  | <span data-ttu-id="4ab6a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4ab6a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ab6a-148">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ab6a-148">Request body</span></span>
<span data-ttu-id="4ab6a-149">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4ab6a-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ab6a-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ab6a-150">Response</span></span>

<span data-ttu-id="4ab6a-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [photo](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ab6a-151">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ab6a-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ab6a-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ab6a-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ab6a-153">Request</span></span>
<span data-ttu-id="4ab6a-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ab6a-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```
##### <a name="response"></a><span data-ttu-id="4ab6a-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ab6a-155">Response</span></span>
<span data-ttu-id="4ab6a-156">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4ab6a-156">Here is an example of the response.</span></span>

<span data-ttu-id="4ab6a-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden, wie oben beschrieben, die Standardeigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ab6a-p105">Note: The response object shown here may be truncated for brevity. The default properties will be returned from an actual call, as described above.</span></span>
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
