<span data-ttu-id="d32c2-p114">Beziehungen zwischen einer Domäne und anderen Objekten im Verzeichnis, z. B. die Überprüfungsdatensätze und Dienstkonfigurationsdatensätze, die über Navigationseigenschaften verfügbar gemacht werden. Sie können diese Beziehungen lesen, indem Sie auf diese Navigationseigenschaften in Ihren Anforderungen abzielen.</span><span class="sxs-lookup"><span data-stu-id="d32c2-p114">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties. You can read these relationships by targeting these navigation properties in your requests.</span></span>

Beziehungen zwischen einer Domäne und anderen Objekten im Verzeichnis, z. B. die Überprüfungsdatensätze und Dienstkonfigurationsdatensätze, die über Navigationseigenschaften verfügbar gemacht werden. Sie können diese Beziehungen lesen, indem Sie auf diese Navigationseigenschaften in Ihren Anforderungen abzielen.

| <span data-ttu-id="d32c2-199">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d32c2-199">Relationship</span></span> | <span data-ttu-id="d32c2-200">Typ</span><span class="sxs-lookup"><span data-stu-id="d32c2-200">Type</span></span> |<span data-ttu-id="d32c2-201">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d32c2-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d32c2-202">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="d32c2-202">domainNameReferences</span></span>|<span data-ttu-id="d32c2-203">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d32c2-203">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d32c2-204">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="d32c2-204">Read-only, Nullable</span></span>|
|<span data-ttu-id="d32c2-205">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="d32c2-205">serviceConfigurationRecords</span></span>|<span data-ttu-id="d32c2-206">[domainDnsRecord](domaindnsrecord.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d32c2-206">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="d32c2-207">DNS-Einträge, die der Kunde der Zonendatei der Domäne hinzufügt, bevor die Domäne von Microsoft-Onlinediensten verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="d32c2-207">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span><br><span data-ttu-id="d32c2-208">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="d32c2-208">Read-only, Nullable</span></span> |
|<span data-ttu-id="d32c2-209">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="d32c2-209">verificationDnsRecords</span></span>|<span data-ttu-id="d32c2-210">[domainDnsRecord](domaindnsrecord.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d32c2-210">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="d32c2-211">DNS-Einträge, die der Kunde der DNS-Zonendatei der Domäne hinzufügt, bevor die Domänenbesitzüberprüfung mit Azure AD abgeschlossen werden kann.</span><span class="sxs-lookup"><span data-stu-id="d32c2-211">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span><br><span data-ttu-id="d32c2-212">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="d32c2-212">Read-only, Nullable</span></span>|

## <span data-ttu-id="d32c2-213">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d32c2-213">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="d32c2-214">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d32c2-214">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->