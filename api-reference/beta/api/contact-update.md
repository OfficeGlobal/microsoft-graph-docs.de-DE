---
title: Kontakt aktualisieren
description: Aktualisieren Sie die Eigenschaften des Kontaktobjekts an.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c6ed3304b5f44a8bb1d35c1db491e8eaf7ae47b4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528207"
---
# <a name="update-contact"></a><span data-ttu-id="628bb-103">Kontakt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="628bb-103">Update contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="628bb-104">Aktualisieren Sie die Eigenschaften des Kontaktobjekts an.</span><span class="sxs-lookup"><span data-stu-id="628bb-104">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="628bb-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="628bb-105">Permissions</span></span>
<span data-ttu-id="628bb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="628bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="628bb-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="628bb-108">Permission type</span></span>      | <span data-ttu-id="628bb-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="628bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="628bb-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="628bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="628bb-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="628bb-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="628bb-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="628bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="628bb-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="628bb-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="628bb-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="628bb-114">Application</span></span> | <span data-ttu-id="628bb-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="628bb-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="628bb-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="628bb-116">HTTP request</span></span>
<span data-ttu-id="628bb-117"><!-- { "blockType": "ignored" } -->[Wenden Sie sich an](../resources/contact.md) von des Benutzers Standard [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="628bb-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="628bb-118">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="628bb-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="628bb-119">[Wenden Sie sich an](../resources/contact.md) , die in einem untergeordneten Ordner von einem [ContactFolder](../resources/mailfolder.md)enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="628bb-119">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="628bb-120">Das folgende Beispiel zeigt eine Ebene von schachteln, aber ein Kontakt kann befindet sich ein untergeordnetes Element des ein untergeordnetes Element und so weiter.</span><span class="sxs-lookup"><span data-stu-id="628bb-120">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="628bb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="628bb-121">Request headers</span></span>
| <span data-ttu-id="628bb-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="628bb-122">Header</span></span>       | <span data-ttu-id="628bb-123">Wert</span><span class="sxs-lookup"><span data-stu-id="628bb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="628bb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="628bb-124">Authorization</span></span>  | <span data-ttu-id="628bb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="628bb-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="628bb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="628bb-127">Content-Type</span></span>  | <span data-ttu-id="628bb-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="628bb-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="628bb-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="628bb-130">Request body</span></span>
<span data-ttu-id="628bb-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="628bb-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="628bb-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="628bb-134">Property</span></span>     | <span data-ttu-id="628bb-135">Typ</span><span class="sxs-lookup"><span data-stu-id="628bb-135">Type</span></span>   |<span data-ttu-id="628bb-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="628bb-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="628bb-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="628bb-137">assistantName</span></span>|<span data-ttu-id="628bb-138">String</span><span class="sxs-lookup"><span data-stu-id="628bb-138">String</span></span>|<span data-ttu-id="628bb-139">Der Name des Assistenten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="628bb-140">birthday</span><span class="sxs-lookup"><span data-stu-id="628bb-140">birthday</span></span>|<span data-ttu-id="628bb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="628bb-141">DateTimeOffset</span></span>|<span data-ttu-id="628bb-142">Das Geburtsdatum des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-142">The contact's birthday.</span></span>|
|<span data-ttu-id="628bb-143">categories</span><span class="sxs-lookup"><span data-stu-id="628bb-143">categories</span></span>|<span data-ttu-id="628bb-144">String</span><span class="sxs-lookup"><span data-stu-id="628bb-144">String</span></span>|<span data-ttu-id="628bb-145">Die Kategorien, die mit dem Kontakt verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="628bb-145">The categories associated with the contact.</span></span>|
|<span data-ttu-id="628bb-146">children</span><span class="sxs-lookup"><span data-stu-id="628bb-146">children</span></span>|<span data-ttu-id="628bb-147">String</span><span class="sxs-lookup"><span data-stu-id="628bb-147">String</span></span>||
|<span data-ttu-id="628bb-148">companyName</span><span class="sxs-lookup"><span data-stu-id="628bb-148">companyName</span></span>|<span data-ttu-id="628bb-149">String</span><span class="sxs-lookup"><span data-stu-id="628bb-149">String</span></span>|<span data-ttu-id="628bb-150">Der Name des Unternehmens des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-150">The name of the contact's company.</span></span>|
|<span data-ttu-id="628bb-151">department</span><span class="sxs-lookup"><span data-stu-id="628bb-151">department</span></span>|<span data-ttu-id="628bb-152">String</span><span class="sxs-lookup"><span data-stu-id="628bb-152">String</span></span>|<span data-ttu-id="628bb-153">Die Abteilung des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-153">The contact's department.</span></span>|
|<span data-ttu-id="628bb-154">displayName</span><span class="sxs-lookup"><span data-stu-id="628bb-154">displayName</span></span>|<span data-ttu-id="628bb-155">String</span><span class="sxs-lookup"><span data-stu-id="628bb-155">String</span></span>|<span data-ttu-id="628bb-156">Der Anzeigename des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-156">The contact's display name.</span></span> <span data-ttu-id="628bb-157">Beachten Sie, dass es sich bei spätere Aktualisierungen mit anderen Eigenschaften verursachen einen automatisch generierten Wert den Wert DisplayName überschrieben, den Sie angegeben haben.</span><span class="sxs-lookup"><span data-stu-id="628bb-157">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="628bb-158">Um einen bereits vorhandenen Wert zu erhalten, immer als schließen Sie DisplayName in einem Aktualisierungsvorgang ein.</span><span class="sxs-lookup"><span data-stu-id="628bb-158">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="628bb-159">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="628bb-159">emailAddresses</span></span>|<span data-ttu-id="628bb-160">[TypedEmailAddress](../resources/typedemailaddress.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="628bb-160">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="628bb-161">Die E-Mail-Adressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-161">The contact's email addresses.</span></span>|
|<span data-ttu-id="628bb-162">fileAs</span><span class="sxs-lookup"><span data-stu-id="628bb-162">fileAs</span></span>|<span data-ttu-id="628bb-163">String</span><span class="sxs-lookup"><span data-stu-id="628bb-163">String</span></span>|<span data-ttu-id="628bb-164">Der Name, unter dem der Kontakt abgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="628bb-164">The name the contact is filed under.</span></span>|
|<span data-ttu-id="628bb-165">gender</span><span class="sxs-lookup"><span data-stu-id="628bb-165">gender</span></span> |<span data-ttu-id="628bb-166">String</span><span class="sxs-lookup"><span data-stu-id="628bb-166">String</span></span> |<span data-ttu-id="628bb-167">Geschlecht des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-167">The contact's gender.</span></span> |
|<span data-ttu-id="628bb-168">generation</span><span class="sxs-lookup"><span data-stu-id="628bb-168">generation</span></span>|<span data-ttu-id="628bb-169">String</span><span class="sxs-lookup"><span data-stu-id="628bb-169">String</span></span>|<span data-ttu-id="628bb-170">Die Generation des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-170">The contact's generation.</span></span>|
|<span data-ttu-id="628bb-171">givenName</span><span class="sxs-lookup"><span data-stu-id="628bb-171">givenName</span></span>|<span data-ttu-id="628bb-172">String</span><span class="sxs-lookup"><span data-stu-id="628bb-172">String</span></span>|<span data-ttu-id="628bb-173">Der Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-173">The contact's given name.</span></span>|
|<span data-ttu-id="628bb-174">imAddresses</span><span class="sxs-lookup"><span data-stu-id="628bb-174">imAddresses</span></span>|<span data-ttu-id="628bb-175">String</span><span class="sxs-lookup"><span data-stu-id="628bb-175">String</span></span>|<span data-ttu-id="628bb-176">Instant Messaging Chatadressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-176">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="628bb-177">initials</span><span class="sxs-lookup"><span data-stu-id="628bb-177">initials</span></span>|<span data-ttu-id="628bb-178">String</span><span class="sxs-lookup"><span data-stu-id="628bb-178">String</span></span>|<span data-ttu-id="628bb-179">Die Initialen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-179">The contact's initials.</span></span>|
|<span data-ttu-id="628bb-180">jobTitle</span><span class="sxs-lookup"><span data-stu-id="628bb-180">jobTitle</span></span>|<span data-ttu-id="628bb-181">String</span><span class="sxs-lookup"><span data-stu-id="628bb-181">String</span></span>|<span data-ttu-id="628bb-182">Die Position des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-182">The contact’s job title.</span></span>|
|<span data-ttu-id="628bb-183">manager</span><span class="sxs-lookup"><span data-stu-id="628bb-183">manager</span></span>|<span data-ttu-id="628bb-184">String</span><span class="sxs-lookup"><span data-stu-id="628bb-184">String</span></span>|<span data-ttu-id="628bb-185">Der Name des Vorgesetzten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-185">The name of the contact's manager.</span></span>
|<span data-ttu-id="628bb-186">middleName</span><span class="sxs-lookup"><span data-stu-id="628bb-186">middleName</span></span>|<span data-ttu-id="628bb-187">String</span><span class="sxs-lookup"><span data-stu-id="628bb-187">String</span></span>|<span data-ttu-id="628bb-188">Der zweite Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-188">The contact's middle name.</span></span>|
|<span data-ttu-id="628bb-189">nickName</span><span class="sxs-lookup"><span data-stu-id="628bb-189">nickName</span></span>|<span data-ttu-id="628bb-190">String</span><span class="sxs-lookup"><span data-stu-id="628bb-190">String</span></span>|<span data-ttu-id="628bb-191">Der Spitzname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-191">The contact's nickname.</span></span>|
|<span data-ttu-id="628bb-192">officeLocation</span><span class="sxs-lookup"><span data-stu-id="628bb-192">officeLocation</span></span>|<span data-ttu-id="628bb-193">String</span><span class="sxs-lookup"><span data-stu-id="628bb-193">String</span></span>|<span data-ttu-id="628bb-194">Der Bürostandort des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-194">The location of the contact's office.</span></span>|
|<span data-ttu-id="628bb-195">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="628bb-195">parentFolderId</span></span>|<span data-ttu-id="628bb-196">String</span><span class="sxs-lookup"><span data-stu-id="628bb-196">String</span></span>|<span data-ttu-id="628bb-197">Die ID des übergeordneten Ordners des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-197">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="628bb-198">personalNotes</span><span class="sxs-lookup"><span data-stu-id="628bb-198">personalNotes</span></span>|<span data-ttu-id="628bb-199">String</span><span class="sxs-lookup"><span data-stu-id="628bb-199">String</span></span>|<span data-ttu-id="628bb-200">Die Notizen des Benutzers zu dem Kontakt.</span><span class="sxs-lookup"><span data-stu-id="628bb-200">The user's notes about the contact.</span></span>|
|<span data-ttu-id="628bb-201">phones</span><span class="sxs-lookup"><span data-stu-id="628bb-201">phones</span></span> |<span data-ttu-id="628bb-202">[phone](../resources/phone.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="628bb-202">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="628bb-203">Telefonnummern für den Kontakt zugeordnet ist, beispielsweise Telefon (privat), Mobiltelefon und Telefon (geschäftlich)</span><span class="sxs-lookup"><span data-stu-id="628bb-203">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="628bb-204">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="628bb-204">postalAddresses</span></span> |<span data-ttu-id="628bb-205">[physikalische Adresse](../resources/physicaladdress.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="628bb-205">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="628bb-206">Der Kontakt zugeordnete Adressen home beispielsweise Adresse und Geschäftsadresse.</span><span class="sxs-lookup"><span data-stu-id="628bb-206">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="628bb-207">profession</span><span class="sxs-lookup"><span data-stu-id="628bb-207">profession</span></span>|<span data-ttu-id="628bb-208">String</span><span class="sxs-lookup"><span data-stu-id="628bb-208">String</span></span>|<span data-ttu-id="628bb-209">Der Beruf des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-209">The contact's profession.</span></span>|
|<span data-ttu-id="628bb-210">spouseName</span><span class="sxs-lookup"><span data-stu-id="628bb-210">spouseName</span></span>|<span data-ttu-id="628bb-211">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="628bb-211">String</span></span>|<span data-ttu-id="628bb-212">Der Name des Ehepartners/Partners des Kontakts</span><span class="sxs-lookup"><span data-stu-id="628bb-212">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="628bb-213">surname</span><span class="sxs-lookup"><span data-stu-id="628bb-213">surname</span></span>|<span data-ttu-id="628bb-214">String</span><span class="sxs-lookup"><span data-stu-id="628bb-214">String</span></span>|<span data-ttu-id="628bb-215">Der Nachname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-215">The contact's surname.</span></span>|
|<span data-ttu-id="628bb-216">title</span><span class="sxs-lookup"><span data-stu-id="628bb-216">title</span></span>|<span data-ttu-id="628bb-217">String</span><span class="sxs-lookup"><span data-stu-id="628bb-217">String</span></span>|<span data-ttu-id="628bb-218">Der Titel des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-218">The contact's title.</span></span>|
|<span data-ttu-id="628bb-219">websites</span><span class="sxs-lookup"><span data-stu-id="628bb-219">websites</span></span> |<span data-ttu-id="628bb-220">[website](../resources/website.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="628bb-220">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="628bb-221">Websites, die dem Kontakt zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="628bb-221">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="628bb-222">WeddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="628bb-222">weddingAnniversary</span></span> |<span data-ttu-id="628bb-223">Datum</span><span class="sxs-lookup"><span data-stu-id="628bb-223">Date</span></span> |<span data-ttu-id="628bb-224">Hochzeitstag des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="628bb-224">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="628bb-225">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="628bb-225">yomiCompanyName</span></span>|<span data-ttu-id="628bb-226">String</span><span class="sxs-lookup"><span data-stu-id="628bb-226">String</span></span>|<span data-ttu-id="628bb-p107">Der phonetische japanische Firmenname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="628bb-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="628bb-229">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="628bb-229">yomiGivenName</span></span>|<span data-ttu-id="628bb-230">String</span><span class="sxs-lookup"><span data-stu-id="628bb-230">String</span></span>|<span data-ttu-id="628bb-p108">Der phonetische japanische Vorname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="628bb-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="628bb-233">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="628bb-233">yomiSurname</span></span>|<span data-ttu-id="628bb-234">String</span><span class="sxs-lookup"><span data-stu-id="628bb-234">String</span></span>|<span data-ttu-id="628bb-p109">Der phonetische japanische Nachname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="628bb-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="628bb-237">Da die Ressource **wenden Sie sich an** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren und Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz **wenden Sie sich an** .</span><span class="sxs-lookup"><span data-stu-id="628bb-237">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="628bb-238">Antwort</span><span class="sxs-lookup"><span data-stu-id="628bb-238">Response</span></span>

<span data-ttu-id="628bb-239">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [wenden Sie sich an](../resources/contact.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="628bb-239">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="628bb-240">Beispiel</span><span class="sxs-lookup"><span data-stu-id="628bb-240">Example</span></span>
##### <a name="request"></a><span data-ttu-id="628bb-241">Anforderung</span><span class="sxs-lookup"><span data-stu-id="628bb-241">Request</span></span>
<span data-ttu-id="628bb-242">Das folgende Beispiel aktualisiert die persönlichen e-Mail-Adresse des angegebenen Kontakts an.</span><span class="sxs-lookup"><span data-stu-id="628bb-242">The following example updates the personal email address of the specified contact.</span></span>
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
##### <a name="response"></a><span data-ttu-id="628bb-243">Antwort</span><span class="sxs-lookup"><span data-stu-id="628bb-243">Response</span></span>
<span data-ttu-id="628bb-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="628bb-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="628bb-247">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="628bb-247">See also</span></span>

- [<span data-ttu-id="628bb-248">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="628bb-248">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="628bb-249">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="628bb-249">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contact-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
