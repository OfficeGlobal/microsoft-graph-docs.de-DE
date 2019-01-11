---
title: Offene Erweiterung löschen
description: 'Mit dieser API können Sie offene Erweiterungen (Objekte des Typs openTypeExtension aus der jeweils angegebenen Ressourceninstanz löschen. '
localization_priority: Normal
ms.openlocfilehash: c51870b7e302971d27a894f0e724d0dec6fe5cf1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894460"
---
# <a name="delete-open-extension"></a><span data-ttu-id="8a4b3-103">Offene Erweiterung löschen</span><span class="sxs-lookup"><span data-stu-id="8a4b3-103">Delete open extension</span></span>

<span data-ttu-id="8a4b3-104">Mit dieser API können Sie offene Erweiterungen (Objekte des Typs [openTypeExtension](../resources/opentypeextension.md) aus der jeweils angegebenen Ressourceninstanz löschen.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-104">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8a4b3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8a4b3-105">Permissions</span></span>

<span data-ttu-id="8a4b3-106">Je nach der Ressource, die Sie die Erweiterung von löschen möchten, und die Berechtigung Typ (delegierte oder-Anwendung) angefordert, die Berechtigung, die in der folgenden Tabelle angegebenen mit den geringsten ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-106">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="8a4b3-107">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a4b3-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a4b3-108">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="8a4b3-108">Supported resource</span></span> | <span data-ttu-id="8a4b3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a4b3-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8a4b3-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a4b3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a4b3-111">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a4b3-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="8a4b3-112">Gerät</span><span class="sxs-lookup"><span data-stu-id="8a4b3-112">device</span></span>](../resources/device.md) | <span data-ttu-id="8a4b3-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a4b3-113">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="8a4b3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a4b3-114">Not supported</span></span> | <span data-ttu-id="8a4b3-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4b3-115">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="8a4b3-116">event</span><span class="sxs-lookup"><span data-stu-id="8a4b3-116">event</span></span>](../resources/event.md) | <span data-ttu-id="8a4b3-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4b3-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="8a4b3-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4b3-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="8a4b3-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4b3-119">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="8a4b3-120">group</span><span class="sxs-lookup"><span data-stu-id="8a4b3-120">group</span></span>](../resources/group.md) | <span data-ttu-id="8a4b3-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4b3-121">Group.ReadWrite.All</span></span> | <span data-ttu-id="8a4b3-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a4b3-122">Not supported</span></span> | <span data-ttu-id="8a4b3-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4b3-123">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="8a4b3-124">group event</span><span class="sxs-lookup"><span data-stu-id="8a4b3-124">group event</span></span>](../resources/event.md) | <span data-ttu-id="8a4b3-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4b3-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="8a4b3-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a4b3-126">Not supported</span></span> | <span data-ttu-id="8a4b3-127">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a4b3-127">Not supported</span></span> |
| [<span data-ttu-id="8a4b3-128">group post</span><span class="sxs-lookup"><span data-stu-id="8a4b3-128">group post</span></span>](../resources/post.md) | <span data-ttu-id="8a4b3-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4b3-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="8a4b3-130">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a4b3-130">Not supported</span></span> | <span data-ttu-id="8a4b3-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4b3-131">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="8a4b3-132">message</span><span class="sxs-lookup"><span data-stu-id="8a4b3-132">message</span></span>](../resources/message.md) | <span data-ttu-id="8a4b3-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4b3-133">Mail.ReadWrite</span></span> | <span data-ttu-id="8a4b3-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4b3-134">Mail.ReadWrite</span></span> | <span data-ttu-id="8a4b3-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4b3-135">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="8a4b3-136">organization</span><span class="sxs-lookup"><span data-stu-id="8a4b3-136">organization</span></span>](../resources/organization.md) | <span data-ttu-id="8a4b3-137">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a4b3-137">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="8a4b3-138">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a4b3-138">Not supported</span></span> | <span data-ttu-id="8a4b3-139">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a4b3-139">Not supported</span></span> |
| [<span data-ttu-id="8a4b3-140">personal contact</span><span class="sxs-lookup"><span data-stu-id="8a4b3-140">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="8a4b3-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4b3-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="8a4b3-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4b3-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="8a4b3-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4b3-143">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="8a4b3-144">user</span><span class="sxs-lookup"><span data-stu-id="8a4b3-144">user</span></span>](../resources/user.md) | <span data-ttu-id="8a4b3-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4b3-145">User.ReadWrite.All</span></span> | <span data-ttu-id="8a4b3-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4b3-146">User.ReadWrite</span></span> | <span data-ttu-id="8a4b3-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4b3-147">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a4b3-148">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a4b3-148">HTTP request</span></span>
<span data-ttu-id="8a4b3-149">In der Anforderung geben Sie die Ressourceninstanz an, spezifizieren in der Navigationseigenschaft **extensions** dieser Instanz die Erweiterung und wenden anschließend den Befehl `DELETE` auf diese Erweiterungsinstanz an.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-149">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="8a4b3-p102">**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Identifizieren einer Ressourceninstanz, um eine Erweiterung daraus zu löschen. Alle anderen Syntaxen, mit denen Sie diese Ressourceninstanzen identifizieren können, unterstützen das Löschen offener Erweiterungen daraus in einer ähnlichen Weise.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="8a4b3-152">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="8a4b3-152">Path parameters</span></span>
|<span data-ttu-id="8a4b3-153">Parameter</span><span class="sxs-lookup"><span data-stu-id="8a4b3-153">Parameter</span></span>|<span data-ttu-id="8a4b3-154">Typ</span><span class="sxs-lookup"><span data-stu-id="8a4b3-154">Type</span></span>|<span data-ttu-id="8a4b3-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a4b3-155">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8a4b3-156">id</span><span class="sxs-lookup"><span data-stu-id="8a4b3-156">id</span></span>|<span data-ttu-id="8a4b3-157">string</span><span class="sxs-lookup"><span data-stu-id="8a4b3-157">string</span></span>|<span data-ttu-id="8a4b3-p103">Ein eindeutiger Bezeichner für eine Instanz in der entsprechenden Sammlung. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="8a4b3-160">extensionId</span><span class="sxs-lookup"><span data-stu-id="8a4b3-160">extensionId</span></span>|<span data-ttu-id="8a4b3-161">string</span><span class="sxs-lookup"><span data-stu-id="8a4b3-161">string</span></span>|<span data-ttu-id="8a4b3-p104">Dies kann ein Erweiterungsname sein. Der Erweiterungsname ist ein eindeutiger Textbezeichner der Erweiterung oder ein vollqualifizierter Name, der den Erweiterungstyp und den eindeutigen Textbezeichner verkettet. Der vollqualifizierte Name wird beim Erstellen der Erweiterung in der `id`-Eigenschaft zurückgegeben. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="8a4b3-165">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a4b3-165">Request headers</span></span>
| <span data-ttu-id="8a4b3-166">Name</span><span class="sxs-lookup"><span data-stu-id="8a4b3-166">Name</span></span>       | <span data-ttu-id="8a4b3-167">Wert</span><span class="sxs-lookup"><span data-stu-id="8a4b3-167">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="8a4b3-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a4b3-168">Authorization</span></span> | <span data-ttu-id="8a4b3-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a4b3-171">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8a4b3-171">Request body</span></span>
<span data-ttu-id="8a4b3-172">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-172">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a4b3-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a4b3-173">Response</span></span>

<span data-ttu-id="8a4b3-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a4b3-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a4b3-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a4b3-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a4b3-177">Request</span></span>
<span data-ttu-id="8a4b3-178">Das erste Beispiel referenziert eine Erweiterung über ihren Namen und löscht die Erweiterung in der angegebenen Nachricht.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-178">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="8a4b3-179">Das zweite Beispiel löscht eine Erweiterung in dem angegebenen Gruppenereignis.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-179">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="8a4b3-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a4b3-180">Response</span></span>
<span data-ttu-id="8a4b3-181">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8a4b3-181">Here is an example of the response.</span></span>
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
