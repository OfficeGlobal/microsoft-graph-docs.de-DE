# <a name="delete-open-extension"></a><span data-ttu-id="ad3c5-101">Offene Erweiterung löschen</span><span class="sxs-lookup"><span data-stu-id="ad3c5-101">Delete open extension</span></span>

<span data-ttu-id="ad3c5-102">Mit dieser API können Sie offene Erweiterungen (Objekte des Typs [openTypeExtension](../resources/openTypeExtension.md) aus der jeweils angegebenen Ressourceninstanz löschen.</span><span class="sxs-lookup"><span data-stu-id="ad3c5-102">Delete an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ad3c5-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ad3c5-103">Permissions</span></span>

<span data-ttu-id="ad3c5-p101">Zum Aufrufen dieser API ist eine der folgenden Berechtigungen erforderlich (je nachdem, aus welcher Ressource Sie die Erweiterung löschen möchten): Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ad3c5-p101">One of the following permissions is required to call this API, depending on the resource you're deleting the extension from. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad3c5-106">**Unterstützte Ressource**</span><span class="sxs-lookup"><span data-stu-id="ad3c5-106">**Supported resource**</span></span>|<span data-ttu-id="ad3c5-107">**Berechtigung**</span><span class="sxs-lookup"><span data-stu-id="ad3c5-107">**Permission**</span></span>|<span data-ttu-id="ad3c5-108">**Unterstützte Ressource**</span><span class="sxs-lookup"><span data-stu-id="ad3c5-108">**Supported resource**</span></span>|<span data-ttu-id="ad3c5-109">**Berechtigung**</span><span class="sxs-lookup"><span data-stu-id="ad3c5-109">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="ad3c5-110">device</span><span class="sxs-lookup"><span data-stu-id="ad3c5-110">device</span></span>](../resources/device.md) | <span data-ttu-id="ad3c5-111">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad3c5-111">Device.ReadWrite.All</span></span> | [<span data-ttu-id="ad3c5-112">event</span><span class="sxs-lookup"><span data-stu-id="ad3c5-112">event</span></span>](../resources/event.md) | <span data-ttu-id="ad3c5-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad3c5-113">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="ad3c5-114">group</span><span class="sxs-lookup"><span data-stu-id="ad3c5-114">group</span></span>](../resources/group.md) | <span data-ttu-id="ad3c5-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad3c5-115">Group.ReadWrite.All</span></span> | [<span data-ttu-id="ad3c5-116">group event</span><span class="sxs-lookup"><span data-stu-id="ad3c5-116">group event</span></span>](../resources/event.md) | <span data-ttu-id="ad3c5-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad3c5-117">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="ad3c5-118">group post</span><span class="sxs-lookup"><span data-stu-id="ad3c5-118">group post</span></span>](../resources/post.md) | <span data-ttu-id="ad3c5-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad3c5-119">Group.ReadWrite.All</span></span> | [<span data-ttu-id="ad3c5-120">message</span><span class="sxs-lookup"><span data-stu-id="ad3c5-120">message</span></span>](../resources/message.md) | <span data-ttu-id="ad3c5-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad3c5-121">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="ad3c5-122">organization</span><span class="sxs-lookup"><span data-stu-id="ad3c5-122">organization</span></span>](../resources/organization.md) | <span data-ttu-id="ad3c5-123">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad3c5-123">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="ad3c5-124">personal contact</span><span class="sxs-lookup"><span data-stu-id="ad3c5-124">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="ad3c5-125">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad3c5-125">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="ad3c5-126">user</span><span class="sxs-lookup"><span data-stu-id="ad3c5-126">user</span></span>](../resources/user.md) | <span data-ttu-id="ad3c5-127">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad3c5-127">Directory.AccessAsUser.All</span></span> | | |

## <a name="http-request"></a><span data-ttu-id="ad3c5-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad3c5-128">HTTP request</span></span>
<span data-ttu-id="ad3c5-129">In der Anforderung geben Sie die Ressourceninstanz an, spezifizieren in der Navigationseigenschaft **extensions** dieser Instanz die Erweiterung und wenden anschließend den Befehl `DELETE` auf diese Erweiterungsinstanz an.</span><span class="sxs-lookup"><span data-stu-id="ad3c5-129">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="ad3c5-p102">**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Identifizieren einer Ressourceninstanz, um eine Erweiterung daraus zu löschen. Alle anderen Syntaxen, mit denen Sie diese Ressourceninstanzen identifizieren können, unterstützen das Löschen offener Erweiterungen daraus in einer ähnlichen Weise.</span><span class="sxs-lookup"><span data-stu-id="ad3c5-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="parameters"></a><span data-ttu-id="ad3c5-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="ad3c5-132">Parameters</span></span>
|<span data-ttu-id="ad3c5-133">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="ad3c5-133">**Parameter**</span></span>|<span data-ttu-id="ad3c5-134">**Typ**</span><span class="sxs-lookup"><span data-stu-id="ad3c5-134">**Type**</span></span>|<span data-ttu-id="ad3c5-135">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="ad3c5-135">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ad3c5-136">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="ad3c5-136">_URL parameters_</span></span>|
|<span data-ttu-id="ad3c5-137">id</span><span class="sxs-lookup"><span data-stu-id="ad3c5-137">id</span></span>|<span data-ttu-id="ad3c5-138">string</span><span class="sxs-lookup"><span data-stu-id="ad3c5-138">string</span></span>|<span data-ttu-id="ad3c5-p103">Ein eindeutiger Bezeichner für eine Instanz in der entsprechenden Sammlung. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ad3c5-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="ad3c5-141">extensionId</span><span class="sxs-lookup"><span data-stu-id="ad3c5-141">extensionId</span></span>|<span data-ttu-id="ad3c5-142">string</span><span class="sxs-lookup"><span data-stu-id="ad3c5-142">string</span></span>|<span data-ttu-id="ad3c5-p104">Dies kann ein Erweiterungsname sein. Der Erweiterungsname ist ein eindeutiger Textbezeichner der Erweiterung oder ein vollqualifizierter Name, der den Erweiterungstyp und den eindeutigen Textbezeichner verkettet. Der vollqualifizierte Name wird beim Erstellen der Erweiterung in der `id`-Eigenschaft zurückgegeben. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ad3c5-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ad3c5-146">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ad3c5-146">Request headers</span></span>
| <span data-ttu-id="ad3c5-147">Name</span><span class="sxs-lookup"><span data-stu-id="ad3c5-147">Name</span></span>       | <span data-ttu-id="ad3c5-148">Wert</span><span class="sxs-lookup"><span data-stu-id="ad3c5-148">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ad3c5-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad3c5-149">Authorization</span></span> | <span data-ttu-id="ad3c5-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ad3c5-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad3c5-152">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ad3c5-152">Request body</span></span>
<span data-ttu-id="ad3c5-153">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ad3c5-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad3c5-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad3c5-154">Response</span></span>

<span data-ttu-id="ad3c5-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ad3c5-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad3c5-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ad3c5-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad3c5-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad3c5-158">Request</span></span>
<span data-ttu-id="ad3c5-159">Das erste Beispiel referenziert eine Erweiterung über ihren Namen und löscht die Erweiterung in der angegebenen Nachricht.</span><span class="sxs-lookup"><span data-stu-id="ad3c5-159">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="ad3c5-160">Das zweite Beispiel löscht eine Erweiterung in dem angegebenen Gruppenereignis.</span><span class="sxs-lookup"><span data-stu-id="ad3c5-160">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a><span data-ttu-id="ad3c5-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad3c5-161">Response</span></span>
<span data-ttu-id="ad3c5-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ad3c5-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->