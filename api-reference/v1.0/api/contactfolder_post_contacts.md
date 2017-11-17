# <a name="create-contact"></a><span data-ttu-id="ef1ec-101">Kontakt erstellen</span><span class="sxs-lookup"><span data-stu-id="ef1ec-101">Create Contact</span></span>

<span data-ttu-id="ef1ec-102">Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.</span><span class="sxs-lookup"><span data-stu-id="ef1ec-102">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef1ec-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ef1ec-103">Permissions</span></span>

<span data-ttu-id="ef1ec-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ef1ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ef1ec-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef1ec-106">Permission type</span></span>      | <span data-ttu-id="ef1ec-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef1ec-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef1ec-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef1ec-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ef1ec-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef1ec-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ef1ec-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef1ec-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef1ec-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef1ec-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ef1ec-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef1ec-112">Application</span></span> | <span data-ttu-id="ef1ec-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef1ec-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef1ec-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef1ec-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="ef1ec-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef1ec-115">Request headers</span></span>

| <span data-ttu-id="ef1ec-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ef1ec-116">Header</span></span>       | <span data-ttu-id="ef1ec-117">Wert</span><span class="sxs-lookup"><span data-stu-id="ef1ec-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ef1ec-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef1ec-118">Authorization</span></span>  | <span data-ttu-id="ef1ec-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ef1ec-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ef1ec-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef1ec-121">Content-Type</span></span>  | <span data-ttu-id="ef1ec-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="ef1ec-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ef1ec-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef1ec-124">Request body</span></span>
<span data-ttu-id="ef1ec-125">Geben Sie im Anforderungstext eine JSON-Darstellung des [Contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ef1ec-125">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ef1ec-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef1ec-126">Response</span></span>

<span data-ttu-id="ef1ec-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef1ec-127">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef1ec-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef1ec-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef1ec-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef1ec-129">Request</span></span>

<span data-ttu-id="ef1ec-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef1ec-130">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<span data-ttu-id="ef1ec-131">Geben Sie im Anforderungstext eine JSON-Darstellung des [Contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ef1ec-131">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="ef1ec-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef1ec-132">Response</span></span>

<span data-ttu-id="ef1ec-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ef1ec-133">Here is an example of the response.</span></span> <span data-ttu-id="ef1ec-134">**Hinweis:** Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ef1ec-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ef1ec-135">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ef1ec-135">All default properties will be returned from the actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
