# <a name="delete-open-extension"></a><span data-ttu-id="245d1-101">Offene Erweiterung löschen</span><span class="sxs-lookup"><span data-stu-id="245d1-101">Delete open extension</span></span>

<span data-ttu-id="245d1-102">Mit dieser API können Sie offene Erweiterungen (Objekte des Typs [openTypeExtension](../resources/openTypeExtension.md) aus der jeweils angegebenen Ressourceninstanz löschen.</span><span class="sxs-lookup"><span data-stu-id="245d1-102">Delete an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="245d1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="245d1-103">Permissions</span></span>

<span data-ttu-id="245d1-104">Je nach der Ressource, die Sie die Erweiterung von löschen möchten, und die Berechtigung Typ (delegierte oder-Anwendung) angefordert, die Berechtigung, die in der folgenden Tabelle angegebenen mit den geringsten ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="245d1-104">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="245d1-105">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="245d1-105">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="245d1-106">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="245d1-106">Supported resource</span></span> | <span data-ttu-id="245d1-107">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="245d1-107">Delegated (work or school account)</span></span> | <span data-ttu-id="245d1-108">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="245d1-108">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="245d1-109">Anwendung</span><span class="sxs-lookup"><span data-stu-id="245d1-109">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="245d1-110">device</span><span class="sxs-lookup"><span data-stu-id="245d1-110">device</span></span>](../resources/device.md) | <span data-ttu-id="245d1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="245d1-111">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="245d1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="245d1-112">Not supported</span></span> | <span data-ttu-id="245d1-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="245d1-113">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="245d1-114">event</span><span class="sxs-lookup"><span data-stu-id="245d1-114">event</span></span>](../resources/event.md) | <span data-ttu-id="245d1-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="245d1-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="245d1-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="245d1-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="245d1-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="245d1-117">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="245d1-118">group</span><span class="sxs-lookup"><span data-stu-id="245d1-118">group</span></span>](../resources/group.md) | <span data-ttu-id="245d1-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="245d1-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="245d1-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="245d1-120">Not supported</span></span> | <span data-ttu-id="245d1-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="245d1-121">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="245d1-122">group event</span><span class="sxs-lookup"><span data-stu-id="245d1-122">group event</span></span>](../resources/event.md) | <span data-ttu-id="245d1-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="245d1-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="245d1-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="245d1-124">Not supported</span></span> | <span data-ttu-id="245d1-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="245d1-125">Not supported</span></span> |
| [<span data-ttu-id="245d1-126">group post</span><span class="sxs-lookup"><span data-stu-id="245d1-126">group post</span></span>](../resources/post.md) | <span data-ttu-id="245d1-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="245d1-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="245d1-128">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="245d1-128">Not supported</span></span> | <span data-ttu-id="245d1-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="245d1-129">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="245d1-130">message</span><span class="sxs-lookup"><span data-stu-id="245d1-130">message</span></span>](../resources/message.md) | <span data-ttu-id="245d1-131">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="245d1-131">Mail.ReadWrite</span></span> | <span data-ttu-id="245d1-132">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="245d1-132">Mail.ReadWrite</span></span> | <span data-ttu-id="245d1-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="245d1-133">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="245d1-134">organization</span><span class="sxs-lookup"><span data-stu-id="245d1-134">organization</span></span>](../resources/organization.md) | <span data-ttu-id="245d1-135">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="245d1-135">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="245d1-136">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="245d1-136">Not supported</span></span> | <span data-ttu-id="245d1-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="245d1-137">Not supported</span></span> |
| [<span data-ttu-id="245d1-138">personal contact</span><span class="sxs-lookup"><span data-stu-id="245d1-138">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="245d1-139">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="245d1-139">Contacts.ReadWrite</span></span> | <span data-ttu-id="245d1-140">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="245d1-140">Contacts.ReadWrite</span></span> | <span data-ttu-id="245d1-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="245d1-141">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="245d1-142">user</span><span class="sxs-lookup"><span data-stu-id="245d1-142">user</span></span>](../resources/user.md) | <span data-ttu-id="245d1-143">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="245d1-143">User.ReadWrite.All</span></span> | <span data-ttu-id="245d1-144">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="245d1-144">User.ReadWrite</span></span> | <span data-ttu-id="245d1-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="245d1-145">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="245d1-146">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="245d1-146">HTTP request</span></span>
<span data-ttu-id="245d1-147">In der Anforderung geben Sie die Ressourceninstanz an, spezifizieren in der Navigationseigenschaft **extensions** dieser Instanz die Erweiterung und wenden anschließend den Befehl `DELETE` auf diese Erweiterungsinstanz an.</span><span class="sxs-lookup"><span data-stu-id="245d1-147">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="245d1-p102">**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Identifizieren einer Ressourceninstanz, um eine Erweiterung daraus zu löschen. Alle anderen Syntaxen, mit denen Sie diese Ressourceninstanzen identifizieren können, unterstützen das Löschen offener Erweiterungen daraus in einer ähnlichen Weise.</span><span class="sxs-lookup"><span data-stu-id="245d1-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="245d1-150">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="245d1-150">Path parameters</span></span>
|<span data-ttu-id="245d1-151">Parameter</span><span class="sxs-lookup"><span data-stu-id="245d1-151">Parameter</span></span>|<span data-ttu-id="245d1-152">Typ</span><span class="sxs-lookup"><span data-stu-id="245d1-152">Type</span></span>|<span data-ttu-id="245d1-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="245d1-153">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="245d1-154">id</span><span class="sxs-lookup"><span data-stu-id="245d1-154">id</span></span>|<span data-ttu-id="245d1-155">string</span><span class="sxs-lookup"><span data-stu-id="245d1-155">string</span></span>|<span data-ttu-id="245d1-p103">Ein eindeutiger Bezeichner für eine Instanz in der entsprechenden Sammlung. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="245d1-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="245d1-158">extensionId</span><span class="sxs-lookup"><span data-stu-id="245d1-158">extensionId</span></span>|<span data-ttu-id="245d1-159">string</span><span class="sxs-lookup"><span data-stu-id="245d1-159">string</span></span>|<span data-ttu-id="245d1-p104">Dies kann ein Erweiterungsname sein. Der Erweiterungsname ist ein eindeutiger Textbezeichner der Erweiterung oder ein vollqualifizierter Name, der den Erweiterungstyp und den eindeutigen Textbezeichner verkettet. Der vollqualifizierte Name wird beim Erstellen der Erweiterung in der `id`-Eigenschaft zurückgegeben. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="245d1-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="245d1-163">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="245d1-163">Request headers</span></span>
| <span data-ttu-id="245d1-164">Name</span><span class="sxs-lookup"><span data-stu-id="245d1-164">Name</span></span>       | <span data-ttu-id="245d1-165">Wert</span><span class="sxs-lookup"><span data-stu-id="245d1-165">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="245d1-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="245d1-166">Authorization</span></span> | <span data-ttu-id="245d1-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="245d1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="245d1-169">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="245d1-169">Request body</span></span>
<span data-ttu-id="245d1-170">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="245d1-170">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="245d1-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="245d1-171">Response</span></span>

<span data-ttu-id="245d1-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="245d1-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="245d1-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="245d1-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="245d1-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="245d1-175">Request</span></span>
<span data-ttu-id="245d1-176">Das erste Beispiel referenziert eine Erweiterung über ihren Namen und löscht die Erweiterung in der angegebenen Nachricht.</span><span class="sxs-lookup"><span data-stu-id="245d1-176">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="245d1-177">Das zweite Beispiel löscht eine Erweiterung in dem angegebenen Gruppenereignis.</span><span class="sxs-lookup"><span data-stu-id="245d1-177">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="245d1-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="245d1-178">Response</span></span>
<span data-ttu-id="245d1-179">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="245d1-179">Here is an example of the response.</span></span>
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