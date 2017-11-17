# <a name="update-contactfolder"></a><span data-ttu-id="5d72d-101">contactFolder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5d72d-101">Update contactfolder</span></span>

<span data-ttu-id="5d72d-102">Mit dieser API können Sie die Eigenschaften von Objekten des Typs „contactfolder“ aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="5d72d-102">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d72d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5d72d-103">Permissions</span></span>
<span data-ttu-id="5d72d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d72d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5d72d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d72d-106">Permission type</span></span>      | <span data-ttu-id="5d72d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d72d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d72d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d72d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5d72d-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d72d-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5d72d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d72d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d72d-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d72d-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5d72d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d72d-112">Application</span></span> | <span data-ttu-id="5d72d-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d72d-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d72d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d72d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5d72d-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d72d-115">Request headers</span></span>
| <span data-ttu-id="5d72d-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5d72d-116">Header</span></span>       | <span data-ttu-id="5d72d-117">Wert</span><span class="sxs-lookup"><span data-stu-id="5d72d-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5d72d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d72d-118">Authorization</span></span>  | <span data-ttu-id="5d72d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5d72d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5d72d-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d72d-121">Content-Type</span></span>  | <span data-ttu-id="5d72d-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="5d72d-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5d72d-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d72d-124">Request body</span></span>
<span data-ttu-id="5d72d-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="5d72d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5d72d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d72d-128">Property</span></span>     | <span data-ttu-id="5d72d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5d72d-129">Type</span></span>   |<span data-ttu-id="5d72d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d72d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d72d-131">displayName</span><span class="sxs-lookup"><span data-stu-id="5d72d-131">displayName</span></span>|<span data-ttu-id="5d72d-132">String</span><span class="sxs-lookup"><span data-stu-id="5d72d-132">String</span></span>|<span data-ttu-id="5d72d-133">Der Anzeigename des Ordners.</span><span class="sxs-lookup"><span data-stu-id="5d72d-133">The folder's display name.</span></span>|
|<span data-ttu-id="5d72d-134">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="5d72d-134">parentFolderId</span></span>|<span data-ttu-id="5d72d-135">String</span><span class="sxs-lookup"><span data-stu-id="5d72d-135">String</span></span>|<span data-ttu-id="5d72d-136">Die ID des übergeordneten Ordners des Ordners.</span><span class="sxs-lookup"><span data-stu-id="5d72d-136">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="5d72d-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d72d-137">Response</span></span>

<span data-ttu-id="5d72d-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [contactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d72d-138">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d72d-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d72d-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d72d-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d72d-140">Request</span></span>
<span data-ttu-id="5d72d-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d72d-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="5d72d-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d72d-142">Response</span></span>
<span data-ttu-id="5d72d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d72d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
