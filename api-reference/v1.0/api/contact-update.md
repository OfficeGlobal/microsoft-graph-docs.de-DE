---
title: Kontakt aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Kontaktobjekts aktualisieren.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 381aa191639e32677d4fccbf9e9f48c99f3d988f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927905"
---
# <a name="update-contact"></a><span data-ttu-id="7304e-103">Kontakt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7304e-103">Update contact</span></span>

<span data-ttu-id="7304e-104">Mit dieser API können Sie die Eigenschaften eines Kontaktobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="7304e-104">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7304e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7304e-105">Permissions</span></span>
<span data-ttu-id="7304e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7304e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7304e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7304e-108">Permission type</span></span>      | <span data-ttu-id="7304e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7304e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7304e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7304e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7304e-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7304e-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7304e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7304e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7304e-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7304e-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7304e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7304e-114">Application</span></span> | <span data-ttu-id="7304e-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7304e-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7304e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7304e-116">HTTP request</span></span>
<span data-ttu-id="7304e-117"><!-- { "blockType": "ignored" } -->[Wenden Sie sich](../resources/contact.md) von einem Benutzer standardmäßig [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="7304e-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="7304e-118">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="7304e-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="7304e-p102">Ein [Kontakt](../resources/contact.md) in einem untergeordneten Ordner eines [contactFolder](../resources/mailfolder.md). Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="7304e-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7304e-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7304e-121">Request headers</span></span>
| <span data-ttu-id="7304e-122">Header</span><span class="sxs-lookup"><span data-stu-id="7304e-122">Header</span></span>       | <span data-ttu-id="7304e-123">Wert</span><span class="sxs-lookup"><span data-stu-id="7304e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7304e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7304e-124">Authorization</span></span>  | <span data-ttu-id="7304e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7304e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7304e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7304e-127">Content-Type</span></span>  | <span data-ttu-id="7304e-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="7304e-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7304e-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7304e-130">Request body</span></span>
<span data-ttu-id="7304e-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="7304e-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7304e-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7304e-134">Property</span></span>     | <span data-ttu-id="7304e-135">Typ</span><span class="sxs-lookup"><span data-stu-id="7304e-135">Type</span></span>   |<span data-ttu-id="7304e-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7304e-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7304e-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="7304e-137">assistantName</span></span>|<span data-ttu-id="7304e-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-138">String</span></span>|<span data-ttu-id="7304e-139">Der Name des Assistenten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="7304e-140">birthday</span><span class="sxs-lookup"><span data-stu-id="7304e-140">birthday</span></span>|<span data-ttu-id="7304e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7304e-141">DateTimeOffset</span></span>|<span data-ttu-id="7304e-142">Das Geburtsdatum des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-142">The contact's birthday.</span></span>|
|<span data-ttu-id="7304e-143">businessAddress</span><span class="sxs-lookup"><span data-stu-id="7304e-143">businessAddress</span></span>|[<span data-ttu-id="7304e-144">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="7304e-144">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="7304e-145">Die Geschäftsadresse des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-145">The contact's business address.</span></span>|
|<span data-ttu-id="7304e-146">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="7304e-146">businessHomePage</span></span>|<span data-ttu-id="7304e-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-147">String</span></span>|<span data-ttu-id="7304e-148">Die geschäftliche Homepage des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-148">The business home page of the contact.</span></span>|
|<span data-ttu-id="7304e-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="7304e-149">businessPhones</span></span>|<span data-ttu-id="7304e-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-150">String</span></span>|<span data-ttu-id="7304e-151">Die geschäftlichen Telefonnummern des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-151">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="7304e-152">categories</span><span class="sxs-lookup"><span data-stu-id="7304e-152">categories</span></span>|<span data-ttu-id="7304e-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-153">String</span></span>|<span data-ttu-id="7304e-154">Die Kategorien, die mit dem Kontakt verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="7304e-154">The categories associated with the contact.</span></span>|
|<span data-ttu-id="7304e-155">children</span><span class="sxs-lookup"><span data-stu-id="7304e-155">children</span></span>|<span data-ttu-id="7304e-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-156">String</span></span>|<span data-ttu-id="7304e-157">Die Namen der Kinder des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-157">The names of the contact's children.</span></span>|
|<span data-ttu-id="7304e-158">companyName</span><span class="sxs-lookup"><span data-stu-id="7304e-158">companyName</span></span>|<span data-ttu-id="7304e-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-159">String</span></span>|<span data-ttu-id="7304e-160">Der Name des Unternehmens des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-160">The name of the contact's company.</span></span>|
|<span data-ttu-id="7304e-161">department</span><span class="sxs-lookup"><span data-stu-id="7304e-161">department</span></span>|<span data-ttu-id="7304e-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-162">String</span></span>|<span data-ttu-id="7304e-163">Die Abteilung des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-163">The contact's department.</span></span>|
|<span data-ttu-id="7304e-164">displayName</span><span class="sxs-lookup"><span data-stu-id="7304e-164">displayName</span></span>|<span data-ttu-id="7304e-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-165">String</span></span>|<span data-ttu-id="7304e-166">Der Anzeigename des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-166">The contact's display name.</span></span> <span data-ttu-id="7304e-167">Beachten Sie, dass es sich bei spätere Aktualisierungen mit anderen Eigenschaften verursachen einen automatisch generierten Wert den Wert DisplayName überschrieben, den Sie angegeben haben.</span><span class="sxs-lookup"><span data-stu-id="7304e-167">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="7304e-168">Um einen bereits vorhandenen Wert zu erhalten, immer als schließen Sie DisplayName in einem Aktualisierungsvorgang ein.</span><span class="sxs-lookup"><span data-stu-id="7304e-168">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="7304e-169">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="7304e-169">emailAddresses</span></span>|<span data-ttu-id="7304e-170">[EmailAddress](../resources/emailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="7304e-170">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="7304e-171">Die E-Mail-Adressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-171">The contact's email addresses.</span></span>|
|<span data-ttu-id="7304e-172">fileAs</span><span class="sxs-lookup"><span data-stu-id="7304e-172">fileAs</span></span>|<span data-ttu-id="7304e-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-173">String</span></span>|<span data-ttu-id="7304e-174">Der Name, unter dem der Kontakt abgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="7304e-174">The name the contact is filed under.</span></span>|
|<span data-ttu-id="7304e-175">generation</span><span class="sxs-lookup"><span data-stu-id="7304e-175">generation</span></span>|<span data-ttu-id="7304e-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-176">String</span></span>|<span data-ttu-id="7304e-177">Die Generation des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-177">The contact's generation.</span></span>|
|<span data-ttu-id="7304e-178">givenName</span><span class="sxs-lookup"><span data-stu-id="7304e-178">givenName</span></span>|<span data-ttu-id="7304e-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-179">String</span></span>|<span data-ttu-id="7304e-180">Der Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-180">The contact's given name.</span></span>|
|<span data-ttu-id="7304e-181">homeAddress</span><span class="sxs-lookup"><span data-stu-id="7304e-181">homeAddress</span></span>|[<span data-ttu-id="7304e-182">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="7304e-182">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="7304e-183">Die Privatadresse des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-183">The contact's home address.</span></span>|
|<span data-ttu-id="7304e-184">homePhones</span><span class="sxs-lookup"><span data-stu-id="7304e-184">homePhones</span></span>|<span data-ttu-id="7304e-185">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="7304e-185">String collection</span></span>|<span data-ttu-id="7304e-186">Die privaten Telefonnummern des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-186">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="7304e-187">imAddresses</span><span class="sxs-lookup"><span data-stu-id="7304e-187">imAddresses</span></span>|<span data-ttu-id="7304e-188">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-188">String</span></span>|<span data-ttu-id="7304e-189">Instant Messaging Chatadressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-189">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="7304e-190">initials</span><span class="sxs-lookup"><span data-stu-id="7304e-190">initials</span></span>|<span data-ttu-id="7304e-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-191">String</span></span>|<span data-ttu-id="7304e-192">Die Initialen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-192">The contact's initials.</span></span>|
|<span data-ttu-id="7304e-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="7304e-193">jobTitle</span></span>|<span data-ttu-id="7304e-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-194">String</span></span>|<span data-ttu-id="7304e-195">Die Position des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-195">The contact’s job title.</span></span>|
|<span data-ttu-id="7304e-196">manager</span><span class="sxs-lookup"><span data-stu-id="7304e-196">manager</span></span>|<span data-ttu-id="7304e-197">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-197">String</span></span>|<span data-ttu-id="7304e-198">Der Name des Vorgesetzten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-198">The name of the contact's manager.</span></span>
|<span data-ttu-id="7304e-199">middleName</span><span class="sxs-lookup"><span data-stu-id="7304e-199">middleName</span></span>|<span data-ttu-id="7304e-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-200">String</span></span>|<span data-ttu-id="7304e-201">Der zweite Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-201">The contact's middle name.</span></span>|
|<span data-ttu-id="7304e-202">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="7304e-202">mobilePhone</span></span>|<span data-ttu-id="7304e-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-203">String</span></span>|<span data-ttu-id="7304e-204">Die Mobiltelefonnummer des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-204">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="7304e-205">nickName</span><span class="sxs-lookup"><span data-stu-id="7304e-205">nickName</span></span>|<span data-ttu-id="7304e-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-206">String</span></span>|<span data-ttu-id="7304e-207">Der Spitzname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-207">The contact's nickname.</span></span>|
|<span data-ttu-id="7304e-208">officeLocation</span><span class="sxs-lookup"><span data-stu-id="7304e-208">officeLocation</span></span>|<span data-ttu-id="7304e-209">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-209">String</span></span>|<span data-ttu-id="7304e-210">Der Bürostandort des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-210">The location of the contact's office.</span></span>|
|<span data-ttu-id="7304e-211">otherAddress</span><span class="sxs-lookup"><span data-stu-id="7304e-211">otherAddress</span></span>|[<span data-ttu-id="7304e-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="7304e-212">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="7304e-213">Weitere Adressen für den Kontakt.</span><span class="sxs-lookup"><span data-stu-id="7304e-213">Other addresses for the contact.</span></span>|
|<span data-ttu-id="7304e-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="7304e-214">parentFolderId</span></span>|<span data-ttu-id="7304e-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-215">String</span></span>|<span data-ttu-id="7304e-216">Die ID des übergeordneten Ordners des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-216">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="7304e-217">personalNotes</span><span class="sxs-lookup"><span data-stu-id="7304e-217">personalNotes</span></span>|<span data-ttu-id="7304e-218">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-218">String</span></span>|<span data-ttu-id="7304e-219">Die Notizen des Benutzers zu dem Kontakt.</span><span class="sxs-lookup"><span data-stu-id="7304e-219">The user's notes about the contact.</span></span>|
|<span data-ttu-id="7304e-220">profession</span><span class="sxs-lookup"><span data-stu-id="7304e-220">profession</span></span>|<span data-ttu-id="7304e-221">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-221">String</span></span>|<span data-ttu-id="7304e-222">Der Beruf des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-222">The contact's profession.</span></span>|
|<span data-ttu-id="7304e-223">spouseName</span><span class="sxs-lookup"><span data-stu-id="7304e-223">spouseName</span></span>|<span data-ttu-id="7304e-224">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-224">String</span></span>|<span data-ttu-id="7304e-225">Der Name des Ehepartners/Partners des Kontakts</span><span class="sxs-lookup"><span data-stu-id="7304e-225">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="7304e-226">surname</span><span class="sxs-lookup"><span data-stu-id="7304e-226">surname</span></span>|<span data-ttu-id="7304e-227">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-227">String</span></span>|<span data-ttu-id="7304e-228">Der Nachname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-228">The contact's surname.</span></span>|
|<span data-ttu-id="7304e-229">title</span><span class="sxs-lookup"><span data-stu-id="7304e-229">title</span></span>|<span data-ttu-id="7304e-230">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-230">String</span></span>|<span data-ttu-id="7304e-231">Der Titel des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="7304e-231">The contact's title.</span></span>|
|<span data-ttu-id="7304e-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="7304e-232">yomiCompanyName</span></span>|<span data-ttu-id="7304e-233">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-233">String</span></span>|<span data-ttu-id="7304e-p107">Der phonetische japanische Firmenname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="7304e-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="7304e-236">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="7304e-236">yomiGivenName</span></span>|<span data-ttu-id="7304e-237">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-237">String</span></span>|<span data-ttu-id="7304e-p108">Der phonetische japanische Vorname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="7304e-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="7304e-240">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="7304e-240">yomiSurname</span></span>|<span data-ttu-id="7304e-241">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7304e-241">String</span></span>|<span data-ttu-id="7304e-p109">Der phonetische japanische Nachname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="7304e-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="7304e-244">Antwort</span><span class="sxs-lookup"><span data-stu-id="7304e-244">Response</span></span>

<span data-ttu-id="7304e-245">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7304e-245">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7304e-246">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7304e-246">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7304e-247">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7304e-247">Request</span></span>
<span data-ttu-id="7304e-248">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7304e-248">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contacts/{id}
Content-type: application/json
Content-length: 1977

{
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "birthday": "1974-07-22"
}
```
##### <a name="response"></a><span data-ttu-id="7304e-249">Antwort</span><span class="sxs-lookup"><span data-stu-id="7304e-249">Response</span></span>
<span data-ttu-id="7304e-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7304e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "https://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
