# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="bfa24-101">windowsInformationProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bfa24-101">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="bfa24-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bfa24-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfa24-103">Richtlinie für Windows Information Protection zum Konfigurieren detaillierter Verwaltungseinstellungen</span><span class="sxs-lookup"><span data-stu-id="bfa24-103">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="bfa24-104">Erbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bfa24-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bfa24-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="bfa24-105">Methods</span></span>
|<span data-ttu-id="bfa24-106">Methode</span><span class="sxs-lookup"><span data-stu-id="bfa24-106">Method</span></span>|<span data-ttu-id="bfa24-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bfa24-107">Return Type</span></span>|<span data-ttu-id="bfa24-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfa24-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bfa24-109">windowsInformationProtections auflisten</span><span class="sxs-lookup"><span data-stu-id="bfa24-109">List windowsInformationProtections</span></span>](../api/intune_mam_windowsinformationprotection_list.md)|<span data-ttu-id="bfa24-110">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-110">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="bfa24-111">Listet die Eigenschaften und Beziehungen der [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)-Objekte auf.</span><span class="sxs-lookup"><span data-stu-id="bfa24-111">List properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="bfa24-112">windowsInformationProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="bfa24-112">Get windowsInformationProtection</span></span>](../api/intune_mam_windowsinformationprotection_get.md)|[<span data-ttu-id="bfa24-113">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="bfa24-113">windowsInformationProtection</span></span>](../resources/intune_mam_windowsinformationprotection.md)|<span data-ttu-id="bfa24-114">Liest die Eigenschaften und Beziehungen des [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)-Objekts auf.</span><span class="sxs-lookup"><span data-stu-id="bfa24-114">Read properties and relationships of [plannerPlanDetails](../resources/intune_mam_windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="bfa24-115">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="bfa24-115">assign action</span></span>](../api/intune_mam_windowsinformationprotection_assign.md)|<span data-ttu-id="bfa24-116">Keine</span><span class="sxs-lookup"><span data-stu-id="bfa24-116">None</span></span>|<span data-ttu-id="bfa24-117">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="bfa24-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bfa24-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bfa24-118">Properties</span></span>
|<span data-ttu-id="bfa24-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bfa24-119">Property</span></span>|<span data-ttu-id="bfa24-120">Typ</span><span class="sxs-lookup"><span data-stu-id="bfa24-120">Type</span></span>|<span data-ttu-id="bfa24-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfa24-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfa24-122">displayName</span><span class="sxs-lookup"><span data-stu-id="bfa24-122">displayName</span></span>|<span data-ttu-id="bfa24-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bfa24-123">String</span></span>|<span data-ttu-id="bfa24-124">Anzeigename der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="bfa24-124">Policy display name.</span></span> <span data-ttu-id="bfa24-125">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bfa24-125">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bfa24-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfa24-126">description</span></span>|<span data-ttu-id="bfa24-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bfa24-127">String</span></span>|<span data-ttu-id="bfa24-128">Beschreibung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="bfa24-128">The policy's description.</span></span> <span data-ttu-id="bfa24-129">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bfa24-129">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bfa24-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bfa24-130">createdDateTime</span></span>|<span data-ttu-id="bfa24-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfa24-131">DateTimeOffset</span></span>|<span data-ttu-id="bfa24-132">Datum und Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="bfa24-132">The date and time the group was created.</span></span> <span data-ttu-id="bfa24-133">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bfa24-133">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bfa24-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfa24-134">lastModifiedDateTime</span></span>|<span data-ttu-id="bfa24-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfa24-135">DateTimeOffset</span></span>|<span data-ttu-id="bfa24-136">Datum und Uhrzeit der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="bfa24-136">Last time the policy was modified.</span></span> <span data-ttu-id="bfa24-137">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bfa24-137">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bfa24-138">id</span><span class="sxs-lookup"><span data-stu-id="bfa24-138">id</span></span>|<span data-ttu-id="bfa24-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bfa24-139">String</span></span>|<span data-ttu-id="bfa24-140">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="bfa24-140">Key of the setting.</span></span> <span data-ttu-id="bfa24-141">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bfa24-141">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bfa24-142">Version</span><span class="sxs-lookup"><span data-stu-id="bfa24-142">version</span></span>|<span data-ttu-id="bfa24-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bfa24-143">String</span></span>|<span data-ttu-id="bfa24-144">Version der Entität.</span><span class="sxs-lookup"><span data-stu-id="bfa24-144">Version of the entity.</span></span> <span data-ttu-id="bfa24-145">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bfa24-145">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bfa24-146">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="bfa24-146">enforcementLevel</span></span>|<span data-ttu-id="bfa24-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bfa24-147">String</span></span>|<span data-ttu-id="bfa24-148">WIP-Erzwingungsstufe. Die unterstützten Werte finden Sie in der Enum-Definition. Mögliche Werte sind: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="bfa24-148">WIP enforcement level.See the Enum definition for supported values Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="bfa24-149">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="bfa24-149">enterpriseDomain</span></span>|<span data-ttu-id="bfa24-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bfa24-150">String</span></span>|<span data-ttu-id="bfa24-151">Primäre Unternehmensdomäne</span><span class="sxs-lookup"><span data-stu-id="bfa24-151">Primary enterprise domain</span></span>|
|<span data-ttu-id="bfa24-152">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="bfa24-152">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="bfa24-153">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-153">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bfa24-154">Liste von Unternehmensdomänen, die geschützt werden sollen</span><span class="sxs-lookup"><span data-stu-id="bfa24-154">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="bfa24-155">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="bfa24-155">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="bfa24-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bfa24-156">Boolean</span></span>|<span data-ttu-id="bfa24-157">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss.</span><span class="sxs-lookup"><span data-stu-id="bfa24-157">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="bfa24-158">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="bfa24-158">dataRecoveryCertificate</span></span>|[<span data-ttu-id="bfa24-159">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="bfa24-159">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="bfa24-160">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="bfa24-160">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="bfa24-161">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem).</span><span class="sxs-lookup"><span data-stu-id="bfa24-161">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="bfa24-162">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="bfa24-162">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="bfa24-163">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bfa24-163">Boolean</span></span>|<span data-ttu-id="bfa24-164">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="bfa24-164">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="bfa24-165">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="bfa24-165">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="bfa24-166">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="bfa24-166">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="bfa24-167">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="bfa24-167">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="bfa24-168">Guid</span><span class="sxs-lookup"><span data-stu-id="bfa24-168">Guid</span></span>|<span data-ttu-id="bfa24-169">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="bfa24-169">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="bfa24-170">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind.</span><span class="sxs-lookup"><span data-stu-id="bfa24-170">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="bfa24-171">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="bfa24-171">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="bfa24-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bfa24-172">Boolean</span></span>|<span data-ttu-id="bfa24-173">Gibt an, ob Azure RMS-Verschlüsselung für WIP zugelassen werden soll.</span><span class="sxs-lookup"><span data-stu-id="bfa24-173">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="bfa24-174">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="bfa24-174">iconsVisible</span></span>|<span data-ttu-id="bfa24-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bfa24-175">Boolean</span></span>|<span data-ttu-id="bfa24-176">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="bfa24-176">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="bfa24-177">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps.</span><span class="sxs-lookup"><span data-stu-id="bfa24-177">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="bfa24-178">protectedApps</span><span class="sxs-lookup"><span data-stu-id="bfa24-178">protectedApps</span></span>|<span data-ttu-id="bfa24-179">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-179">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="bfa24-180">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt.</span><span class="sxs-lookup"><span data-stu-id="bfa24-180">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="bfa24-181">exemptApps</span><span class="sxs-lookup"><span data-stu-id="bfa24-181">exemptApps</span></span>|<span data-ttu-id="bfa24-182">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-182">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="bfa24-183">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="bfa24-183">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="bfa24-184">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="bfa24-184">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="bfa24-185">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="bfa24-185">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="bfa24-186">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-186">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bfa24-187">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="bfa24-187">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="bfa24-188">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet.</span><span class="sxs-lookup"><span data-stu-id="bfa24-188">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="bfa24-189">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="bfa24-189">enterpriseProxiedDomains</span></span>|<span data-ttu-id="bfa24-190">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-190">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="bfa24-191">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="bfa24-191">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="bfa24-192">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="bfa24-192">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="bfa24-193">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="bfa24-193">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="bfa24-194">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein.</span><span class="sxs-lookup"><span data-stu-id="bfa24-194">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="bfa24-195">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="bfa24-195">enterpriseIPRanges</span></span>|<span data-ttu-id="bfa24-196">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-196">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="bfa24-197">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="bfa24-197">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="bfa24-198">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="bfa24-198">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="bfa24-199">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="bfa24-199">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="bfa24-200">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="bfa24-200">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="bfa24-201">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bfa24-201">Boolean</span></span>|<span data-ttu-id="bfa24-202">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="bfa24-202">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="bfa24-203">Der Standardwert ist „FALSE“.</span><span class="sxs-lookup"><span data-stu-id="bfa24-203">Default is false</span></span>|
|<span data-ttu-id="bfa24-204">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="bfa24-204">enterpriseProxyServers</span></span>|<span data-ttu-id="bfa24-205">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-205">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bfa24-206">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="bfa24-206">This is a list of proxy servers.</span></span> <span data-ttu-id="bfa24-207">Ein Server, der sich nicht in dieser Liste befindet, wird als unternehmensfremd betrachtet.</span><span class="sxs-lookup"><span data-stu-id="bfa24-207">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="bfa24-208">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="bfa24-208">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="bfa24-209">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-209">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bfa24-210">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="bfa24-210">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="bfa24-211">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="bfa24-211">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="bfa24-212">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="bfa24-212">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="bfa24-213">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="bfa24-213">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="bfa24-214">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="bfa24-214">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="bfa24-215">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="bfa24-215">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="bfa24-216">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bfa24-216">Boolean</span></span>|<span data-ttu-id="bfa24-217">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="bfa24-217">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="bfa24-218">Der Standardwert ist „FALSE“.</span><span class="sxs-lookup"><span data-stu-id="bfa24-218">Default is false</span></span>|
|<span data-ttu-id="bfa24-219">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="bfa24-219">neutralDomainResources</span></span>|<span data-ttu-id="bfa24-220">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-220">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bfa24-221">Liste von Domänennamen, die für geschäftliche oder persönliche Ressourcen verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="bfa24-221">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="bfa24-222">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="bfa24-222">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="bfa24-223">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bfa24-223">Boolean</span></span>|<span data-ttu-id="bfa24-224">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="bfa24-224">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="bfa24-225">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="bfa24-225">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="bfa24-226">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-226">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="bfa24-227">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="bfa24-227">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="bfa24-228">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bfa24-228">isAssigned</span></span>|<span data-ttu-id="bfa24-229">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bfa24-229">Boolean</span></span>|<span data-ttu-id="bfa24-230">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="bfa24-230">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfa24-231">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bfa24-231">Relationships</span></span>
|<span data-ttu-id="bfa24-232">Beziehung</span><span class="sxs-lookup"><span data-stu-id="bfa24-232">Relationship</span></span>|<span data-ttu-id="bfa24-233">Typ</span><span class="sxs-lookup"><span data-stu-id="bfa24-233">Type</span></span>|<span data-ttu-id="bfa24-234">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfa24-234">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfa24-235">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="bfa24-235">protectedAppLockerFiles</span></span>|<span data-ttu-id="bfa24-236">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-236">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="bfa24-237">Eine weitere Möglichkeit zur Eingabe geschützter Apps über XML-Dateien.</span><span class="sxs-lookup"><span data-stu-id="bfa24-237">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="bfa24-238">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="bfa24-238">exemptAppLockerFiles</span></span>|<span data-ttu-id="bfa24-239">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-239">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="bfa24-240">Eine weitere Möglichkeit zur Eingabe ausgenommener Apps über XML-Dateien.</span><span class="sxs-lookup"><span data-stu-id="bfa24-240">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="bfa24-241">Zuweisungen</span><span class="sxs-lookup"><span data-stu-id="bfa24-241">assignments</span></span>|<span data-ttu-id="bfa24-242">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bfa24-242">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="bfa24-243">Navigationseigenschaft zu einer Liste der Sicherheitsgruppen, für die die Richtlinie gilt.</span><span class="sxs-lookup"><span data-stu-id="bfa24-243">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfa24-244">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bfa24-244">JSON Representation</span></span>
<span data-ttu-id="bfa24-245">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bfa24-245">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true
}
```



