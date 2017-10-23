# <a name="group-getmemberobjects"></a><span data-ttu-id="1db84-101">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="1db84-101">group: getMemberObjects</span></span>
<span data-ttu-id="1db84-p101">Diese API gibt alle Gruppen zurück, in denen die angegebene Gruppe Mitglied ist. Die Überprüfung ist transitiv. Hinweis: Gruppen können nicht Mitglieder von Verzeichnisrollen sein, es werden daher keine Verzeichnisrollen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1db84-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="1db84-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1db84-105">Permissions</span></span>
<span data-ttu-id="1db84-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1db84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1db84-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1db84-108">Permission type</span></span>      | <span data-ttu-id="1db84-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1db84-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1db84-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1db84-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1db84-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1db84-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1db84-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1db84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1db84-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1db84-113">Not supported.</span></span>    |
|<span data-ttu-id="1db84-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1db84-114">Application</span></span> | <span data-ttu-id="1db84-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1db84-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1db84-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1db84-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="1db84-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1db84-117">Request headers</span></span>
| <span data-ttu-id="1db84-118">Name</span><span class="sxs-lookup"><span data-stu-id="1db84-118">Name</span></span>       | <span data-ttu-id="1db84-119">Typ</span><span class="sxs-lookup"><span data-stu-id="1db84-119">Type</span></span> | <span data-ttu-id="1db84-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1db84-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1db84-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1db84-121">Authorization</span></span>  | <span data-ttu-id="1db84-122">string</span><span class="sxs-lookup"><span data-stu-id="1db84-122">string</span></span>  | <span data-ttu-id="1db84-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1db84-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1db84-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1db84-125">Request body</span></span>
<span data-ttu-id="1db84-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="1db84-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1db84-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="1db84-127">Parameter</span></span>    | <span data-ttu-id="1db84-128">Typ</span><span class="sxs-lookup"><span data-stu-id="1db84-128">Type</span></span>   |<span data-ttu-id="1db84-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1db84-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1db84-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="1db84-130">securityEnabledOnly</span></span>|<span data-ttu-id="1db84-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="1db84-131">Boolean</span></span>| <span data-ttu-id="1db84-p104">Festgelegt auf **false**. Die Option, dass nur Gruppen mit aktivierter Sicherheit zurückgegeben werden, wird nur für Benutzer unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1db84-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="1db84-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1db84-134">Response</span></span>
<span data-ttu-id="1db84-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen enthält, von denen die Gruppe ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="1db84-135">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="1db84-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1db84-136">Example</span></span>
<span data-ttu-id="1db84-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1db84-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1db84-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1db84-138">Request</span></span>
<span data-ttu-id="1db84-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1db84-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

##### <a name="response"></a><span data-ttu-id="1db84-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1db84-140">Response</span></span>
<span data-ttu-id="1db84-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1db84-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
