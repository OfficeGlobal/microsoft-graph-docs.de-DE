---
title: Datenerweiterung aktualisieren
description: 'Aktualisieren Sie eine offene Erweiterung (openTypeExtension-Objekt) mit den Eigenschaften im Anforderungsheader:'
ms.openlocfilehash: 3b35ac56898aa910f0da5e3ac311fefd67fff12d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060045"
---
# <a name="update-open-extension"></a><span data-ttu-id="2a6fe-103">Datenerweiterung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2a6fe-103">Update open extension</span></span>

> <span data-ttu-id="2a6fe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a6fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2a6fe-106">Aktualisieren Sie eine offene Erweiterung ([openTypeExtension](../resources/opentypeextension.md)-Objekt) mit den Eigenschaften im Anforderungsheader:</span><span class="sxs-lookup"><span data-stu-id="2a6fe-106">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="2a6fe-107">Wenn eine Eigenschaft im Anforderungsheader mit dem Name einer vorhandenen Eigenschaft in der Erweiterung übereinstimmt, werden die Daten in die Erweiterung aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-107">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="2a6fe-108">Andernfalls werden die Eigenschaft und die entsprechenden Daten zur Erweiterung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-108">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="2a6fe-109">Die Daten in einer Erweiterung können Grundtypen oder Arrays von Grundtypen sein.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-109">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a6fe-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2a6fe-110">Permissions</span></span>

<span data-ttu-id="2a6fe-111">Je nach der Ressource, der die Erweiterung in erstellt wurde und die Berechtigung Typ (delegierte oder-Anwendung) angefordert, die Berechtigung, die in der folgenden Tabelle angegebenen mit den geringsten ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-111">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2a6fe-112">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a6fe-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a6fe-113">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="2a6fe-113">Supported resource</span></span> | <span data-ttu-id="2a6fe-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a6fe-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2a6fe-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a6fe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a6fe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a6fe-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="2a6fe-117">Gerät</span><span class="sxs-lookup"><span data-stu-id="2a6fe-117">device</span></span>](../resources/device.md) | <span data-ttu-id="2a6fe-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a6fe-118">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="2a6fe-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a6fe-119">Not supported</span></span> | <span data-ttu-id="2a6fe-120">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a6fe-120">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="2a6fe-121">event</span><span class="sxs-lookup"><span data-stu-id="2a6fe-121">event</span></span>](../resources/event.md) | <span data-ttu-id="2a6fe-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a6fe-122">Calendars.ReadWrite</span></span> | <span data-ttu-id="2a6fe-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a6fe-123">Calendars.ReadWrite</span></span> | <span data-ttu-id="2a6fe-124">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a6fe-124">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="2a6fe-125">group</span><span class="sxs-lookup"><span data-stu-id="2a6fe-125">group</span></span>](../resources/group.md) | <span data-ttu-id="2a6fe-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a6fe-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="2a6fe-127">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a6fe-127">Not supported</span></span> | <span data-ttu-id="2a6fe-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a6fe-128">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="2a6fe-129">group event</span><span class="sxs-lookup"><span data-stu-id="2a6fe-129">group event</span></span>](../resources/event.md) | <span data-ttu-id="2a6fe-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a6fe-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="2a6fe-131">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a6fe-131">Not supported</span></span> | <span data-ttu-id="2a6fe-132">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a6fe-132">Not supported</span></span> |
| [<span data-ttu-id="2a6fe-133">group post</span><span class="sxs-lookup"><span data-stu-id="2a6fe-133">group post</span></span>](../resources/post.md) | <span data-ttu-id="2a6fe-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a6fe-134">Group.ReadWrite.All</span></span> | <span data-ttu-id="2a6fe-135">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a6fe-135">Not supported</span></span> | <span data-ttu-id="2a6fe-136">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a6fe-136">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="2a6fe-137">message</span><span class="sxs-lookup"><span data-stu-id="2a6fe-137">message</span></span>](../resources/message.md) | <span data-ttu-id="2a6fe-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a6fe-138">Mail.ReadWrite</span></span> | <span data-ttu-id="2a6fe-139">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a6fe-139">Mail.ReadWrite</span></span> | <span data-ttu-id="2a6fe-140">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a6fe-140">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="2a6fe-141">organization</span><span class="sxs-lookup"><span data-stu-id="2a6fe-141">organization</span></span>](../resources/organization.md) | <span data-ttu-id="2a6fe-142">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a6fe-142">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="2a6fe-143">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a6fe-143">Not supported</span></span> | <span data-ttu-id="2a6fe-144">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a6fe-144">Not supported</span></span> |
| [<span data-ttu-id="2a6fe-145">personal contact</span><span class="sxs-lookup"><span data-stu-id="2a6fe-145">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="2a6fe-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a6fe-146">Contacts.ReadWrite</span></span> | <span data-ttu-id="2a6fe-147">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a6fe-147">Contacts.ReadWrite</span></span> | <span data-ttu-id="2a6fe-148">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a6fe-148">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="2a6fe-149">user</span><span class="sxs-lookup"><span data-stu-id="2a6fe-149">user</span></span>](../resources/user.md) | <span data-ttu-id="2a6fe-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a6fe-150">User.ReadWrite.All</span></span> | <span data-ttu-id="2a6fe-151">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a6fe-151">User.ReadWrite</span></span> | <span data-ttu-id="2a6fe-152">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a6fe-152">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a6fe-153">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a6fe-153">HTTP request</span></span>

<span data-ttu-id="2a6fe-154">In der Anforderung geben Sie die Ressourceninstanz an, spezifizieren in der Navigationseigenschaft **extensions** dieser Instanz die Erweiterung und wenden anschließend den Befehl `PATCH` auf diese Erweiterungsinstanz an.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-154">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{Id}/extensions/{extensionId}
PATCH /devices/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/extensions/{extensionId}
PATCH /groups/{id}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
PATCH /organization/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="2a6fe-p103">**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Identifizieren einer Ressourceninstanz, um eine Erweiterung darin zu aktualisieren. Alle anderen Syntaxen, mit denen Sie diese Ressourceninstanzen identifizieren können, unterstützen das Aktualisieren offener Erweiterungen darin in einer ähnlichen Weise.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it. All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="2a6fe-157">Im Abschnitt [Anforderungstext](#request-body) wird beschrieben, wie Sie benutzerdefinierte Daten zur Änderung oder Ergänzung der Erweiterung in den Anforderungstext einschließen können.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-157">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="2a6fe-158">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="2a6fe-158">Path parameters</span></span>
|<span data-ttu-id="2a6fe-159">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="2a6fe-159">**Parameter**</span></span>|<span data-ttu-id="2a6fe-160">**Typ**</span><span class="sxs-lookup"><span data-stu-id="2a6fe-160">**Type**</span></span>|<span data-ttu-id="2a6fe-161">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="2a6fe-161">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2a6fe-162">id</span><span class="sxs-lookup"><span data-stu-id="2a6fe-162">id</span></span>|<span data-ttu-id="2a6fe-163">string</span><span class="sxs-lookup"><span data-stu-id="2a6fe-163">string</span></span>|<span data-ttu-id="2a6fe-p104">Ein eindeutiger Bezeichner für eine Instanz der entsprechenden Sammlung. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2a6fe-p104">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="2a6fe-166">extensionId</span><span class="sxs-lookup"><span data-stu-id="2a6fe-166">extensionId</span></span>|<span data-ttu-id="2a6fe-167">string</span><span class="sxs-lookup"><span data-stu-id="2a6fe-167">string</span></span>|<span data-ttu-id="2a6fe-p105">Dies kann ein Erweiterungsname sein. Der Erweiterungsname ist ein eindeutiger Textbezeichner einer Erweiterung oder ein vollqualifizierter Name, der den Erweiterungstyp und den eindeutigen Textbezeichner verkettet. Der vollqualifizierte Name wird beim Erstellen der Erweiterung in der `id`-Eigenschaft zurückgegeben. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2a6fe-p105">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2a6fe-171">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a6fe-171">Request headers</span></span>
| <span data-ttu-id="2a6fe-172">Name</span><span class="sxs-lookup"><span data-stu-id="2a6fe-172">Name</span></span>       | <span data-ttu-id="2a6fe-173">Wert</span><span class="sxs-lookup"><span data-stu-id="2a6fe-173">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2a6fe-174">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a6fe-174">Authorization</span></span> | <span data-ttu-id="2a6fe-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a6fe-177">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a6fe-177">Content-Type</span></span> | <span data-ttu-id="2a6fe-178">application/json</span><span class="sxs-lookup"><span data-stu-id="2a6fe-178">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a6fe-179">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a6fe-179">Request body</span></span>

<span data-ttu-id="2a6fe-p107">Stellen Sie den JSON-Text eines [openTypeExtension](../resources/opentypeextension.md)-Objekts mit den folgenden erforderlichen Name-Wert-Paaren und allen benutzerdefinierten Daten bereit, die geändert oder zu dieser Erweiterung hinzugefügt werden sollen. Die Daten in der JSON-Nutzlast können Grundtypen oder Arrays von Grundtypen sein.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-p107">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="2a6fe-182">Name</span><span class="sxs-lookup"><span data-stu-id="2a6fe-182">Name</span></span>       | <span data-ttu-id="2a6fe-183">Wert</span><span class="sxs-lookup"><span data-stu-id="2a6fe-183">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2a6fe-184">@odata.type</span><span class="sxs-lookup"><span data-stu-id="2a6fe-184">@odata.type</span></span> | <span data-ttu-id="2a6fe-185">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="2a6fe-185">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="2a6fe-186">extensionName</span><span class="sxs-lookup"><span data-stu-id="2a6fe-186">extensionName</span></span> | <span data-ttu-id="2a6fe-187">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="2a6fe-187">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="2a6fe-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a6fe-188">Response</span></span>

<span data-ttu-id="2a6fe-189">Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und das aktualisierte [openTypeExtension](../resources/opentypeextension.md)-Objekt zurück.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-189">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="2a6fe-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a6fe-190">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="2a6fe-191">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="2a6fe-191">Request 1</span></span>

<span data-ttu-id="2a6fe-p108">Im ersten Beispiel wird gezeigt, wie eine Erweiterung in einer Nachricht aktualisiert wird. Die Erweiterung wird anfänglich durch die folgende JSON-Nutzlast dargestellt:</span><span class="sxs-lookup"><span data-stu-id="2a6fe-p108">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

<span data-ttu-id="2a6fe-194">Sie können anhand des Namens auf die Erweiterung verweisen:</span><span class="sxs-lookup"><span data-stu-id="2a6fe-194">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="2a6fe-195">Sie können auch anhand des vollqualifizierten Namens auf die Erweiterung verweisen:</span><span class="sxs-lookup"><span data-stu-id="2a6fe-195">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

<span data-ttu-id="2a6fe-196">Sie können die Beispielanforderung und den folgenden Anforderungstext verwenden, um die oben genannte Erweiterung auf folgende Weise zu aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="2a6fe-196">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="2a6fe-197">Durch Ändern des `companyName` von `Wingtip Toys` zu `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="2a6fe-197">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="2a6fe-198">Durch Ändern des `dealValue` von `500050` zu `500100`</span><span class="sxs-lookup"><span data-stu-id="2a6fe-198">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="2a6fe-199">Durch Hinzufügen neuer Daten als die benutzerdefinierte `updated`-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a6fe-199">Adding new data as the custom property `updated`</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "Microsoft.Graph.OpenTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a><span data-ttu-id="2a6fe-200">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="2a6fe-200">Response 1</span></span>

<span data-ttu-id="2a6fe-201">Es wird unabhängig von der zur Referenzierung der Erweiterung verwendeten Methode jeweils die gleiche Antwort zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-201">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": 500100,
    "expirationDate": "2015-12-03T10:00:00Z",
    "updated": "2015-10-29T11:00:00.000Z"
}
```

****

#### <a name="request-2"></a><span data-ttu-id="2a6fe-202">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="2a6fe-202">Request 2</span></span>

<span data-ttu-id="2a6fe-p109">Im zweiten Beispiel wird gezeigt, wie eine Erweiterung in einem Gruppenbeitrag aktualisiert wird. Die Erweiterung wird anfänglich durch die folgende JSON-Nutzlast mit einem `expirationDate`-Wert von `2015-07-03T13:04:00Z` dargestellt:</span><span class="sxs-lookup"><span data-stu-id="2a6fe-p109">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<span data-ttu-id="2a6fe-205">Im Folgenden werden die Anforderung und Anforderungstext zum Ändern von `expirationDate` zu `2016-07-30T11:00:00Z` dargestellt:</span><span class="sxs-lookup"><span data-stu-id="2a6fe-205">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

<!-- {
  "blockType": "request",
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate')
Content-type: application/json

{
   "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
   "extensionName": "Com.Contoso.Estimate",
   "companyName": "Contoso",
   "expirationDate": "2016-07-30T11:00:00.000Z",
   "DealValue": 1010100,
   "topPicks": [
       "Employees only",
       "Add spouse or guest",
       "Add family"
    ]
}
```

#### <a name="response-2"></a><span data-ttu-id="2a6fe-206">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="2a6fe-206">Response 2</span></span>

<span data-ttu-id="2a6fe-207">Im Folgenden wird die Antwort des zweiten Beispiels dargestellt, welche das aktualisierte `expirationDate`-Element in die Erweiterung zeigt.</span><span class="sxs-lookup"><span data-stu-id="2a6fe-207">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "response",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.opentypeextension"  
} --> 
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2016-07-30T11:00:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
} -->
