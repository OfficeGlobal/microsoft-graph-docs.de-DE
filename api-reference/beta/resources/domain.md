---
title: domain-Ressourcentyp
description: Stellt eine Domäne dar, die einem Mandanten zugewiesen ist.
ms.openlocfilehash: e142998a23f24ff2693f8a70f13c2c8a35432961
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065898"
---
# <a name="domain-resource-type"></a><span data-ttu-id="1fe80-103">domain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1fe80-103">domain resource type</span></span>

> <span data-ttu-id="1fe80-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1fe80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fe80-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fe80-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1fe80-106">Stellt eine Domäne dar, die einem Mandanten zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="1fe80-106">Represents a domain associated with the tenant.</span></span>

<span data-ttu-id="1fe80-p102">Verwenden Sie Domänenvorgänge, um Domänen einem Mandanten zuzuweisen, den Besitz von Domänen zu überprüfen und unterstützte Dienste zu konfigurieren.  Mithilfe von Domänenvorgängen können Registrierungsstellen die Domänenzuweisung für Dienste wie Office 365 automatisieren. Im Rahmen der Domänenanmeldung kann eine Registrierungsstelle beispielsweise eine Vanity-Domäne für E-Mails, Websites, Authentifizierung usw. aktivieren.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p102">Use domain operations to associate domains to a tenant, verify domain ownership, and configure supported services.  Domain operations enable registrars to automate domain association for services such as Office 365. For example, as part of domain sign up, a registrar can enable a vanity domain for email, websites, authentication, etc.</span></span>

<span data-ttu-id="1fe80-110">So ordnen Sie eine Domäne einem Mandanten zu:</span><span class="sxs-lookup"><span data-stu-id="1fe80-110">To associate a domain with a tenant:</span></span>

1. <span data-ttu-id="1fe80-111">[Ordnen Sie](../api/domain-post-domains.md) dem Mandanten eine Domäne zu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-111">[Associate](../api/domain-post-domains.md) a domain with a tenant.</span></span>

2. <span data-ttu-id="1fe80-p103">[Rufen Sie](../api/domain-list-verificationdnsrecords.md) die Domänenüberprüfungseinträge ab. Fügen Sie die Details des Überprüfungsdatensatzes mithilfe der Domänenregistrierungsstelle oder der DNS-Serverkonfiguration der Zonendatei der Domäne hinzu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p103">[Retrieve](../api/domain-list-verificationdnsrecords.md) the domain verification records. Add the verification record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

3. <span data-ttu-id="1fe80-p104">[Überprüfen Sie](../api/domain-verify.md) den Besitz der Domäne. Dadurch wird die Domäne überprüft und die *IsVerified*-Eigenschaft auf *true* festgelegt.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p104">[Verify](../api/domain-verify.md) the ownership of the domain. This will verify the domain and set the *isVerified* property to *true*.</span></span>

4. <span data-ttu-id="1fe80-116">[Geben Sie](../api/domain-update.md) die unterstützten Dienste an, die Sie mit der Domäne verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="1fe80-116">[Indicate](../api/domain-update.md) the supported services you plan to use with the domain.</span></span>

5. <span data-ttu-id="1fe80-p105">[Konfigurieren Sie](../api/domain-list-serviceconfigurationrecords.md) unterstützte Dienste, indem Sie eine Liste von Datensätzen abrufen, die zum Aktivieren von Diensten für die Domäne erforderlich sind. Fügen Sie die Details des Konfigurationsdatensatzes mithilfe der Domänenregistrierungsstelle oder der DNS-Serverkonfiguration der Zonendatei der Domäne hinzu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p105">[Configure](../api/domain-list-serviceconfigurationrecords.md) supported services by retrieving a list of records needed to enable services for the domain. Add the configuration record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="1fe80-119">Methoden</span><span class="sxs-lookup"><span data-stu-id="1fe80-119">Methods</span></span>

| <span data-ttu-id="1fe80-120">Methode</span><span class="sxs-lookup"><span data-stu-id="1fe80-120">Method</span></span>   | <span data-ttu-id="1fe80-121">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1fe80-121">Return Type</span></span> |<span data-ttu-id="1fe80-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1fe80-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1fe80-123">Domäne abrufen</span><span class="sxs-lookup"><span data-stu-id="1fe80-123">Get domain</span></span>](../api/domain-get.md) | [<span data-ttu-id="1fe80-124">Domäne</span><span class="sxs-lookup"><span data-stu-id="1fe80-124">domain</span></span>](domain.md) | <span data-ttu-id="1fe80-125">Dient zum Lesen der Eigenschaften und der Beziehungen eines Domänenobjekts.</span><span class="sxs-lookup"><span data-stu-id="1fe80-125">Read properties and relationships of a domain object.</span></span>|
|[<span data-ttu-id="1fe80-126">Domäne erstellen</span><span class="sxs-lookup"><span data-stu-id="1fe80-126">Create domain</span></span>](../api/domain-post-domains.md) | [<span data-ttu-id="1fe80-127">Domäne</span><span class="sxs-lookup"><span data-stu-id="1fe80-127">domain</span></span>](domain.md) | <span data-ttu-id="1fe80-128">Fügt eine Domäne zum Mandanten hinzu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-128">Adds a domain to the tenant.</span></span> |
|[<span data-ttu-id="1fe80-129">domainNameReference auflisten</span><span class="sxs-lookup"><span data-stu-id="1fe80-129">List domainNameReference</span></span>](../api/domain-list-domainnamereferences.md) |<span data-ttu-id="1fe80-130">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1fe80-130">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1fe80-131">Dient zum Abrufen einer Liste von Verzeichnisobjekten mit einem Verweis auf die Domäne.</span><span class="sxs-lookup"><span data-stu-id="1fe80-131">Retrieve a list of directory objects with a reference to the domain.</span></span>|
|[<span data-ttu-id="1fe80-132">serviceConfigurationRecords auflisten</span><span class="sxs-lookup"><span data-stu-id="1fe80-132">List serviceConfigurationRecords</span></span>](../api/domain-list-serviceconfigurationrecords.md) |<span data-ttu-id="1fe80-133">[domainDnsRecord](domaindnsrecord.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1fe80-133">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="1fe80-134">Dient zum Abrufen einer von Domänen-DNS-Einträgen für die Domänenkonfiguration.</span><span class="sxs-lookup"><span data-stu-id="1fe80-134">Retrieve a list of domain DNS records for domain configuration.</span></span>|
|[<span data-ttu-id="1fe80-135">verificationDnsRecords auflisten</span><span class="sxs-lookup"><span data-stu-id="1fe80-135">List verificationDnsRecords</span></span>](../api/domain-list-verificationdnsrecords.md) |<span data-ttu-id="1fe80-136">[domainDnsRecord](domaindnsrecord.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1fe80-136">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="1fe80-137">Dient zum Abrufen einer von Domänen-DNS-Einträgen für die Domänenüberprüfung.</span><span class="sxs-lookup"><span data-stu-id="1fe80-137">Retrieve a list of domain DNS records for domain verification.</span></span>|
|[<span data-ttu-id="1fe80-138">Domäne aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1fe80-138">Update domain</span></span>](../api/domain-update.md) | [<span data-ttu-id="1fe80-139">Domäne</span><span class="sxs-lookup"><span data-stu-id="1fe80-139">domain</span></span>](domain.md) |<span data-ttu-id="1fe80-140">Dient zum Aktualisieren einer Domäne.</span><span class="sxs-lookup"><span data-stu-id="1fe80-140">Updates a domain.</span></span>|
|[<span data-ttu-id="1fe80-141">Domäne löschen</span><span class="sxs-lookup"><span data-stu-id="1fe80-141">Delete domain</span></span>](../api/domain-delete.md) | <span data-ttu-id="1fe80-142">Keine</span><span class="sxs-lookup"><span data-stu-id="1fe80-142">None</span></span> |<span data-ttu-id="1fe80-143">Dient zum Löschen einer Domäne.</span><span class="sxs-lookup"><span data-stu-id="1fe80-143">Deletes a domain.</span></span>|
|[<span data-ttu-id="1fe80-144">ForceDelete Domäne</span><span class="sxs-lookup"><span data-stu-id="1fe80-144">ForceDelete domain</span></span>](../api/domain-forcedelete.md)|<span data-ttu-id="1fe80-145">Keines</span><span class="sxs-lookup"><span data-stu-id="1fe80-145">None</span></span>|<span data-ttu-id="1fe80-146">Löscht eine Domäne mithilfe eines asynchronen Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="1fe80-146">Deletes a domain using an asynchronous operation.</span></span>|
|[<span data-ttu-id="1fe80-147">Domäne überprüfen</span><span class="sxs-lookup"><span data-stu-id="1fe80-147">Verify domain</span></span>](../api/domain-verify.md)|[<span data-ttu-id="1fe80-148">Domäne</span><span class="sxs-lookup"><span data-stu-id="1fe80-148">domain</span></span>](domain.md)|<span data-ttu-id="1fe80-149">Überprüft den Besitz der Domäne.</span><span class="sxs-lookup"><span data-stu-id="1fe80-149">Validates the ownership of the domain.</span></span>|

## <a name="properties"></a><span data-ttu-id="1fe80-150">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1fe80-150">Properties</span></span>

| <span data-ttu-id="1fe80-151">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1fe80-151">Property</span></span>   | <span data-ttu-id="1fe80-152">Typ</span><span class="sxs-lookup"><span data-stu-id="1fe80-152">Type</span></span> | <span data-ttu-id="1fe80-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1fe80-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1fe80-154">authenticationType</span><span class="sxs-lookup"><span data-stu-id="1fe80-154">authenticationType</span></span>|<span data-ttu-id="1fe80-155">String</span><span class="sxs-lookup"><span data-stu-id="1fe80-155">String</span></span>| <span data-ttu-id="1fe80-p106">Gibt den konfigurierten Authentifizierungstyp für die Domäne an. Der Wert ist entweder *Verwaltet* oder *Verbund*.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p106">Indicates the configured authentication type for the domain. The value is either *Managed* or *Federated*.</span></span><br> <span data-ttu-id="1fe80-158">*Verwaltet* gibt eine cloudverwaltete Domäne an, bei der Azure AD die Benutzerauthentifizierung ausführt.</span><span class="sxs-lookup"><span data-stu-id="1fe80-158">*Managed* indicates a cloud managed domain where Azure AD performs user authentication.</span></span><br><span data-ttu-id="1fe80-p107">*Verbund* gibt an, dass die Authentifizierung im Verbund mit einem Identitätsanbieter steht, z. B. das lokale Active Directory des Mandanten über Active Directory-Verbunddienste. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p107">*Federated* indicates authentication is federated with an identity provider such as the tenant's on-premises Active Directory via Active Directory Federation Services. Not nullable</span></span> |
|<span data-ttu-id="1fe80-161">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="1fe80-161">availabilityStatus</span></span>|<span data-ttu-id="1fe80-162">String</span><span class="sxs-lookup"><span data-stu-id="1fe80-162">String</span></span>| <span data-ttu-id="1fe80-p108">Diese Eigenschaft ist immer null, außer wenn die Aktion [verify](../api/domain-verify.md) verwendet wird. Wenn die Aktion [verify](../api/domain-verify.md) verwendet wird, wird in der Antwort eine **Domänen**entität zurückgegeben. Die Eigenschaft **availabilityStatus** der **Domänen**entität in der Antwort ist entweder *AvailableImmediately* oder *EmailVerifiedDomainTakeoverScheduled*.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p108">This property is always null except when the [verify](../api/domain-verify.md) action is used. When the [verify](../api/domain-verify.md) action is used, a **domain** entity is returned in the response. The **availabilityStatus** property of the **domain** entity in the response is either *AvailableImmediately* or *EmailVerifiedDomainTakeoverScheduled*.</span></span>|
|<span data-ttu-id="1fe80-166">id</span><span class="sxs-lookup"><span data-stu-id="1fe80-166">id</span></span>|<span data-ttu-id="1fe80-167">String</span><span class="sxs-lookup"><span data-stu-id="1fe80-167">String</span></span>| <span data-ttu-id="1fe80-p109">Der vollqualifizierte Name der Domäne. Schlüssel, unveränderlich, lässt keine Nullwerte zu, eindeutig</span><span class="sxs-lookup"><span data-stu-id="1fe80-p109">The fully qualified name of the domain. Key, immutable, not nullable, unique</span></span> |
|<span data-ttu-id="1fe80-170">isAdminManaged</span><span class="sxs-lookup"><span data-stu-id="1fe80-170">isAdminManaged</span></span>|<span data-ttu-id="1fe80-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1fe80-171">Boolean</span></span>| <span data-ttu-id="1fe80-p110">Der Wert der Eigenschaft ist „false“, wenn die DNS-Datensatzverwaltung der Domäne an Office 365 delegiert wurde. Andernfalls ist der Wert „true“. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p110">The value of the property is false if the DNS record management of the domain has been delegated to Office 365. Otherwise, the value is true. Not nullable</span></span> |
|<span data-ttu-id="1fe80-175">isDefault</span><span class="sxs-lookup"><span data-stu-id="1fe80-175">isDefault</span></span>|<span data-ttu-id="1fe80-176">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1fe80-176">Boolean</span></span>| <span data-ttu-id="1fe80-p111">„True“, wenn dies die Standarddomäne ist, die für die Benutzererstellung verwendet wird. Es gibt nur eine Standarddomäne pro Unternehmen. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p111">True if this is the default domain that is used for user creation. There is only one default domain per company. Not nullable</span></span> |
|<span data-ttu-id="1fe80-180">isInitial</span><span class="sxs-lookup"><span data-stu-id="1fe80-180">isInitial</span></span>|<span data-ttu-id="1fe80-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1fe80-181">Boolean</span></span>| <span data-ttu-id="1fe80-p112">„True“, wenn dies die erste Domäne ist, die von Microsoft Online Services (companyname.onmicrosoft.com) erstellt wird. Es gibt nur eine anfängliche Domäne pro Unternehmen. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p112">True if this is the initial domain created by Microsoft Online Services (companyname.onmicrosoft.com). There is only one initial domain per company. Not nullable</span></span> |
|<span data-ttu-id="1fe80-185">isRoot</span><span class="sxs-lookup"><span data-stu-id="1fe80-185">isRoot</span></span>|<span data-ttu-id="1fe80-186">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1fe80-186">Boolean</span></span>| <span data-ttu-id="1fe80-p113">„True“, wenn die Domäne eine überprüfte Stammdomäne ist. Andernfalls „false“, wenn die Domäne eine Unterdomäne oder ungeprüft ist. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p113">True if the domain is a verified root domain. Otherwise, false if the domain is a subdomain or unverified. Not nullable</span></span> |
|<span data-ttu-id="1fe80-190">isVerified</span><span class="sxs-lookup"><span data-stu-id="1fe80-190">isVerified</span></span>|<span data-ttu-id="1fe80-191">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1fe80-191">Boolean</span></span>| <span data-ttu-id="1fe80-p114">„True“, wenn die Domänenbesitzüberprüfung für die Domäne abgeschlossen ist. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p114">True if the domain has completed domain ownership verification. Not nullable</span></span> |
|<span data-ttu-id="1fe80-194">supportedServices</span><span class="sxs-lookup"><span data-stu-id="1fe80-194">supportedServices</span></span>|<span data-ttu-id="1fe80-195">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1fe80-195">String collection</span></span>| <span data-ttu-id="1fe80-196">Die der Domäne zugewiesenen Funktionen.</span><span class="sxs-lookup"><span data-stu-id="1fe80-196">The capabilities assigned to the domain.</span></span><br><br><span data-ttu-id="1fe80-197">Kann 0, 1 oder mehrere der folgenden Werte umfassen: *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="1fe80-197">Can include 0, 1 or more of following values: *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span><br><br> <span data-ttu-id="1fe80-198">Zu den Werten, die Sie mithilfe der Graph-API hinzufügen/entfernen können, gehören: *Email*, *OfficeCommunicationsOnline*, *Yammer*</span><span class="sxs-lookup"><span data-stu-id="1fe80-198">The values which you can add/remove using Graph API include: *Email*, *OfficeCommunicationsOnline*, *Yammer*</span></span><br><span data-ttu-id="1fe80-199">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-199">Not nullable</span></span>|
|<span data-ttu-id="1fe80-200">Status</span><span class="sxs-lookup"><span data-stu-id="1fe80-200">state</span></span>|[<span data-ttu-id="1fe80-201">domainState</span><span class="sxs-lookup"><span data-stu-id="1fe80-201">domainState</span></span>](domainstate.md)| <span data-ttu-id="1fe80-202">Status von asynchronen Vorgängen, die für die Domäne geplant sind.</span><span class="sxs-lookup"><span data-stu-id="1fe80-202">Status of asynchronous operations scheduled for the domain.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1fe80-203">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1fe80-203">Relationships</span></span>

<span data-ttu-id="1fe80-p115">Beziehungen zwischen einer Domäne und anderen Objekten im Verzeichnis, z. B. die Überprüfungsdatensätze und Dienstkonfigurationsdatensätze, die über Navigationseigenschaften verfügbar gemacht werden. Sie können diese Beziehungen lesen, indem Sie auf diese Navigationseigenschaften in Ihren Anforderungen abzielen.</span><span class="sxs-lookup"><span data-stu-id="1fe80-p115">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties. You can read these relationships by targeting these navigation properties in your requests.</span></span>

| <span data-ttu-id="1fe80-206">Beziehung</span><span class="sxs-lookup"><span data-stu-id="1fe80-206">Relationship</span></span> | <span data-ttu-id="1fe80-207">Typ</span><span class="sxs-lookup"><span data-stu-id="1fe80-207">Type</span></span> |<span data-ttu-id="1fe80-208">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1fe80-208">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fe80-209">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="1fe80-209">domainNameReferences</span></span>|<span data-ttu-id="1fe80-210">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1fe80-210">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1fe80-211">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-211">Read-only, Nullable</span></span>|
|<span data-ttu-id="1fe80-212">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="1fe80-212">serviceConfigurationRecords</span></span>|<span data-ttu-id="1fe80-213">[domainDnsRecord](domaindnsrecord.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1fe80-213">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="1fe80-214">DNS-Einträge, die der Kunde der Zonendatei der Domäne hinzufügt, bevor die Domäne von Microsoft-Onlinediensten verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="1fe80-214">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span><br><span data-ttu-id="1fe80-215">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-215">Read-only, Nullable</span></span> |
|<span data-ttu-id="1fe80-216">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="1fe80-216">verificationDnsRecords</span></span>|<span data-ttu-id="1fe80-217">[domainDnsRecord](domaindnsrecord.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1fe80-217">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="1fe80-218">DNS-Einträge, die der Kunde der DNS-Zonendatei der Domäne hinzufügt, bevor die Domänenbesitzüberprüfung mit Azure AD abgeschlossen werden kann.</span><span class="sxs-lookup"><span data-stu-id="1fe80-218">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span><br><span data-ttu-id="1fe80-219">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="1fe80-219">Read-only, Nullable</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fe80-220">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1fe80-220">JSON representation</span></span>
<span data-ttu-id="1fe80-221">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1fe80-221">Here is a JSON representation of the resource.</span></span>

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