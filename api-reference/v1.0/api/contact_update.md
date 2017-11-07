# <a name="update-contact"></a><span data-ttu-id="e0ab5-101">Kontakt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e0ab5-101">Update contact</span></span>

<span data-ttu-id="e0ab5-102">Mit dieser API können Sie die Eigenschaften eines Kontaktobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-102">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0ab5-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e0ab5-103">Permissions</span></span>
<span data-ttu-id="e0ab5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e0ab5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e0ab5-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e0ab5-106">Permission type</span></span>      | <span data-ttu-id="e0ab5-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e0ab5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0ab5-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0ab5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e0ab5-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0ab5-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e0ab5-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e0ab5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0ab5-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0ab5-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e0ab5-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0ab5-112">Application</span></span> | <span data-ttu-id="e0ab5-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0ab5-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0ab5-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0ab5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="e0ab5-115">Ein [Kontakt](../resources/contact.md) aus dem standardmäßigen [contactFolder](../resources/contactfolder.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="e0ab5-116">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="e0ab5-p102">Ein [Kontakt](../resources/contact.md) in einem untergeordneten Ordner eines [contactFolder](../resources/mailfolder.md). Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e0ab5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0ab5-119">Request headers</span></span>
| <span data-ttu-id="e0ab5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e0ab5-120">Header</span></span>       | <span data-ttu-id="e0ab5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e0ab5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0ab5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0ab5-122">Authorization</span></span>  | <span data-ttu-id="e0ab5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e0ab5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0ab5-125">Content-Type</span></span>  | <span data-ttu-id="e0ab5-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e0ab5-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0ab5-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0ab5-128">Request body</span></span>
<span data-ttu-id="e0ab5-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e0ab5-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0ab5-132">Property</span></span>     | <span data-ttu-id="e0ab5-133">Typ</span><span class="sxs-lookup"><span data-stu-id="e0ab5-133">Type</span></span>   |<span data-ttu-id="e0ab5-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0ab5-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0ab5-135">assistantName</span><span class="sxs-lookup"><span data-stu-id="e0ab5-135">assistantName</span></span>|<span data-ttu-id="e0ab5-136">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-136">String</span></span>|<span data-ttu-id="e0ab5-137">Der Name des Assistenten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-137">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="e0ab5-138">birthday</span><span class="sxs-lookup"><span data-stu-id="e0ab5-138">birthday</span></span>|<span data-ttu-id="e0ab5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0ab5-139">DateTimeOffset</span></span>|<span data-ttu-id="e0ab5-140">Das Geburtsdatum des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-140">The contact's birthday.</span></span>|
|<span data-ttu-id="e0ab5-141">businessAddress</span><span class="sxs-lookup"><span data-stu-id="e0ab5-141">businessAddress</span></span>|[<span data-ttu-id="e0ab5-142">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="e0ab5-142">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="e0ab5-143">Die Geschäftsadresse des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-143">The contact's business address.</span></span>|
|<span data-ttu-id="e0ab5-144">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="e0ab5-144">businessHomePage</span></span>|<span data-ttu-id="e0ab5-145">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-145">String</span></span>|<span data-ttu-id="e0ab5-146">Die geschäftliche Homepage des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-146">The business home page of the contact.</span></span>|
|<span data-ttu-id="e0ab5-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="e0ab5-147">businessPhones</span></span>|<span data-ttu-id="e0ab5-148">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-148">String</span></span>|<span data-ttu-id="e0ab5-149">Die geschäftlichen Telefonnummern des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-149">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="e0ab5-150">categories</span><span class="sxs-lookup"><span data-stu-id="e0ab5-150">categories</span></span>|<span data-ttu-id="e0ab5-151">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-151">String</span></span>|<span data-ttu-id="e0ab5-152">Die Kategorien, die mit dem Kontakt verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-152">The categories associated with the contact.</span></span>|
|<span data-ttu-id="e0ab5-153">children</span><span class="sxs-lookup"><span data-stu-id="e0ab5-153">children</span></span>|<span data-ttu-id="e0ab5-154">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-154">String</span></span>|<span data-ttu-id="e0ab5-155">Die Namen der Kinder des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-155">The names of the contact's children.</span></span>|
|<span data-ttu-id="e0ab5-156">companyName</span><span class="sxs-lookup"><span data-stu-id="e0ab5-156">companyName</span></span>|<span data-ttu-id="e0ab5-157">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-157">String</span></span>|<span data-ttu-id="e0ab5-158">Der Name des Unternehmens des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-158">The name of the contact's company.</span></span>|
|<span data-ttu-id="e0ab5-159">department</span><span class="sxs-lookup"><span data-stu-id="e0ab5-159">department</span></span>|<span data-ttu-id="e0ab5-160">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-160">String</span></span>|<span data-ttu-id="e0ab5-161">Die Abteilung des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-161">The contact's department.</span></span>|
|<span data-ttu-id="e0ab5-162">displayName</span><span class="sxs-lookup"><span data-stu-id="e0ab5-162">displayName</span></span>|<span data-ttu-id="e0ab5-163">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-163">String</span></span>|<span data-ttu-id="e0ab5-164">Der Anzeigename des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-164">The contact's display name.</span></span>|
|<span data-ttu-id="e0ab5-165">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="e0ab5-165">emailAddresses</span></span>|<span data-ttu-id="e0ab5-166">[EmailAddress](../resources/emailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="e0ab5-166">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="e0ab5-167">Die E-Mail-Adressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-167">The contact's email addresses.</span></span>|
|<span data-ttu-id="e0ab5-168">fileAs</span><span class="sxs-lookup"><span data-stu-id="e0ab5-168">fileAs</span></span>|<span data-ttu-id="e0ab5-169">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-169">String</span></span>|<span data-ttu-id="e0ab5-170">Der Name, unter dem der Kontakt abgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-170">The name the contact is filed under.</span></span>|
|<span data-ttu-id="e0ab5-171">generation</span><span class="sxs-lookup"><span data-stu-id="e0ab5-171">generation</span></span>|<span data-ttu-id="e0ab5-172">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-172">String</span></span>|<span data-ttu-id="e0ab5-173">Die Generation des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-173">The contact's generation.</span></span>|
|<span data-ttu-id="e0ab5-174">givenName</span><span class="sxs-lookup"><span data-stu-id="e0ab5-174">givenName</span></span>|<span data-ttu-id="e0ab5-175">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-175">String</span></span>|<span data-ttu-id="e0ab5-176">Der Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-176">The contact's given name.</span></span>|
|<span data-ttu-id="e0ab5-177">homeAddress</span><span class="sxs-lookup"><span data-stu-id="e0ab5-177">homeAddress</span></span>|[<span data-ttu-id="e0ab5-178">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="e0ab5-178">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="e0ab5-179">Die Privatadresse des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-179">The contact's home address.</span></span>|
|<span data-ttu-id="e0ab5-180">homePhones</span><span class="sxs-lookup"><span data-stu-id="e0ab5-180">homePhones</span></span>|<span data-ttu-id="e0ab5-181">String collection</span><span class="sxs-lookup"><span data-stu-id="e0ab5-181">String collection</span></span>|<span data-ttu-id="e0ab5-182">Die privaten Telefonnummern des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-182">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="e0ab5-183">imAddresses</span><span class="sxs-lookup"><span data-stu-id="e0ab5-183">imAddresses</span></span>|<span data-ttu-id="e0ab5-184">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-184">String</span></span>|<span data-ttu-id="e0ab5-185">Instant Messaging Chatadressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-185">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="e0ab5-186">initials</span><span class="sxs-lookup"><span data-stu-id="e0ab5-186">initials</span></span>|<span data-ttu-id="e0ab5-187">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-187">String</span></span>|<span data-ttu-id="e0ab5-188">Die Initialen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-188">The contact's initials.</span></span>|
|<span data-ttu-id="e0ab5-189">jobTitle</span><span class="sxs-lookup"><span data-stu-id="e0ab5-189">jobTitle</span></span>|<span data-ttu-id="e0ab5-190">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-190">String</span></span>|<span data-ttu-id="e0ab5-191">Die Position des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-191">The contact’s job title.</span></span>|
|<span data-ttu-id="e0ab5-192">manager</span><span class="sxs-lookup"><span data-stu-id="e0ab5-192">manager</span></span>|<span data-ttu-id="e0ab5-193">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-193">String</span></span>|<span data-ttu-id="e0ab5-194">Der Name des Vorgesetzten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-194">The name of the contact's manager.</span></span>
|<span data-ttu-id="e0ab5-195">middleName</span><span class="sxs-lookup"><span data-stu-id="e0ab5-195">middleName</span></span>|<span data-ttu-id="e0ab5-196">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-196">String</span></span>|<span data-ttu-id="e0ab5-197">Der zweite Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-197">The contact's middle name.</span></span>|
|<span data-ttu-id="e0ab5-198">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="e0ab5-198">mobilePhone</span></span>|<span data-ttu-id="e0ab5-199">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-199">String</span></span>|<span data-ttu-id="e0ab5-200">Die Mobiltelefonnummer des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-200">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="e0ab5-201">nickName</span><span class="sxs-lookup"><span data-stu-id="e0ab5-201">nickName</span></span>|<span data-ttu-id="e0ab5-202">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-202">String</span></span>|<span data-ttu-id="e0ab5-203">Der Spitzname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-203">The contact's nickname.</span></span>|
|<span data-ttu-id="e0ab5-204">officeLocation</span><span class="sxs-lookup"><span data-stu-id="e0ab5-204">officeLocation</span></span>|<span data-ttu-id="e0ab5-205">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-205">String</span></span>|<span data-ttu-id="e0ab5-206">Der Bürostandort des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-206">The location of the contact's office.</span></span>|
|<span data-ttu-id="e0ab5-207">otherAddress</span><span class="sxs-lookup"><span data-stu-id="e0ab5-207">otherAddress</span></span>|[<span data-ttu-id="e0ab5-208">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="e0ab5-208">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="e0ab5-209">Weitere Adressen für den Kontakt.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-209">Other addresses for the contact.</span></span>|
|<span data-ttu-id="e0ab5-210">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="e0ab5-210">parentFolderId</span></span>|<span data-ttu-id="e0ab5-211">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-211">String</span></span>|<span data-ttu-id="e0ab5-212">Die ID des übergeordneten Ordners des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-212">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="e0ab5-213">personalNotes</span><span class="sxs-lookup"><span data-stu-id="e0ab5-213">personalNotes</span></span>|<span data-ttu-id="e0ab5-214">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-214">String</span></span>|<span data-ttu-id="e0ab5-215">Die Notizen des Benutzers zu dem Kontakt.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-215">The user's notes about the contact.</span></span>|
|<span data-ttu-id="e0ab5-216">profession</span><span class="sxs-lookup"><span data-stu-id="e0ab5-216">profession</span></span>|<span data-ttu-id="e0ab5-217">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-217">String</span></span>|<span data-ttu-id="e0ab5-218">Der Beruf des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-218">The contact's profession.</span></span>|
|<span data-ttu-id="e0ab5-219">spouseName</span><span class="sxs-lookup"><span data-stu-id="e0ab5-219">spouseName</span></span>|<span data-ttu-id="e0ab5-220">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0ab5-220">String</span></span>|<span data-ttu-id="e0ab5-221">Der Name des Ehepartners/Partners des Kontakts</span><span class="sxs-lookup"><span data-stu-id="e0ab5-221">The name of the contact's spouse.</span></span>|
|<span data-ttu-id="e0ab5-222">surname</span><span class="sxs-lookup"><span data-stu-id="e0ab5-222">surname</span></span>|<span data-ttu-id="e0ab5-223">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-223">String</span></span>|<span data-ttu-id="e0ab5-224">Der Nachname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-224">The contact's surname.</span></span>|
|<span data-ttu-id="e0ab5-225">title</span><span class="sxs-lookup"><span data-stu-id="e0ab5-225">title</span></span>|<span data-ttu-id="e0ab5-226">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-226">String</span></span>|<span data-ttu-id="e0ab5-227">Der Titel des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-227">The contact's title.</span></span>|
|<span data-ttu-id="e0ab5-228">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="e0ab5-228">yomiCompanyName</span></span>|<span data-ttu-id="e0ab5-229">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-229">String</span></span>|<span data-ttu-id="e0ab5-p106">Der phonetische japanische Firmenname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-p106">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="e0ab5-232">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="e0ab5-232">yomiGivenName</span></span>|<span data-ttu-id="e0ab5-233">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-233">String</span></span>|<span data-ttu-id="e0ab5-p107">Der phonetische japanische Vorname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-p107">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="e0ab5-236">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="e0ab5-236">yomiSurname</span></span>|<span data-ttu-id="e0ab5-237">String</span><span class="sxs-lookup"><span data-stu-id="e0ab5-237">String</span></span>|<span data-ttu-id="e0ab5-p108">Der phonetische japanische Nachname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-p108">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="e0ab5-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0ab5-240">Response</span></span>

<span data-ttu-id="e0ab5-241">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-241">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0ab5-242">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0ab5-242">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0ab5-243">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0ab5-243">Request</span></span>
<span data-ttu-id="e0ab5-244">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-244">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e0ab5-245">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0ab5-245">Response</span></span>
<span data-ttu-id="e0ab5-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0ab5-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "businessHomePage": "http://www.contoso.com",
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
