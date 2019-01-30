---
title: Datenerweiterung erstellen
description: Erstellen Sie eine open-Erweiterung (OpenTypeExtension-Objekt) und Hinzufügen von benutzerdefinierten Eigenschaften
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: a654d0bc48bc5f4f83be4adaf258fa3186914745
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642709"
---
# <a name="create-open-extension"></a><span data-ttu-id="42367-103">Datenerweiterung erstellen</span><span class="sxs-lookup"><span data-stu-id="42367-103">Create open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42367-104">Erstellen Sie eine open-Erweiterung ([OpenTypeExtension](../resources/opentypeextension.md) -Objekt) und fügen Sie benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer unterstützten Ressource hinzu.</span><span class="sxs-lookup"><span data-stu-id="42367-104">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a supported resource.</span></span>

> <span data-ttu-id="42367-105">**Hinweis:** Wenn beim Erstellen von open Extensions auf Outlook-Ressourcen finden Sie in [OpenTypeExtension Ressourcentyp](../resources/opentypeextension.md#outlook-specific-considerations) **Outlook-spezifischen Aspekte** .</span><span class="sxs-lookup"><span data-stu-id="42367-105">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="42367-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="42367-106">Permissions</span></span>

<span data-ttu-id="42367-107">Je nach der Ressource, die Sie die Erweiterung im erstellen und die Berechtigung Typ (delegierte oder-Anwendung) angefordert, die Berechtigung, die in der folgenden Tabelle angegebenen mit den geringsten ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="42367-107">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="42367-108">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42367-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42367-109">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="42367-109">Supported resource</span></span> | <span data-ttu-id="42367-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="42367-110">Delegated (work or school account)</span></span> | <span data-ttu-id="42367-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="42367-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42367-112">Application</span><span class="sxs-lookup"><span data-stu-id="42367-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="42367-113">device</span><span class="sxs-lookup"><span data-stu-id="42367-113">device</span></span>](../resources/device.md) | <span data-ttu-id="42367-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42367-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="42367-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42367-115">Not supported</span></span> | <span data-ttu-id="42367-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42367-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="42367-117">event</span><span class="sxs-lookup"><span data-stu-id="42367-117">event</span></span>](../resources/event.md) | <span data-ttu-id="42367-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42367-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="42367-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42367-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="42367-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42367-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="42367-121">group</span><span class="sxs-lookup"><span data-stu-id="42367-121">group</span></span>](../resources/group.md) | <span data-ttu-id="42367-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42367-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="42367-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42367-123">Not supported</span></span> | <span data-ttu-id="42367-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42367-124">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="42367-125">group event</span><span class="sxs-lookup"><span data-stu-id="42367-125">group event</span></span>](../resources/event.md) | <span data-ttu-id="42367-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42367-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="42367-127">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42367-127">Not supported</span></span> | <span data-ttu-id="42367-128">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42367-128">Not supported</span></span> |
| [<span data-ttu-id="42367-129">group post</span><span class="sxs-lookup"><span data-stu-id="42367-129">group post</span></span>](../resources/post.md) | <span data-ttu-id="42367-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42367-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="42367-131">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42367-131">Not supported</span></span> | <span data-ttu-id="42367-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42367-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="42367-133">message</span><span class="sxs-lookup"><span data-stu-id="42367-133">message</span></span>](../resources/message.md) | <span data-ttu-id="42367-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42367-134">Mail.ReadWrite</span></span> | <span data-ttu-id="42367-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42367-135">Mail.ReadWrite</span></span> | <span data-ttu-id="42367-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42367-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="42367-137">organization</span><span class="sxs-lookup"><span data-stu-id="42367-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="42367-138">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42367-138">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="42367-139">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42367-139">Not supported</span></span> | <span data-ttu-id="42367-140">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42367-140">Not supported</span></span> |
| [<span data-ttu-id="42367-141">personal contact</span><span class="sxs-lookup"><span data-stu-id="42367-141">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="42367-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42367-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="42367-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42367-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="42367-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42367-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="42367-145">user</span><span class="sxs-lookup"><span data-stu-id="42367-145">user</span></span>](../resources/user.md) | <span data-ttu-id="42367-146">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42367-146">User.ReadWrite.All</span></span> | <span data-ttu-id="42367-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42367-147">User.ReadWrite</span></span> | <span data-ttu-id="42367-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42367-148">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42367-149">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="42367-149">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="42367-150">Erstellen einer Erweiterung in einer neuen Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="42367-150">Create an extension in a new resource instance</span></span>

<span data-ttu-id="42367-151">Verwenden Sie die gleiche REST-Anforderung, die Sie verwenden, um die Instanz zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="42367-151">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="42367-152">**Hinweis:** Diese Syntax enthält einige allgemeinen Bereitstellungsmethoden für die Ressourceninstanzen unterstützte zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="42367-152">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="42367-153">Andere POST-Syntax, die Sie erstellen diese Ressourceninstanzen können unterstützt erstellen open Erweiterungen in diese auf ähnliche Weise.</span><span class="sxs-lookup"><span data-stu-id="42367-153">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="42367-154">Im Abschnitt [Anforderungstext](#request-body) ist beschrieben, wie Sie die Eigenschaften der neuen Ressourceninstanz _und die Erweiterung_ in den Anforderungstext einschließen können.</span><span class="sxs-lookup"><span data-stu-id="42367-154">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="42367-155">Erstellen einer Erweiterung in einer vorhandenen Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="42367-155">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="42367-156">Geben Sie die Ressourceninstanz in der Anforderung an, und wenden Sie den Befehl `POST` auf die Navigationseigenschaft **extensions** an.</span><span class="sxs-lookup"><span data-stu-id="42367-156">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /administrativeunits/{id}/extensions
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

><span data-ttu-id="42367-157">**Hinweis:** Diese Syntax enthält einige allgemeinen Bereitstellungsmethoden für eine Ressourceninstanz identifizieren, um eine Erweiterung in es zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="42367-157">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="42367-158">Alle anderen Syntax, die Ihnen ermöglicht, diese Ressourceninstanzen identifizieren unterstützt das Erstellen von open Extensions darin auf ähnliche Weise.</span><span class="sxs-lookup"><span data-stu-id="42367-158">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="42367-159">Im Abschnitt [Anforderungstext](#request-body) wird beschrieben, wie Sie _die Erweiterung_ in den Anforderungstext einschließen können.</span><span class="sxs-lookup"><span data-stu-id="42367-159">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="42367-160">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="42367-160">Path parameters</span></span>

|<span data-ttu-id="42367-161">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="42367-161">**Parameter**</span></span>|<span data-ttu-id="42367-162">**Typ**</span><span class="sxs-lookup"><span data-stu-id="42367-162">**Type**</span></span>|<span data-ttu-id="42367-163">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="42367-163">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="42367-164">id</span><span class="sxs-lookup"><span data-stu-id="42367-164">id</span></span>|<span data-ttu-id="42367-165">string</span><span class="sxs-lookup"><span data-stu-id="42367-165">string</span></span>|<span data-ttu-id="42367-p104">Ein eindeutiger Bezeichner für ein Objekt in der entsprechenden Sammlung. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="42367-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="42367-168">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="42367-168">Request headers</span></span>

| <span data-ttu-id="42367-169">Name</span><span class="sxs-lookup"><span data-stu-id="42367-169">Name</span></span>       | <span data-ttu-id="42367-170">Wert</span><span class="sxs-lookup"><span data-stu-id="42367-170">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="42367-171">Authorization</span><span class="sxs-lookup"><span data-stu-id="42367-171">Authorization</span></span> | <span data-ttu-id="42367-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="42367-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42367-174">Content-Type</span><span class="sxs-lookup"><span data-stu-id="42367-174">Content-Type</span></span> | <span data-ttu-id="42367-175">application/json</span><span class="sxs-lookup"><span data-stu-id="42367-175">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="42367-176">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="42367-176">Request body</span></span>

<span data-ttu-id="42367-177">Bieten Sie ein JSON-Hauptteil eines [OpenTypeExtension](../resources/opentypeextension.md)die folgenden erforderlichen Name / Wert-Paare und zusätzlichen benutzerdefinierten Daten.</span><span class="sxs-lookup"><span data-stu-id="42367-177">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data.</span></span> <span data-ttu-id="42367-178">Die Daten in der JSON-Nutzlast möglich Grundtypen oder Arrays von Grundtypen.</span><span class="sxs-lookup"><span data-stu-id="42367-178">The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="42367-179">Name</span><span class="sxs-lookup"><span data-stu-id="42367-179">Name</span></span>       | <span data-ttu-id="42367-180">Wert</span><span class="sxs-lookup"><span data-stu-id="42367-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="42367-181">@odata.type</span><span class="sxs-lookup"><span data-stu-id="42367-181">@odata.type</span></span> | <span data-ttu-id="42367-182">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="42367-182">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="42367-183">extensionName</span><span class="sxs-lookup"><span data-stu-id="42367-183">extensionName</span></span> | <span data-ttu-id="42367-184">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="42367-184">%unique_string%</span></span> |

<span data-ttu-id="42367-185">Beim Erstellen einer Erweiterung in einer _neuen_ Ressourceninstanz müssen Sie zusätzlich zu dem neuen **openTypeExtension**-Objekt eine JSON-Darstellung der zur Erstellung einer solchen Ressourceninstanz erforderlichen Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="42367-185">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="42367-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="42367-186">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="42367-187">Antwortcode</span><span class="sxs-lookup"><span data-stu-id="42367-187">Response code</span></span>

<span data-ttu-id="42367-188">Je nach Vorgang lautet der Antwortcode `201 Created` oder `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="42367-188">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="42367-189">Beim Erstellen einer Erweiterungs mit den gleichen Vorgang, mit denen Sie eine Ressourceninstanz zu erstellen, gibt der Vorgang den gleichen Antwortcode, den es zurückgibt, wenn Sie den Vorgang zum Erstellen der Ressourceninstanz ohne die Erweiterung verwenden.</span><span class="sxs-lookup"><span data-stu-id="42367-189">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="42367-190">Finden Sie in den entsprechenden Themen für die Instanz als aufgeführten [oben](#create-an-extension-in-a-new-resource-instance)zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="42367-190">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="42367-191">Antworttext</span><span class="sxs-lookup"><span data-stu-id="42367-191">Response body</span></span>

| <span data-ttu-id="42367-192">Szenario</span><span class="sxs-lookup"><span data-stu-id="42367-192">Scenario</span></span>       | <span data-ttu-id="42367-193">Ressource</span><span class="sxs-lookup"><span data-stu-id="42367-193">Resource</span></span>  | <span data-ttu-id="42367-194">Antworttext</span><span class="sxs-lookup"><span data-stu-id="42367-194">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="42367-195">Erstellen einer Erweiterung bei gleichzeitiger expliziter Erstellung einer _neuen_ Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="42367-195">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="42367-196">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="42367-196">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="42367-197">Enthält die neue Instanz, erweitert um das [openTypeExtension](../resources/opentypeextension.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="42367-197">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="42367-198">Erstellen einer Erweiterung bei gleichzeitiger impliziter Erstellung einer Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="42367-198">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="42367-199">post</span><span class="sxs-lookup"><span data-stu-id="42367-199">post</span></span>](../resources/post.md) | <span data-ttu-id="42367-200">Die Antwort enthält nur einen Antwortcode, keinen Antworttext.</span><span class="sxs-lookup"><span data-stu-id="42367-200">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="42367-201">Erstellen einer Erweiterung in einer _vorhandenen_ Ressourceninstanz</span><span class="sxs-lookup"><span data-stu-id="42367-201">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="42367-202">Alle unterstützten Ressourcen</span><span class="sxs-lookup"><span data-stu-id="42367-202">All supported resources</span></span> | <span data-ttu-id="42367-203">Enthält das **openTypeExtension**-Objekt.</span><span class="sxs-lookup"><span data-stu-id="42367-203">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="42367-204">Beispiel</span><span class="sxs-lookup"><span data-stu-id="42367-204">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="42367-205">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="42367-205">Request 1</span></span>

<span data-ttu-id="42367-p108">Im ersten Beispiel werden mit ein und demselben Aufruf eine Nachricht und eine Erweiterung erstellt. Der Anforderungstext enthält Folgendes:</span><span class="sxs-lookup"><span data-stu-id="42367-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="42367-208">Die für eine neue Nachricht typischen Eigenschaften **subject**, **body** und **toRecipients**</span><span class="sxs-lookup"><span data-stu-id="42367-208">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="42367-209">Daneben die folgenden Parameter der Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="42367-209">And for the extension:</span></span>

  - <span data-ttu-id="42367-210">Den Typ `Microsoft.Graph.OpenTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="42367-210">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
  - <span data-ttu-id="42367-211">Den Erweiterungsnamen „Com.Contoso.Referral“</span><span class="sxs-lookup"><span data-stu-id="42367-211">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="42367-212">Zusätzliche Daten, die als drei benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden: `companyName`, `expirationDate`, und `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="42367-212">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a><span data-ttu-id="42367-213">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="42367-213">Response 1</span></span>

<span data-ttu-id="42367-p109">Unten sehen Sie die Antwort für Beispiel 1. Der Antworttext enthält die Eigenschaften der neuen Nachricht sowie die folgenden Parameter der neuen Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="42367-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="42367-216">Die Eigenschaft **id** mit dem vollqualifizierten Namen `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`</span><span class="sxs-lookup"><span data-stu-id="42367-216">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="42367-217">Die in der Anforderung angegebene Standardeigenschaft **extensionName**</span><span class="sxs-lookup"><span data-stu-id="42367-217">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="42367-218">Die in der Anforderung angegebenen benutzerdefinierten Daten, gespeichert als 3 benutzerdefinierte Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="42367-218">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="42367-p110">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42367-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
      "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a><span data-ttu-id="42367-221">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="42367-221">Request 2</span></span>

<span data-ttu-id="42367-p111">Das zweite Beispiel erstellt eine Erweiterung in der angegebenen Nachricht. Der Anforderungstext enthält die folgenden Parameter für die Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="42367-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="42367-224">Den Typ `Microsoft.Graph.OpenTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="42367-224">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="42367-225">Den Erweiterungsnamen „Com.Contoso.Referral“</span><span class="sxs-lookup"><span data-stu-id="42367-225">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="42367-226">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `dealValue` und `expirationDate`</span><span class="sxs-lookup"><span data-stu-id="42367-226">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a><span data-ttu-id="42367-227">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="42367-227">Response 2</span></span>

<span data-ttu-id="42367-p112">Die Antwort für das zweite Beispiel sehen Sie unten. Der Antworttext enthält die folgenden Parameter für die neue Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="42367-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="42367-230">Die Standardeigenschaft **extensionName**</span><span class="sxs-lookup"><span data-stu-id="42367-230">The default property **extensionName**.</span></span>
- <span data-ttu-id="42367-231">Die Eigenschaft **id** mit dem vollqualifizierten Namen `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`</span><span class="sxs-lookup"><span data-stu-id="42367-231">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="42367-232">Die benutzerdefinierten Daten, die gespeichert werden sollen</span><span class="sxs-lookup"><span data-stu-id="42367-232">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="42367-233">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="42367-233">Request 3</span></span>

<span data-ttu-id="42367-p113">Das dritte Beispiel erstellt eine Erweiterung in dem angegebenen Gruppenereignis. Der Anforderungstext enthält die folgenden Parameter für die Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="42367-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="42367-236">Den Typ `Microsoft.Graph.OpenTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="42367-236">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="42367-237">Den Erweiterungsnamen „Com.Contoso.Deal“</span><span class="sxs-lookup"><span data-stu-id="42367-237">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="42367-238">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `dealValue` und `expirationDate`</span><span class="sxs-lookup"><span data-stu-id="42367-238">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a><span data-ttu-id="42367-239">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="42367-239">Response 3</span></span>

<span data-ttu-id="42367-240">Unten sehen Sie die Antwort auf die Anforderung im dritten Beispiel:</span><span class="sxs-lookup"><span data-stu-id="42367-240">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="42367-241">Anforderung 4</span><span class="sxs-lookup"><span data-stu-id="42367-241">Request 4</span></span>

<span data-ttu-id="42367-p114">Das vierte Beispiel erstellt eine Erweiterung in einem neuen Gruppenbeitrag, mit demselben **reply**-Aktionsaufruf, wie er für bereits vorhandene Gruppenbeiträge verwendet wird. Die Aktion **reply** erstellt einen neuen Beitrag und eine neue, in diesen Beitrag eingebettete Erweiterung. Der Antworttext enthält eine Eigenschaft **post** mit dem **Text** des neuen Beitrags sowie die folgenden Daten der neuen Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="42367-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="42367-245">Den Typ `Microsoft.Graph.OpenTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="42367-245">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="42367-246">Den Erweiterungsnamen „Com.Contoso.HR“</span><span class="sxs-lookup"><span data-stu-id="42367-246">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="42367-247">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `expirationDate` und das Zeichenfolgen-Array `topPicks`</span><span class="sxs-lookup"><span data-stu-id="42367-247">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/reply

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]
  }
}
```

### <a name="response-4"></a><span data-ttu-id="42367-248">Antwort 4</span><span class="sxs-lookup"><span data-stu-id="42367-248">Response 4</span></span>

<span data-ttu-id="42367-p115">Die Antwort für das vierte Beispiel sehen Sie unten. Wird eine Erweiterung in einem neuen Gruppenbeitrag erstellt, wird nur der Antwortcode „HTTP 202“ zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42367-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```

****

### <a name="request-5"></a><span data-ttu-id="42367-251">Anforderung 5</span><span class="sxs-lookup"><span data-stu-id="42367-251">Request 5</span></span>

<span data-ttu-id="42367-p116">Das fünfte Beispiel erstellt in ein und derselben POST-Operation eine Erweiterung in einem neuen Gruppenbeitrag und eine Unterhaltung. Die POST-Operation erstellt eine neue Unterhaltung, einen neuen Thread, einen neuen Beitrag und eine neue, in diesen Beitrag eingebettete Erweiterung. Der Anforderungstext enthält die Eigenschaften **Topic** und **Threads** sowie ein untergeordnetes Objekt des Typs **post** der neuen Unterhaltung. Das **post**-Objekt wiederum enthält den **Text** des neuen Beitrags sowie die folgenden Daten der Erweiterung:</span><span class="sxs-lookup"><span data-stu-id="42367-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="42367-256">Den Typ `Microsoft.Graph.OpenTypeExtension`</span><span class="sxs-lookup"><span data-stu-id="42367-256">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="42367-257">Den Erweiterungsnamen „Com.Contoso.HR“</span><span class="sxs-lookup"><span data-stu-id="42367-257">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="42367-258">Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `expirationDate` und das Zeichenfolgen-Array `topPicks`</span><span class="sxs-lookup"><span data-stu-id="42367-258">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]
            }
          ]
        }
      ]
    }
  ]
}
```

### <a name="response-5"></a><span data-ttu-id="42367-259">Antwort 5</span><span class="sxs-lookup"><span data-stu-id="42367-259">Response 5</span></span>

<span data-ttu-id="42367-p117">Unten sehen Sie die Antwort für das fünfte Beispiel mit der neuen Unterhaltung und einer Thread-ID. Dieser neue Thread enthält einen automatisch erstellten Beitrag, der wiederum die neue Erweiterung enthält.</span><span class="sxs-lookup"><span data-stu-id="42367-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="42367-p118">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42367-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="42367-p119">Zum Abrufen der neuen Erweiterung [rufen Sie zunächst alle Beiträge](../api/conversationthread-list-posts.md) in diesem Thread ab. Anfangs sollte es nur einen Beitrag geben. Wenden Sie dann die Beitrags-ID und den Erweiterungsnamen `Com.Contoso.Benefits` an, um [die Erweiterung abzurufen](../api/opentypeextension-get.md).</span><span class="sxs-lookup"><span data-stu-id="42367-p119">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/opentypeextension-post-opentypeextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
