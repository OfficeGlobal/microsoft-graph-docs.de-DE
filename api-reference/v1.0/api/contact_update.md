# <a name="update-contact"></a><span data-ttu-id="15ac9-101">Kontakt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="15ac9-101">Update contact</span></span>

<span data-ttu-id="15ac9-102">Mit dieser API können Sie die Eigenschaften eines Kontaktobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="15ac9-102">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="15ac9-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="15ac9-103">Permissions</span></span>
<span data-ttu-id="15ac9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="15ac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="15ac9-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15ac9-106">Permission type</span></span>      | <span data-ttu-id="15ac9-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15ac9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15ac9-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15ac9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="15ac9-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ac9-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="15ac9-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15ac9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15ac9-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ac9-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="15ac9-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15ac9-112">Application</span></span> | <span data-ttu-id="15ac9-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ac9-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="15ac9-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15ac9-114">HTTP request</span></span>
<span data-ttu-id="15ac9-115"><!-- { "blockType": "ignored" } -->[Wenden Sie sich](../resources/contact.md) von einem Benutzer standardmäßig [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="15ac9-115"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="15ac9-116">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="15ac9-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="15ac9-p102">Ein [Kontakt](../resources/contact.md) in einem untergeordneten Ordner eines [contactFolder](../resources/mailfolder.md). Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="15ac9-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="15ac9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15ac9-119">Request headers</span></span>
| <span data-ttu-id="15ac9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="15ac9-120">Header</span></span>       | <span data-ttu-id="15ac9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="15ac9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="15ac9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15ac9-122">Authorization</span></span>  | <span data-ttu-id="15ac9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15ac9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="15ac9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15ac9-125">Content-Type</span></span>  | <span data-ttu-id="15ac9-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="15ac9-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="15ac9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15ac9-128">Request body</span></span>
<span data-ttu-id="15ac9-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="15ac9-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="15ac9-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15ac9-132">Property</span></span>     | <span data-ttu-id="15ac9-133">Typ</span><span class="sxs-lookup"><span data-stu-id="15ac9-133">Type</span></span>   |<span data-ttu-id="15ac9-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15ac9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15ac9-135">assistantName</span><span class="sxs-lookup"><span data-stu-id="15ac9-135">assistantName</span></span>|<span data-ttu-id="15ac9-136">String</span><span class="sxs-lookup"><span data-stu-id="15ac9-136">String</span></span>|<span data-ttu-id="15ac9-137">Der Name des Assistenten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-137">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="15ac9-138">birthday</span><span class="sxs-lookup"><span data-stu-id="15ac9-138">birthday</span></span>|<span data-ttu-id="15ac9-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15ac9-139">DateTimeOffset</span></span>|<span data-ttu-id="15ac9-140">Das Geburtsdatum des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-140">The contact's birthday.</span></span>|
|<span data-ttu-id="15ac9-141">businessAddress</span><span class="sxs-lookup"><span data-stu-id="15ac9-141">businessAddress</span></span>|[<span data-ttu-id="15ac9-142">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="15ac9-142">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="15ac9-143">Die Geschäftsadresse des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-143">The contact's business address.</span></span>|
|<span data-ttu-id="15ac9-144">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="15ac9-144">businessHomePage</span></span>|<span data-ttu-id="15ac9-145">String</span><span class="sxs-lookup"><span data-stu-id="15ac9-145">String</span></span>|<span data-ttu-id="15ac9-146">Die geschäftliche Homepage des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-146">The business home page of the contact.</span></span>|
|<span data-ttu-id="15ac9-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="15ac9-147">businessPhones</span></span>|<span data-ttu-id="15ac9-148">String</span><span class="sxs-lookup"><span data-stu-id="15ac9-148">String</span></span>|<span data-ttu-id="15ac9-149">Die geschäftlichen Telefonnummern des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-149">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="15ac9-150">categories</span><span class="sxs-lookup"><span data-stu-id="15ac9-150">categories</span></span>|<span data-ttu-id="15ac9-151">String</span><span class="sxs-lookup"><span data-stu-id="15ac9-151">String</span></span>|<span data-ttu-id="15ac9-152">Die Kategorien, die mit dem Kontakt verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="15ac9-152">The categories associated with the contact.</span></span>|
|<span data-ttu-id="15ac9-153">children</span><span class="sxs-lookup"><span data-stu-id="15ac9-153">children</span></span>|<span data-ttu-id="15ac9-154">String</span><span class="sxs-lookup"><span data-stu-id="15ac9-154">String</span></span>|<span data-ttu-id="15ac9-155">Die Namen der Kinder des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-155">The names of the contact's children.</span></span>|
|<span data-ttu-id="15ac9-156">companyName</span><span class="sxs-lookup"><span data-stu-id="15ac9-156">companyName</span></span>|<span data-ttu-id="15ac9-157">String</span><span class="sxs-lookup"><span data-stu-id="15ac9-157">String</span></span>|<span data-ttu-id="15ac9-158">Der Name des Unternehmens des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-158">The name of the contact's company.</span></span>|
|<span data-ttu-id="15ac9-159">department</span><span class="sxs-lookup"><span data-stu-id="15ac9-159">department</span></span>|<span data-ttu-id="15ac9-160">String</span><span class="sxs-lookup"><span data-stu-id="15ac9-160">String</span></span>|<span data-ttu-id="15ac9-161">Die Abteilung des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-161">The contact's department.</span></span>|
|<span data-ttu-id="15ac9-162">displayName</span><span class="sxs-lookup"><span data-stu-id="15ac9-162">displayName</span></span>|<span data-ttu-id="15ac9-163">String</span><span class="sxs-lookup"><span data-stu-id="15ac9-163">String</span></span>|<span data-ttu-id="15ac9-164">Der Anzeigename des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-164">The contact's display name.</span></span> <span data-ttu-id="15ac9-165">Beachten Sie, dass es sich bei spätere Aktualisierungen mit anderen Eigenschaften verursachen einen automatisch generierten Wert den Wert DisplayName überschrieben, den Sie angegeben haben.</span><span class="sxs-lookup"><span data-stu-id="15ac9-165">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="15ac9-166">Um einen bereits vorhandenen Wert zu erhalten, immer als schließen Sie DisplayName in einem Aktualisierungsvorgang ein.</span><span class="sxs-lookup"><span data-stu-id="15ac9-166">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="15ac9-167">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="15ac9-167">emailAddresses</span></span>|<span data-ttu-id="15ac9-168">[EmailAddress](../resources/emailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="15ac9-168">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="15ac9-169">Die E-Mail-Adressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-169">The contact's email addresses.</span></span>|
|<span data-ttu-id="15ac9-170">fileAs</span><span class="sxs-lookup"><span data-stu-id="15ac9-170">fileAs</span></span>|<span data-ttu-id="15ac9-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-171">String</span></span>|<span data-ttu-id="15ac9-172">Der Name, unter dem der Kontakt abgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="15ac9-172">The name the contact is filed under.</span></span>|
|<span data-ttu-id="15ac9-173">generation</span><span class="sxs-lookup"><span data-stu-id="15ac9-173">generation</span></span>|<span data-ttu-id="15ac9-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-174">String</span></span>|<span data-ttu-id="15ac9-175">Die Generation des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-175">The contact's generation.</span></span>|
|<span data-ttu-id="15ac9-176">givenName</span><span class="sxs-lookup"><span data-stu-id="15ac9-176">givenName</span></span>|<span data-ttu-id="15ac9-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-177">String</span></span>|<span data-ttu-id="15ac9-178">Der Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-178">The contact's given name.</span></span>|
|<span data-ttu-id="15ac9-179">homeAddress</span><span class="sxs-lookup"><span data-stu-id="15ac9-179">homeAddress</span></span>|[<span data-ttu-id="15ac9-180">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="15ac9-180">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="15ac9-181">Die Privatadresse des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-181">The contact's home address.</span></span>|
|<span data-ttu-id="15ac9-182">homePhones</span><span class="sxs-lookup"><span data-stu-id="15ac9-182">homePhones</span></span>|<span data-ttu-id="15ac9-183">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="15ac9-183">String collection</span></span>|<span data-ttu-id="15ac9-184">Die privaten Telefonnummern des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-184">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="15ac9-185">imAddresses</span><span class="sxs-lookup"><span data-stu-id="15ac9-185">imAddresses</span></span>|<span data-ttu-id="15ac9-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-186">String</span></span>|<span data-ttu-id="15ac9-187">Instant Messaging Chatadressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-187">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="15ac9-188">initials</span><span class="sxs-lookup"><span data-stu-id="15ac9-188">initials</span></span>|<span data-ttu-id="15ac9-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-189">String</span></span>|<span data-ttu-id="15ac9-190">Die Initialen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-190">The contact's initials.</span></span>|
|<span data-ttu-id="15ac9-191">jobTitle</span><span class="sxs-lookup"><span data-stu-id="15ac9-191">jobTitle</span></span>|<span data-ttu-id="15ac9-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-192">String</span></span>|<span data-ttu-id="15ac9-193">Die Position des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-193">The contact’s job title.</span></span>|
|<span data-ttu-id="15ac9-194">manager</span><span class="sxs-lookup"><span data-stu-id="15ac9-194">manager</span></span>|<span data-ttu-id="15ac9-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-195">String</span></span>|<span data-ttu-id="15ac9-196">Der Name des Vorgesetzten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-196">The name of the contact's manager.</span></span>
|<span data-ttu-id="15ac9-197">middleName</span><span class="sxs-lookup"><span data-stu-id="15ac9-197">middleName</span></span>|<span data-ttu-id="15ac9-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-198">String</span></span>|<span data-ttu-id="15ac9-199">Der zweite Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-199">The contact's middle name.</span></span>|
|<span data-ttu-id="15ac9-200">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="15ac9-200">mobilePhone</span></span>|<span data-ttu-id="15ac9-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-201">String</span></span>|<span data-ttu-id="15ac9-202">Die Mobiltelefonnummer des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-202">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="15ac9-203">nickName</span><span class="sxs-lookup"><span data-stu-id="15ac9-203">nickName</span></span>|<span data-ttu-id="15ac9-204">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-204">String</span></span>|<span data-ttu-id="15ac9-205">Der Spitzname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-205">The contact's nickname.</span></span>|
|<span data-ttu-id="15ac9-206">officeLocation</span><span class="sxs-lookup"><span data-stu-id="15ac9-206">officeLocation</span></span>|<span data-ttu-id="15ac9-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-207">String</span></span>|<span data-ttu-id="15ac9-208">Der Bürostandort des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-208">The location of the contact's office.</span></span>|
|<span data-ttu-id="15ac9-209">otherAddress</span><span class="sxs-lookup"><span data-stu-id="15ac9-209">otherAddress</span></span>|[<span data-ttu-id="15ac9-210">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="15ac9-210">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="15ac9-211">Weitere Adressen für den Kontakt.</span><span class="sxs-lookup"><span data-stu-id="15ac9-211">Other addresses for the contact.</span></span>|
|<span data-ttu-id="15ac9-212">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="15ac9-212">parentFolderId</span></span>|<span data-ttu-id="15ac9-213">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-213">String</span></span>|<span data-ttu-id="15ac9-214">Die ID des übergeordneten Ordners des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-214">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="15ac9-215">personalNotes</span><span class="sxs-lookup"><span data-stu-id="15ac9-215">personalNotes</span></span>|<span data-ttu-id="15ac9-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-216">String</span></span>|<span data-ttu-id="15ac9-217">Die Notizen des Benutzers zu dem Kontakt.</span><span class="sxs-lookup"><span data-stu-id="15ac9-217">The user's notes about the contact.</span></span>|
|<span data-ttu-id="15ac9-218">profession</span><span class="sxs-lookup"><span data-stu-id="15ac9-218">profession</span></span>|<span data-ttu-id="15ac9-219">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-219">String</span></span>|<span data-ttu-id="15ac9-220">Der Beruf des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-220">The contact's profession.</span></span>|
|<span data-ttu-id="15ac9-221">spouseName</span><span class="sxs-lookup"><span data-stu-id="15ac9-221">spouseName</span></span>|<span data-ttu-id="15ac9-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-222">String</span></span>|<span data-ttu-id="15ac9-223">Der Name des Ehepartners/Partners des Kontakts</span><span class="sxs-lookup"><span data-stu-id="15ac9-223">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="15ac9-224">surname</span><span class="sxs-lookup"><span data-stu-id="15ac9-224">surname</span></span>|<span data-ttu-id="15ac9-225">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-225">String</span></span>|<span data-ttu-id="15ac9-226">Der Nachname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-226">The contact's surname.</span></span>|
|<span data-ttu-id="15ac9-227">title</span><span class="sxs-lookup"><span data-stu-id="15ac9-227">title</span></span>|<span data-ttu-id="15ac9-228">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-228">String</span></span>|<span data-ttu-id="15ac9-229">Der Titel des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="15ac9-229">The contact's title.</span></span>|
|<span data-ttu-id="15ac9-230">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="15ac9-230">yomiCompanyName</span></span>|<span data-ttu-id="15ac9-231">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-231">String</span></span>|<span data-ttu-id="15ac9-p107">Der phonetische japanische Firmenname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="15ac9-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="15ac9-234">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="15ac9-234">yomiGivenName</span></span>|<span data-ttu-id="15ac9-235">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-235">String</span></span>|<span data-ttu-id="15ac9-p108">Der phonetische japanische Vorname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="15ac9-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="15ac9-238">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="15ac9-238">yomiSurname</span></span>|<span data-ttu-id="15ac9-239">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ac9-239">String</span></span>|<span data-ttu-id="15ac9-p109">Der phonetische japanische Nachname des Kontakts. Diese Eigenschaft ist optional.</span><span class="sxs-lookup"><span data-stu-id="15ac9-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="15ac9-242">Antwort</span><span class="sxs-lookup"><span data-stu-id="15ac9-242">Response</span></span>

<span data-ttu-id="15ac9-243">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15ac9-243">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15ac9-244">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15ac9-244">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15ac9-245">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15ac9-245">Request</span></span>
<span data-ttu-id="15ac9-246">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15ac9-246">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="15ac9-247">Antwort</span><span class="sxs-lookup"><span data-stu-id="15ac9-247">Response</span></span>
<span data-ttu-id="15ac9-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15ac9-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
