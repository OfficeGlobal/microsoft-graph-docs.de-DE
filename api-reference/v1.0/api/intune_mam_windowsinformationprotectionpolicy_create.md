# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="d10dc-101">Erstellen von windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d10dc-101">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="d10dc-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d10dc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d10dc-103">Erstellt neue Objekte des Typs [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-103">Create a new [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d10dc-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d10dc-104">Prerequisites</span></span>
<span data-ttu-id="d10dc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d10dc-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d10dc-107">Permission type</span></span>|<span data-ttu-id="d10dc-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d10dc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d10dc-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d10dc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d10dc-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d10dc-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d10dc-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d10dc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d10dc-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d10dc-112">Not supported.</span></span>|
|<span data-ttu-id="d10dc-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d10dc-113">Application</span></span>|<span data-ttu-id="d10dc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d10dc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d10dc-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d10dc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="d10dc-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d10dc-116">Request headers</span></span>
|<span data-ttu-id="d10dc-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d10dc-117">Header</span></span>|<span data-ttu-id="d10dc-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d10dc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d10dc-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d10dc-119">Authorization</span></span>|<span data-ttu-id="d10dc-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d10dc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d10dc-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d10dc-121">Accept</span></span>|<span data-ttu-id="d10dc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d10dc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d10dc-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d10dc-123">Request body</span></span>
<span data-ttu-id="d10dc-124">Geben Sie als Anforderungstext eine JSON-Darstellung eines Objekts des Typs windowsInformationProtectionPolicy an.</span><span class="sxs-lookup"><span data-stu-id="d10dc-124">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="d10dc-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs windowsInformationProtectionPolicy erstellen.</span><span class="sxs-lookup"><span data-stu-id="d10dc-125">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="d10dc-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d10dc-126">Property</span></span>|<span data-ttu-id="d10dc-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d10dc-127">Type</span></span>|<span data-ttu-id="d10dc-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d10dc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d10dc-129">displayName</span><span class="sxs-lookup"><span data-stu-id="d10dc-129">displayName</span></span>|<span data-ttu-id="d10dc-130">String</span><span class="sxs-lookup"><span data-stu-id="d10dc-130">String</span></span>|<span data-ttu-id="d10dc-131">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d10dc-131">Policy display name.</span></span> <span data-ttu-id="d10dc-132">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d10dc-133">description</span><span class="sxs-lookup"><span data-stu-id="d10dc-133">description</span></span>|<span data-ttu-id="d10dc-134">String</span><span class="sxs-lookup"><span data-stu-id="d10dc-134">String</span></span>|<span data-ttu-id="d10dc-135">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d10dc-135">The policy's description.</span></span> <span data-ttu-id="d10dc-136">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d10dc-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d10dc-137">createdDateTime</span></span>|<span data-ttu-id="d10dc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d10dc-138">DateTimeOffset</span></span>|<span data-ttu-id="d10dc-139">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d10dc-139">The date and time the policy was created.</span></span> <span data-ttu-id="d10dc-140">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d10dc-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d10dc-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d10dc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d10dc-142">DateTimeOffset</span></span>|<span data-ttu-id="d10dc-143">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d10dc-143">Last time the policy was modified.</span></span> <span data-ttu-id="d10dc-144">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d10dc-145">id</span><span class="sxs-lookup"><span data-stu-id="d10dc-145">id</span></span>|<span data-ttu-id="d10dc-146">String</span><span class="sxs-lookup"><span data-stu-id="d10dc-146">String</span></span>|<span data-ttu-id="d10dc-147">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d10dc-147">Key of the entity.</span></span> <span data-ttu-id="d10dc-148">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d10dc-149">Version</span><span class="sxs-lookup"><span data-stu-id="d10dc-149">version</span></span>|<span data-ttu-id="d10dc-150">String</span><span class="sxs-lookup"><span data-stu-id="d10dc-150">String</span></span>|<span data-ttu-id="d10dc-151">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="d10dc-151">Version of the entity.</span></span> <span data-ttu-id="d10dc-152">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d10dc-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="d10dc-153">enforcementLevel</span></span>|[<span data-ttu-id="d10dc-154">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="d10dc-154">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="d10dc-155">WIP Erzwingung-Ebene. Siehe die Enum-Definition für unterstützte Werte Inherited aus [WindowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span></span> <span data-ttu-id="d10dc-156">Mögliche Werte: sind `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt` und `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="d10dc-156">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="d10dc-157">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="d10dc-157">enterpriseDomain</span></span>|<span data-ttu-id="d10dc-158">String</span><span class="sxs-lookup"><span data-stu-id="d10dc-158">String</span></span>|<span data-ttu-id="d10dc-159">Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-159">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-160">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="d10dc-160">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="d10dc-161">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d10dc-161">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d10dc-162">Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-162">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-163">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="d10dc-163">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="d10dc-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d10dc-164">Boolean</span></span>|<span data-ttu-id="d10dc-165">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-165">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-166">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d10dc-166">dataRecoveryCertificate</span></span>|[<span data-ttu-id="d10dc-167">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d10dc-167">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="d10dc-168">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="d10dc-168">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="d10dc-169">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-169">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-170">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="d10dc-170">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="d10dc-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d10dc-171">Boolean</span></span>|<span data-ttu-id="d10dc-172">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="d10dc-172">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="d10dc-173">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="d10dc-173">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="d10dc-174">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d10dc-174">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="d10dc-175">Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-175">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-176">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="d10dc-176">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="d10dc-177">Guid</span><span class="sxs-lookup"><span data-stu-id="d10dc-177">Guid</span></span>|<span data-ttu-id="d10dc-178">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="d10dc-178">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="d10dc-179">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-179">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-180">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="d10dc-180">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="d10dc-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d10dc-181">Boolean</span></span>|<span data-ttu-id="d10dc-182">Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-182">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-183">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="d10dc-183">iconsVisible</span></span>|<span data-ttu-id="d10dc-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d10dc-184">Boolean</span></span>|<span data-ttu-id="d10dc-185">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="d10dc-185">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="d10dc-186">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-186">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-187">protectedApps</span><span class="sxs-lookup"><span data-stu-id="d10dc-187">protectedApps</span></span>|<span data-ttu-id="d10dc-188">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d10dc-188">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="d10dc-189">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-189">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-190">exemptApps</span><span class="sxs-lookup"><span data-stu-id="d10dc-190">exemptApps</span></span>|<span data-ttu-id="d10dc-191">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d10dc-191">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="d10dc-192">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="d10dc-192">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="d10dc-193">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="d10dc-193">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="d10dc-194">Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-194">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-195">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="d10dc-195">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="d10dc-196">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d10dc-196">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d10dc-197">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="d10dc-197">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="d10dc-198">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-198">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-199">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="d10dc-199">enterpriseProxiedDomains</span></span>|<span data-ttu-id="d10dc-200">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d10dc-200">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="d10dc-201">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="d10dc-201">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="d10dc-202">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="d10dc-202">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="d10dc-203">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="d10dc-203">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="d10dc-204">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-204">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-205">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="d10dc-205">enterpriseIPRanges</span></span>|<span data-ttu-id="d10dc-206">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d10dc-206">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="d10dc-207">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="d10dc-207">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="d10dc-208">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="d10dc-208">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="d10dc-209">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-209">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-210">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="d10dc-210">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="d10dc-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d10dc-211">Boolean</span></span>|<span data-ttu-id="d10dc-212">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="d10dc-212">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="d10dc-213">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-213">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-214">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="d10dc-214">enterpriseProxyServers</span></span>|<span data-ttu-id="d10dc-215">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d10dc-215">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d10dc-216">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="d10dc-216">This is a list of proxy servers.</span></span> <span data-ttu-id="d10dc-217">Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-217">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-218">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="d10dc-218">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="d10dc-219">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d10dc-219">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d10dc-220">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="d10dc-220">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="d10dc-221">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="d10dc-221">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="d10dc-222">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="d10dc-222">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="d10dc-223">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="d10dc-223">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="d10dc-224">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-224">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-225">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="d10dc-225">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="d10dc-226">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d10dc-226">Boolean</span></span>|<span data-ttu-id="d10dc-227">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="d10dc-227">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="d10dc-228">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-228">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-229">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="d10dc-229">neutralDomainResources</span></span>|<span data-ttu-id="d10dc-230">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d10dc-230">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d10dc-231">Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-231">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-232">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="d10dc-232">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="d10dc-233">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d10dc-233">Boolean</span></span>|<span data-ttu-id="d10dc-234">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-234">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-235">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="d10dc-235">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="d10dc-236">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d10dc-236">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d10dc-237">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-237">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-238">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d10dc-238">isAssigned</span></span>|<span data-ttu-id="d10dc-239">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d10dc-239">Boolean</span></span>|<span data-ttu-id="d10dc-240">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="d10dc-240">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="d10dc-241">Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d10dc-241">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d10dc-242">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="d10dc-242">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="d10dc-243">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d10dc-243">Boolean</span></span>|<span data-ttu-id="d10dc-244">Neue Eigenschaft in RS2. Dokumentation noch ausstehend.</span><span class="sxs-lookup"><span data-stu-id="d10dc-244">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="d10dc-245">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="d10dc-245">mdmEnrollmentUrl</span></span>|<span data-ttu-id="d10dc-246">String</span><span class="sxs-lookup"><span data-stu-id="d10dc-246">String</span></span>|<span data-ttu-id="d10dc-247">URL zur Registrierung in der MDM-Lösung</span><span class="sxs-lookup"><span data-stu-id="d10dc-247">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="d10dc-248">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="d10dc-248">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="d10dc-249">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d10dc-249">Boolean</span></span>|<span data-ttu-id="d10dc-250">Boolescher Wert, der Windows Hello for Business als Methode für die Anmeldung bei Windows festlegt</span><span class="sxs-lookup"><span data-stu-id="d10dc-250">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="d10dc-251">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d10dc-251">pinMinimumLength</span></span>|<span data-ttu-id="d10dc-252">Int32</span><span class="sxs-lookup"><span data-stu-id="d10dc-252">Int32</span></span>|<span data-ttu-id="d10dc-253">Ganze Zahl, die festlegt, wie viele Zeichen die PIN mindestens haben muss.</span><span class="sxs-lookup"><span data-stu-id="d10dc-253">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="d10dc-254">Der Standardwert ist „4“.</span><span class="sxs-lookup"><span data-stu-id="d10dc-254">Default value is 4.</span></span> <span data-ttu-id="d10dc-255">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 4.</span><span class="sxs-lookup"><span data-stu-id="d10dc-255">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="d10dc-256">Die größte Zahl, die Sie konfigurieren können, muss kleiner sein als die Zahl, die Sie für die Richtlinieneinstellung zur Festlegung der PIN-Maximallänge angegeben haben, oder kleiner als 127 (je nachdem, welche Zahl kleiner ist).</span><span class="sxs-lookup"><span data-stu-id="d10dc-256">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="d10dc-257">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="d10dc-257">pinUppercaseLetters</span></span>|[<span data-ttu-id="d10dc-258">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="d10dc-258">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune_mam_windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="d10dc-259">Ganzzahlwert, der konfiguriert, ob Großbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d10dc-259">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d10dc-260">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="d10dc-260">Default is NotAllow.</span></span> <span data-ttu-id="d10dc-261">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="d10dc-261">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="d10dc-262">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="d10dc-262">pinLowercaseLetters</span></span>|[<span data-ttu-id="d10dc-263">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="d10dc-263">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune_mam_windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="d10dc-264">Ganzzahlwert, der konfiguriert, ob Kleinbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d10dc-264">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d10dc-265">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="d10dc-265">Default is NotAllow.</span></span> <span data-ttu-id="d10dc-266">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="d10dc-266">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="d10dc-267">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="d10dc-267">pinSpecialCharacters</span></span>|[<span data-ttu-id="d10dc-268">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="d10dc-268">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune_mam_windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="d10dc-269">Ganzzahlwert, der konfiguriert, ob Sonderzeichen in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d10dc-269">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d10dc-270">Zu den zulässigen Sonderzeichen für Windows Hello for Business-Gesten gehören: !</span><span class="sxs-lookup"><span data-stu-id="d10dc-270">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="d10dc-271">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="d10dc-271">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="d10dc-272">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="d10dc-272">/ : ; < = > ?</span></span><span data-ttu-id="d10dc-273"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="d10dc-273"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="d10dc-274">} ~.</span><span class="sxs-lookup"><span data-stu-id="d10dc-274">} ~.</span></span> <span data-ttu-id="d10dc-275">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="d10dc-275">Default is NotAllow.</span></span> <span data-ttu-id="d10dc-276">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="d10dc-276">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="d10dc-277">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d10dc-277">pinExpirationDays</span></span>|<span data-ttu-id="d10dc-278">Int32</span><span class="sxs-lookup"><span data-stu-id="d10dc-278">Int32</span></span>|<span data-ttu-id="d10dc-279">Ganzzahlwert, der angibt, wie viele Tage die PIN verwendet werden darf, bevor das System den Benutzer auffordert, sie zu ändern.</span><span class="sxs-lookup"><span data-stu-id="d10dc-279">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="d10dc-280">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 730.</span><span class="sxs-lookup"><span data-stu-id="d10dc-280">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="d10dc-281">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="d10dc-281">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="d10dc-282">Wenn Sie für diese Richtlinie „0“ festlegen, läuft die PIN des Benutzers niemals ab.</span><span class="sxs-lookup"><span data-stu-id="d10dc-282">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="d10dc-283">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d10dc-283">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="d10dc-284">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="d10dc-284">Default is 0.</span></span>|
|<span data-ttu-id="d10dc-285">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="d10dc-285">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="d10dc-286">Int32</span><span class="sxs-lookup"><span data-stu-id="d10dc-286">Int32</span></span>|<span data-ttu-id="d10dc-287">Ganzzahlwert, der angibt, wie viele der zuletzt dem Benutzerkonto zugeordneten PINs nicht wiederverwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d10dc-287">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="d10dc-288">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 50.</span><span class="sxs-lookup"><span data-stu-id="d10dc-288">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="d10dc-289">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="d10dc-289">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="d10dc-290">Wenn Sie für diese Richtlinie „0“ festlegen, wird keine Speicherung früherer PINs erzwungen.</span><span class="sxs-lookup"><span data-stu-id="d10dc-290">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="d10dc-291">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d10dc-291">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="d10dc-292">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="d10dc-292">Default is 0.</span></span>|
|<span data-ttu-id="d10dc-293">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="d10dc-293">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="d10dc-294">Int32</span><span class="sxs-lookup"><span data-stu-id="d10dc-294">Int32</span></span>|<span data-ttu-id="d10dc-295">Legt fest, wie oft die Authentifizierung fehlschlagen darf, bevor das Gerät zurückgesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="d10dc-295">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="d10dc-296">Ein Wert von „0“ deaktiviert die Funktion zur Gerätezurücksetzung.</span><span class="sxs-lookup"><span data-stu-id="d10dc-296">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="d10dc-297">Gültig sind Ganzzahlen X, wobei gilt 4 <= X <= 16 für Desktops und 0 <= X <= 999 für Mobilgeräte.</span><span class="sxs-lookup"><span data-stu-id="d10dc-297">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="d10dc-298">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="d10dc-298">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="d10dc-299">Int32</span><span class="sxs-lookup"><span data-stu-id="d10dc-299">Int32</span></span>|<span data-ttu-id="d10dc-300">Gibt an, wie viele Minuten sich das Gerät maximal im Leerlauf befinden darf, bevor eine PIN- oder Kennwortsperre aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="d10dc-300">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="d10dc-301">Gültig sind Ganzzahlen X, wobei gilt 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="d10dc-301">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="d10dc-302">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="d10dc-302">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="d10dc-303">Int32</span><span class="sxs-lookup"><span data-stu-id="d10dc-303">Int32</span></span>|<span data-ttu-id="d10dc-304">Offline-Intervall (in Tagen), nach dem die App-Daten gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="d10dc-304">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="d10dc-305">Antwort</span><span class="sxs-lookup"><span data-stu-id="d10dc-305">Response</span></span>
<span data-ttu-id="d10dc-306">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d10dc-306">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d10dc-307">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d10dc-307">Example</span></span>
### <a name="request"></a><span data-ttu-id="d10dc-308">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d10dc-308">Request</span></span>
<span data-ttu-id="d10dc-309">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d10dc-309">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4405

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value",
  "enforcementLevel": "encryptAndAuditOnly",
  "enterpriseDomain": "Enterprise Domain value",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "Subject Name value",
    "description": "Description value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Y2VydGlmaWNhdGU="
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "Display Name value",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "Ip Address Or FQDN value",
          "proxy": "Proxy value"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "Display Name value",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 0,
  "pinUppercaseLetters": "requireAtLeastOne",
  "pinLowercaseLetters": "requireAtLeastOne",
  "pinSpecialCharacters": "requireAtLeastOne",
  "pinExpirationDays": 1,
  "numberOfPastPinsRemembered": 10,
  "passwordMaximumAttemptCount": 11,
  "minutesOfInactivityBeforeDeviceLock": 3,
  "daysWithoutContactBeforeUnenroll": 0
}
```

### <a name="response"></a><span data-ttu-id="d10dc-310">Antwort</span><span class="sxs-lookup"><span data-stu-id="d10dc-310">Response</span></span>
<span data-ttu-id="d10dc-p131">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d10dc-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4577

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "6397be61-be61-6397-61be-976361be9763",
  "version": "Version value",
  "enforcementLevel": "encryptAndAuditOnly",
  "enterpriseDomain": "Enterprise Domain value",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "Subject Name value",
    "description": "Description value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Y2VydGlmaWNhdGU="
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "Display Name value",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "Ip Address Or FQDN value",
          "proxy": "Proxy value"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "Display Name value",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 0,
  "pinUppercaseLetters": "requireAtLeastOne",
  "pinLowercaseLetters": "requireAtLeastOne",
  "pinSpecialCharacters": "requireAtLeastOne",
  "pinExpirationDays": 1,
  "numberOfPastPinsRemembered": 10,
  "passwordMaximumAttemptCount": 11,
  "minutesOfInactivityBeforeDeviceLock": 3,
  "daysWithoutContactBeforeUnenroll": 0
}
```



