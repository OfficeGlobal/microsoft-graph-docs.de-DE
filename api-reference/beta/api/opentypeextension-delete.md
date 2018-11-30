---
title: Offene Erweiterung löschen
description: 'Mit dieser API können Sie offene Erweiterungen (Objekte des Typs openTypeExtension aus der jeweils angegebenen Ressourceninstanz löschen. '
ms.openlocfilehash: 852573241e65e1a68ecbb308a67f79ee4ec14ab8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060025"
---
# <a name="delete-open-extension"></a><span data-ttu-id="dd736-103">Offene Erweiterung löschen</span><span class="sxs-lookup"><span data-stu-id="dd736-103">Delete open extension</span></span>

> <span data-ttu-id="dd736-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd736-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd736-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd736-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd736-106">Mit dieser API können Sie offene Erweiterungen (Objekte des Typs [openTypeExtension](../resources/opentypeextension.md) aus der jeweils angegebenen Ressourceninstanz löschen.</span><span class="sxs-lookup"><span data-stu-id="dd736-106">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="dd736-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dd736-107">Permissions</span></span>

<span data-ttu-id="dd736-108">Je nach der Ressource, die Sie die Erweiterung von löschen möchten, und die Berechtigung Typ (delegierte oder-Anwendung) angefordert, die Berechtigung, die in der folgenden Tabelle angegebenen mit den geringsten ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="dd736-108">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="dd736-109">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd736-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd736-110">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="dd736-110">Supported resource</span></span> | <span data-ttu-id="dd736-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd736-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd736-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd736-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd736-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd736-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="dd736-114">Gerät</span><span class="sxs-lookup"><span data-stu-id="dd736-114">device</span></span>](../resources/device.md) | <span data-ttu-id="dd736-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd736-115">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="dd736-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd736-116">Not supported</span></span> | <span data-ttu-id="dd736-117">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd736-117">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="dd736-118">event</span><span class="sxs-lookup"><span data-stu-id="dd736-118">event</span></span>](../resources/event.md) | <span data-ttu-id="dd736-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd736-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="dd736-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd736-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="dd736-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd736-121">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="dd736-122">group</span><span class="sxs-lookup"><span data-stu-id="dd736-122">group</span></span>](../resources/group.md) | <span data-ttu-id="dd736-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd736-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="dd736-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd736-124">Not supported</span></span> | <span data-ttu-id="dd736-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd736-125">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="dd736-126">group event</span><span class="sxs-lookup"><span data-stu-id="dd736-126">group event</span></span>](../resources/event.md) | <span data-ttu-id="dd736-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd736-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="dd736-128">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd736-128">Not supported</span></span> | <span data-ttu-id="dd736-129">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd736-129">Not supported</span></span> |
| [<span data-ttu-id="dd736-130">group post</span><span class="sxs-lookup"><span data-stu-id="dd736-130">group post</span></span>](../resources/post.md) | <span data-ttu-id="dd736-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd736-131">Group.ReadWrite.All</span></span> | <span data-ttu-id="dd736-132">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd736-132">Not supported</span></span> | <span data-ttu-id="dd736-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd736-133">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="dd736-134">message</span><span class="sxs-lookup"><span data-stu-id="dd736-134">message</span></span>](../resources/message.md) | <span data-ttu-id="dd736-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd736-135">Mail.ReadWrite</span></span> | <span data-ttu-id="dd736-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd736-136">Mail.ReadWrite</span></span> | <span data-ttu-id="dd736-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd736-137">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="dd736-138">organization</span><span class="sxs-lookup"><span data-stu-id="dd736-138">organization</span></span>](../resources/organization.md) | <span data-ttu-id="dd736-139">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd736-139">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="dd736-140">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd736-140">Not supported</span></span> | <span data-ttu-id="dd736-141">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd736-141">Not supported</span></span> |
| [<span data-ttu-id="dd736-142">personal contact</span><span class="sxs-lookup"><span data-stu-id="dd736-142">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="dd736-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd736-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="dd736-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd736-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="dd736-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd736-145">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="dd736-146">user</span><span class="sxs-lookup"><span data-stu-id="dd736-146">user</span></span>](../resources/user.md) | <span data-ttu-id="dd736-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd736-147">User.ReadWrite.All</span></span> | <span data-ttu-id="dd736-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd736-148">User.ReadWrite</span></span> | <span data-ttu-id="dd736-149">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd736-149">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd736-150">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd736-150">HTTP request</span></span>

<span data-ttu-id="dd736-151">In der Anforderung geben Sie die Ressourceninstanz an, spezifizieren in der Navigationseigenschaft **extensions** dieser Instanz die Erweiterung und wenden anschließend den Befehl `DELETE` auf diese Erweiterungsinstanz an.</span><span class="sxs-lookup"><span data-stu-id="dd736-151">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{Id}/extensions/{extensionId}
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

><span data-ttu-id="dd736-p103">**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Identifizieren einer Ressourceninstanz, um eine Erweiterung daraus zu löschen. Alle anderen Syntaxen, mit denen Sie diese Ressourceninstanzen identifizieren können, unterstützen das Löschen offener Erweiterungen daraus in einer ähnlichen Weise.</span><span class="sxs-lookup"><span data-stu-id="dd736-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="dd736-154">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="dd736-154">Path parameters</span></span>
|<span data-ttu-id="dd736-155">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="dd736-155">**Parameter**</span></span>|<span data-ttu-id="dd736-156">**Typ**</span><span class="sxs-lookup"><span data-stu-id="dd736-156">**Type**</span></span>|<span data-ttu-id="dd736-157">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="dd736-157">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dd736-158">id</span><span class="sxs-lookup"><span data-stu-id="dd736-158">id</span></span>|<span data-ttu-id="dd736-159">string</span><span class="sxs-lookup"><span data-stu-id="dd736-159">string</span></span>|<span data-ttu-id="dd736-p104">Ein eindeutiger Bezeichner für eine Instanz in der entsprechenden Sammlung. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dd736-p104">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="dd736-162">extensionId</span><span class="sxs-lookup"><span data-stu-id="dd736-162">extensionId</span></span>|<span data-ttu-id="dd736-163">string</span><span class="sxs-lookup"><span data-stu-id="dd736-163">string</span></span>|<span data-ttu-id="dd736-p105">Dies kann ein Erweiterungsname sein. Der Erweiterungsname ist ein eindeutiger Textbezeichner der Erweiterung oder ein vollqualifizierter Name, der den Erweiterungstyp und den eindeutigen Textbezeichner verkettet. Der vollqualifizierte Name wird beim Erstellen der Erweiterung in der `id`-Eigenschaft zurückgegeben. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dd736-p105">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="dd736-167">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd736-167">Request headers</span></span>
| <span data-ttu-id="dd736-168">Name</span><span class="sxs-lookup"><span data-stu-id="dd736-168">Name</span></span>       | <span data-ttu-id="dd736-169">Wert</span><span class="sxs-lookup"><span data-stu-id="dd736-169">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="dd736-170">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd736-170">Authorization</span></span> | <span data-ttu-id="dd736-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dd736-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd736-173">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd736-173">Request body</span></span>
<span data-ttu-id="dd736-174">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dd736-174">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd736-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd736-175">Response</span></span>

<span data-ttu-id="dd736-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd736-p107">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd736-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd736-178">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd736-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd736-179">Request</span></span>
<span data-ttu-id="dd736-180">Das erste Beispiel referenziert eine Erweiterung über ihren Namen und löscht die Erweiterung in der angegebenen Nachricht.</span><span class="sxs-lookup"><span data-stu-id="dd736-180">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="dd736-181">Das zweite Beispiel löscht eine Erweiterung in dem angegebenen Gruppenereignis.</span><span class="sxs-lookup"><span data-stu-id="dd736-181">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a><span data-ttu-id="dd736-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd736-182">Response</span></span>
<span data-ttu-id="dd736-183">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dd736-183">Here is an example of the response.</span></span>
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