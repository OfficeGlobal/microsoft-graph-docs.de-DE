# <a name="create-contactfolder"></a><span data-ttu-id="134de-101">ContactFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="134de-101">Create ContactFolder</span></span>

<span data-ttu-id="134de-102">Erstellt einen neuen contactFolder unter dem Standardkontaktordner des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="134de-102">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="134de-103">Sie können auch [eine neue Ressource des Typs „contactfolder“ als untergeordnetes Element eines anderen Kontaktordners erstellen](contactfolder_post_childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="134de-103">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder_post_childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="134de-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="134de-104">Permissions</span></span>
<span data-ttu-id="134de-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="134de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="134de-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="134de-107">Permission type</span></span>      | <span data-ttu-id="134de-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="134de-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="134de-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="134de-109">Delegated (work or school account)</span></span> | <span data-ttu-id="134de-110">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="134de-110">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="134de-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="134de-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="134de-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="134de-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="134de-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="134de-113">Application</span></span> | <span data-ttu-id="134de-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="134de-114">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="134de-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="134de-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="134de-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="134de-116">Request headers</span></span>
| <span data-ttu-id="134de-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="134de-117">Header</span></span>       | <span data-ttu-id="134de-118">Wert</span><span class="sxs-lookup"><span data-stu-id="134de-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="134de-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="134de-119">Authorization</span></span>  | <span data-ttu-id="134de-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="134de-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="134de-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="134de-122">Content-Type</span></span>  | <span data-ttu-id="134de-123">application/json</span><span class="sxs-lookup"><span data-stu-id="134de-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="134de-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="134de-124">Request body</span></span>
<span data-ttu-id="134de-125">Geben Sie im Anforderungstext eine JSON-Darstellung des [ContactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="134de-125">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="134de-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="134de-126">Response</span></span>

<span data-ttu-id="134de-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [ContactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="134de-127">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="134de-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="134de-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="134de-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="134de-129">Request</span></span>
<span data-ttu-id="134de-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="134de-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
<span data-ttu-id="134de-131">Geben Sie im Anforderungstext eine JSON-Darstellung des [contactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="134de-131">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="134de-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="134de-132">Response</span></span>
<span data-ttu-id="134de-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="134de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
