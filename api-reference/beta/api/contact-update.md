---
title: Kontakt aktualisieren
description: Aktualisieren Sie die Eigenschaften des Kontaktobjekts an.
ms.openlocfilehash: 2fbf597ebc8a6c65141c64ae42ae42266f14cbde
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060638"
---
# <a name="update-contact"></a><span data-ttu-id="40cb0-103">Kontakt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="40cb0-103">Update contact</span></span>

> <span data-ttu-id="40cb0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="40cb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40cb0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40cb0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40cb0-106">Aktualisieren Sie die Eigenschaften des Kontaktobjekts an.</span><span class="sxs-lookup"><span data-stu-id="40cb0-106">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="40cb0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="40cb0-107">Permissions</span></span>
<span data-ttu-id="40cb0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40cb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40cb0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40cb0-110">Permission type</span></span>      | <span data-ttu-id="40cb0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40cb0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40cb0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40cb0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40cb0-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40cb0-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="40cb0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40cb0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40cb0-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40cb0-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="40cb0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40cb0-116">Application</span></span> | <span data-ttu-id="40cb0-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40cb0-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="40cb0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40cb0-118">HTTP request</span></span>
<span data-ttu-id="40cb0-119"><!-- { "blockType": "ignored" } -->[Wenden Sie sich an](../resources/contact.md) von des Benutzers Standard [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="40cb0-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="40cb0-120">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="40cb0-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="40cb0-121">[Wenden Sie sich an](../resources/contact.md) , die in einem untergeordneten Ordner von einem [ContactFolder](../resources/mailfolder.md)enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="40cb0-121">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="40cb0-122">Das folgende Beispiel zeigt eine Ebene von schachteln, aber ein Kontakt kann befindet sich ein untergeordnetes Element des ein untergeordnetes Element und so weiter.</span><span class="sxs-lookup"><span data-stu-id="40cb0-122">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="40cb0-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40cb0-123">Request headers</span></span>
| <span data-ttu-id="40cb0-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="40cb0-124">Header</span></span>       | <span data-ttu-id="40cb0-125">Wert</span><span class="sxs-lookup"><span data-stu-id="40cb0-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40cb0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="40cb0-126">Authorization</span></span>  | <span data-ttu-id="40cb0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="40cb0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="40cb0-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40cb0-129">Content-Type</span></span>  | <span data-ttu-id="40cb0-p105">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="40cb0-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40cb0-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40cb0-132">Request body</span></span>
<span data-ttu-id="40cb0-p106">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="40cb0-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="40cb0-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40cb0-136">Property</span></span>     | <span data-ttu-id="40cb0-137">Typ</span><span class="sxs-lookup"><span data-stu-id="40cb0-137">Type</span></span>   |<span data-ttu-id="40cb0-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40cb0-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40cb0-139">assistantName</span><span class="sxs-lookup"><span data-stu-id="40cb0-139">assistantName</span></span>|<span data-ttu-id="40cb0-140">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-140">String</span></span>|<span data-ttu-id="40cb0-141">Der Name des Assistenten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-141">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="40cb0-142">birthday</span><span class="sxs-lookup"><span data-stu-id="40cb0-142">birthday</span></span>|<span data-ttu-id="40cb0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40cb0-143">DateTimeOffset</span></span>|<span data-ttu-id="40cb0-144">Das Geburtsdatum des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-144">The contact's birthday.</span></span>|
|<span data-ttu-id="40cb0-145">categories</span><span class="sxs-lookup"><span data-stu-id="40cb0-145">categories</span></span>|<span data-ttu-id="40cb0-146">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-146">String</span></span>|<span data-ttu-id="40cb0-147">Die Kategorien, die mit dem Kontakt verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="40cb0-147">The categories associated with the contact.</span></span>|
|<span data-ttu-id="40cb0-148">children</span><span class="sxs-lookup"><span data-stu-id="40cb0-148">children</span></span>|<span data-ttu-id="40cb0-149">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-149">String</span></span>||
|<span data-ttu-id="40cb0-150">companyName</span><span class="sxs-lookup"><span data-stu-id="40cb0-150">companyName</span></span>|<span data-ttu-id="40cb0-151">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-151">String</span></span>|<span data-ttu-id="40cb0-152">Der Name des Unternehmens des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-152">The name of the contact's company.</span></span>|
|<span data-ttu-id="40cb0-153">department</span><span class="sxs-lookup"><span data-stu-id="40cb0-153">department</span></span>|<span data-ttu-id="40cb0-154">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-154">String</span></span>|<span data-ttu-id="40cb0-155">Die Abteilung des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-155">The contact's department.</span></span>|
|<span data-ttu-id="40cb0-156">displayName</span><span class="sxs-lookup"><span data-stu-id="40cb0-156">displayName</span></span>|<span data-ttu-id="40cb0-157">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-157">String</span></span>|<span data-ttu-id="40cb0-158">Der Anzeigename des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-158">The contact's display name.</span></span> <span data-ttu-id="40cb0-159">Beachten Sie, dass es sich bei spätere Aktualisierungen mit anderen Eigenschaften verursachen einen automatisch generierten Wert den Wert DisplayName überschrieben, den Sie angegeben haben.</span><span class="sxs-lookup"><span data-stu-id="40cb0-159">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="40cb0-160">Um einen bereits vorhandenen Wert zu erhalten, immer als schließen Sie DisplayName in einem Aktualisierungsvorgang ein.</span><span class="sxs-lookup"><span data-stu-id="40cb0-160">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="40cb0-161">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="40cb0-161">emailAddresses</span></span>|<span data-ttu-id="40cb0-162">[TypedEmailAddress](../resources/typedemailaddress.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="40cb0-162">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="40cb0-163">Die E-Mail-Adressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-163">The contact's email addresses.</span></span>|
|<span data-ttu-id="40cb0-164">fileAs</span><span class="sxs-lookup"><span data-stu-id="40cb0-164">fileAs</span></span>|<span data-ttu-id="40cb0-165">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-165">String</span></span>|<span data-ttu-id="40cb0-166">Der Name, unter dem der Kontakt abgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="40cb0-166">The name the contact is filed under.</span></span>|
|<span data-ttu-id="40cb0-167">gender</span><span class="sxs-lookup"><span data-stu-id="40cb0-167">gender</span></span> |<span data-ttu-id="40cb0-168">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-168">String</span></span> |<span data-ttu-id="40cb0-169">Geschlecht des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-169">The contact's gender.</span></span> |
|<span data-ttu-id="40cb0-170">generation</span><span class="sxs-lookup"><span data-stu-id="40cb0-170">generation</span></span>|<span data-ttu-id="40cb0-171">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-171">String</span></span>|<span data-ttu-id="40cb0-172">Die Generation des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-172">The contact's generation.</span></span>|
|<span data-ttu-id="40cb0-173">givenName</span><span class="sxs-lookup"><span data-stu-id="40cb0-173">givenName</span></span>|<span data-ttu-id="40cb0-174">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-174">String</span></span>|<span data-ttu-id="40cb0-175">Der Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-175">The contact's given name.</span></span>|
|<span data-ttu-id="40cb0-176">imAddresses</span><span class="sxs-lookup"><span data-stu-id="40cb0-176">imAddresses</span></span>|<span data-ttu-id="40cb0-177">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-177">String</span></span>|<span data-ttu-id="40cb0-178">Instant Messaging Chatadressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-178">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="40cb0-179">initials</span><span class="sxs-lookup"><span data-stu-id="40cb0-179">initials</span></span>|<span data-ttu-id="40cb0-180">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-180">String</span></span>|<span data-ttu-id="40cb0-181">Die Initialen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-181">The contact's initials.</span></span>|
|<span data-ttu-id="40cb0-182">jobTitle</span><span class="sxs-lookup"><span data-stu-id="40cb0-182">jobTitle</span></span>|<span data-ttu-id="40cb0-183">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-183">String</span></span>|<span data-ttu-id="40cb0-184">Die Position des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-184">The contact’s job title.</span></span>|
|<span data-ttu-id="40cb0-185">manager</span><span class="sxs-lookup"><span data-stu-id="40cb0-185">manager</span></span>|<span data-ttu-id="40cb0-186">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-186">String</span></span>|<span data-ttu-id="40cb0-187">Der Name des Vorgesetzten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-187">The name of the contact's manager.</span></span>
|<span data-ttu-id="40cb0-188">middleName</span><span class="sxs-lookup"><span data-stu-id="40cb0-188">middleName</span></span>|<span data-ttu-id="40cb0-189">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-189">String</span></span>|<span data-ttu-id="40cb0-190">Der zweite Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-190">The contact's middle name.</span></span>|
|<span data-ttu-id="40cb0-191">nickName</span><span class="sxs-lookup"><span data-stu-id="40cb0-191">nickName</span></span>|<span data-ttu-id="40cb0-192">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-192">String</span></span>|<span data-ttu-id="40cb0-193">Der Spitzname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-193">The contact's nickname.</span></span>|
|<span data-ttu-id="40cb0-194">officeLocation</span><span class="sxs-lookup"><span data-stu-id="40cb0-194">officeLocation</span></span>|<span data-ttu-id="40cb0-195">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-195">String</span></span>|<span data-ttu-id="40cb0-196">Der Bürostandort des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-196">The location of the contact's office.</span></span>|
|<span data-ttu-id="40cb0-197">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="40cb0-197">parentFolderId</span></span>|<span data-ttu-id="40cb0-198">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-198">String</span></span>|<span data-ttu-id="40cb0-199">Die ID des übergeordneten Ordners des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-199">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="40cb0-200">personalNotes</span><span class="sxs-lookup"><span data-stu-id="40cb0-200">personalNotes</span></span>|<span data-ttu-id="40cb0-201">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-201">String</span></span>|<span data-ttu-id="40cb0-202">Die Notizen des Benutzers zu dem Kontakt.</span><span class="sxs-lookup"><span data-stu-id="40cb0-202">The user's notes about the contact.</span></span>|
|<span data-ttu-id="40cb0-203">phones</span><span class="sxs-lookup"><span data-stu-id="40cb0-203">phones</span></span> |<span data-ttu-id="40cb0-204">[phone](../resources/phone.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="40cb0-204">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="40cb0-205">Telefonnummern für den Kontakt zugeordnet ist, beispielsweise Telefon (privat), Mobiltelefon und Telefon (geschäftlich)</span><span class="sxs-lookup"><span data-stu-id="40cb0-205">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="40cb0-206">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="40cb0-206">postalAddresses</span></span> |<span data-ttu-id="40cb0-207">[physikalische Adresse](../resources/physicaladdress.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="40cb0-207">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="40cb0-208">Der Kontakt zugeordnete Adressen home beispielsweise Adresse und Geschäftsadresse.</span><span class="sxs-lookup"><span data-stu-id="40cb0-208">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="40cb0-209">profession</span><span class="sxs-lookup"><span data-stu-id="40cb0-209">profession</span></span>|<span data-ttu-id="40cb0-210">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-210">String</span></span>|<span data-ttu-id="40cb0-211">Der Beruf des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-211">The contact's profession.</span></span>|
|<span data-ttu-id="40cb0-212">spouseName</span><span class="sxs-lookup"><span data-stu-id="40cb0-212">spouseName</span></span>|<span data-ttu-id="40cb0-213">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="40cb0-213">String</span></span>|<span data-ttu-id="40cb0-214">Der Name des Ehepartners/Partners des Kontakts</span><span class="sxs-lookup"><span data-stu-id="40cb0-214">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="40cb0-215">surname</span><span class="sxs-lookup"><span data-stu-id="40cb0-215">surname</span></span>|<span data-ttu-id="40cb0-216">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-216">String</span></span>|<span data-ttu-id="40cb0-217">Der Nachname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-217">The contact's surname.</span></span>|
|<span data-ttu-id="40cb0-218">title</span><span class="sxs-lookup"><span data-stu-id="40cb0-218">title</span></span>|<span data-ttu-id="40cb0-219">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-219">String</span></span>|<span data-ttu-id="40cb0-220">Der Titel des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-220">The contact's title.</span></span>|
|<span data-ttu-id="40cb0-221">websites</span><span class="sxs-lookup"><span data-stu-id="40cb0-221">websites</span></span> |<span data-ttu-id="40cb0-222">[website](../resources/website.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="40cb0-222">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="40cb0-223">Websites, die dem Kontakt zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="40cb0-223">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="40cb0-224">weddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="40cb0-224">weddingAnniversary</span></span> |<span data-ttu-id="40cb0-225">Datum</span><span class="sxs-lookup"><span data-stu-id="40cb0-225">Date</span></span> |<span data-ttu-id="40cb0-226">Hochzeitstag des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="40cb0-226">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="40cb0-227">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="40cb0-227">yomiCompanyName</span></span>|<span data-ttu-id="40cb0-228">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-228">String</span></span>|<span data-ttu-id="40cb0-p108">Der phonetische japanische Firmenname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="40cb0-p108">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="40cb0-231">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="40cb0-231">yomiGivenName</span></span>|<span data-ttu-id="40cb0-232">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-232">String</span></span>|<span data-ttu-id="40cb0-p109">Der phonetische japanische Vorname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="40cb0-p109">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="40cb0-235">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="40cb0-235">yomiSurname</span></span>|<span data-ttu-id="40cb0-236">String</span><span class="sxs-lookup"><span data-stu-id="40cb0-236">String</span></span>|<span data-ttu-id="40cb0-p110">Der phonetische japanische Nachname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="40cb0-p110">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="40cb0-239">Da die Ressource **wenden Sie sich an** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren und Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz **wenden Sie sich an** .</span><span class="sxs-lookup"><span data-stu-id="40cb0-239">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="40cb0-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="40cb0-240">Response</span></span>

<span data-ttu-id="40cb0-241">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [wenden Sie sich an](../resources/contact.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="40cb0-241">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40cb0-242">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40cb0-242">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40cb0-243">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40cb0-243">Request</span></span>
<span data-ttu-id="40cb0-244">Das folgende Beispiel aktualisiert die persönlichen e-Mail-Adresse des angegebenen Kontakts an.</span><span class="sxs-lookup"><span data-stu-id="40cb0-244">The following example updates the personal email address of the specified contact.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contacts/AAMkADh6v5AAAvgTCEAAA=
Content-type: application/json

{
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
          "address": "pavelb@fabrikam.onmicrosoft.com",
          "name": "Pavel Bansky",
          "type": "other",
          "otherLabel": "Volunteer work"
        }
    ]
}
```
##### <a name="response"></a><span data-ttu-id="40cb0-245">Antwort</span><span class="sxs-lookup"><span data-stu-id="40cb0-245">Response</span></span>
<span data-ttu-id="40cb0-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40cb0-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T20:26:23Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
            "type":"other",
            "otherLabel":"Volunteer work",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="40cb0-249">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="40cb0-249">See also</span></span>

- [<span data-ttu-id="40cb0-250">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="40cb0-250">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="40cb0-251">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="40cb0-251">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->