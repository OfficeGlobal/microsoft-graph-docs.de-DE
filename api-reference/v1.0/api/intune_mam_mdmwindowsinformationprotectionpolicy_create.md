# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="8c1e0-101">Erstellen von „mdmWindowsInformationProtectionPolicy“</span><span class="sxs-lookup"><span data-stu-id="8c1e0-101">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="8c1e0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c1e0-103">Diese Methode erstellt ein neues Objekt des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-103">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c1e0-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8c1e0-104">Prerequisites</span></span>
<span data-ttu-id="8c1e0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c1e0-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c1e0-107">Permission type</span></span>|<span data-ttu-id="8c1e0-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c1e0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c1e0-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c1e0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8c1e0-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c1e0-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c1e0-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c1e0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c1e0-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c1e0-112">Not supported.</span></span>|
|<span data-ttu-id="8c1e0-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c1e0-113">Application</span></span>|<span data-ttu-id="8c1e0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c1e0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c1e0-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c1e0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="8c1e0-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c1e0-116">Request headers</span></span>
|<span data-ttu-id="8c1e0-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8c1e0-117">Header</span></span>|<span data-ttu-id="8c1e0-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8c1e0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c1e0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c1e0-119">Authorization</span></span>|<span data-ttu-id="8c1e0-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8c1e0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c1e0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8c1e0-121">Accept</span></span>|<span data-ttu-id="8c1e0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8c1e0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c1e0-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c1e0-123">Request body</span></span>
<span data-ttu-id="8c1e0-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mdmWindowsInformationProtectionPolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-124">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="8c1e0-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mdmWindowsInformationProtectionPolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-125">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="8c1e0-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c1e0-126">Property</span></span>|<span data-ttu-id="8c1e0-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8c1e0-127">Type</span></span>|<span data-ttu-id="8c1e0-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c1e0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c1e0-129">displayName</span><span class="sxs-lookup"><span data-stu-id="8c1e0-129">displayName</span></span>|<span data-ttu-id="8c1e0-130">String</span><span class="sxs-lookup"><span data-stu-id="8c1e0-130">String</span></span>|<span data-ttu-id="8c1e0-131">Anzeigename der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-131">Policy display name.</span></span> <span data-ttu-id="8c1e0-132">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c1e0-133">description</span><span class="sxs-lookup"><span data-stu-id="8c1e0-133">description</span></span>|<span data-ttu-id="8c1e0-134">String</span><span class="sxs-lookup"><span data-stu-id="8c1e0-134">String</span></span>|<span data-ttu-id="8c1e0-135">Beschreibung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-135">The policy's description.</span></span> <span data-ttu-id="8c1e0-136">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c1e0-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c1e0-137">createdDateTime</span></span>|<span data-ttu-id="8c1e0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c1e0-138">DateTimeOffset</span></span>|<span data-ttu-id="8c1e0-139">Datum und Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-139">The date and time the policy was created.</span></span> <span data-ttu-id="8c1e0-140">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c1e0-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c1e0-141">lastModifiedDateTime</span></span>|<span data-ttu-id="8c1e0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c1e0-142">DateTimeOffset</span></span>|<span data-ttu-id="8c1e0-143">Datum und Uhrzeit der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-143">Last time the policy was modified.</span></span> <span data-ttu-id="8c1e0-144">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c1e0-145">id</span><span class="sxs-lookup"><span data-stu-id="8c1e0-145">id</span></span>|<span data-ttu-id="8c1e0-146">String</span><span class="sxs-lookup"><span data-stu-id="8c1e0-146">String</span></span>|<span data-ttu-id="8c1e0-147">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-147">Key of the entity.</span></span> <span data-ttu-id="8c1e0-148">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c1e0-149">version</span><span class="sxs-lookup"><span data-stu-id="8c1e0-149">version</span></span>|<span data-ttu-id="8c1e0-150">String</span><span class="sxs-lookup"><span data-stu-id="8c1e0-150">String</span></span>|<span data-ttu-id="8c1e0-151">Version der Entität.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-151">Version of the entity.</span></span> <span data-ttu-id="8c1e0-152">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c1e0-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="8c1e0-153">enforcementLevel</span></span>|[<span data-ttu-id="8c1e0-154">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="8c1e0-154">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="8c1e0-155">WIP Erzwingung-Ebene. Siehe die Enum-Definition für unterstützte Werte Inherited aus [WindowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span></span> <span data-ttu-id="8c1e0-156">Mögliche Werte: sind `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt` und `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-156">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="8c1e0-157">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="8c1e0-157">enterpriseDomain</span></span>|<span data-ttu-id="8c1e0-158">String</span><span class="sxs-lookup"><span data-stu-id="8c1e0-158">String</span></span>|<span data-ttu-id="8c1e0-159">Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-159">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-160">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="8c1e0-160">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="8c1e0-161">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c1e0-161">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c1e0-162">Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-162">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-163">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="8c1e0-163">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="8c1e0-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8c1e0-164">Boolean</span></span>|<span data-ttu-id="8c1e0-165">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-165">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-166">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8c1e0-166">dataRecoveryCertificate</span></span>|[<span data-ttu-id="8c1e0-167">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8c1e0-167">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="8c1e0-168">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-168">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="8c1e0-169">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-169">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-170">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="8c1e0-170">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="8c1e0-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8c1e0-171">Boolean</span></span>|<span data-ttu-id="8c1e0-172">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-172">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="8c1e0-173">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-173">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="8c1e0-174">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-174">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="8c1e0-175">Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-175">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-176">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="8c1e0-176">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="8c1e0-177">Guid</span><span class="sxs-lookup"><span data-stu-id="8c1e0-177">Guid</span></span>|<span data-ttu-id="8c1e0-178">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-178">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="8c1e0-179">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-179">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-180">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="8c1e0-180">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="8c1e0-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8c1e0-181">Boolean</span></span>|<span data-ttu-id="8c1e0-182">Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-182">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-183">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="8c1e0-183">iconsVisible</span></span>|<span data-ttu-id="8c1e0-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8c1e0-184">Boolean</span></span>|<span data-ttu-id="8c1e0-185">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-185">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="8c1e0-186">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-186">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-187">protectedApps</span><span class="sxs-lookup"><span data-stu-id="8c1e0-187">protectedApps</span></span>|<span data-ttu-id="8c1e0-188">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c1e0-188">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="8c1e0-189">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-189">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-190">exemptApps</span><span class="sxs-lookup"><span data-stu-id="8c1e0-190">exemptApps</span></span>|<span data-ttu-id="8c1e0-191">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c1e0-191">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="8c1e0-192">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-192">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="8c1e0-193">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-193">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="8c1e0-194">Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-194">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-195">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="8c1e0-195">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="8c1e0-196">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c1e0-196">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c1e0-197">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-197">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="8c1e0-198">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-198">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-199">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="8c1e0-199">enterpriseProxiedDomains</span></span>|<span data-ttu-id="8c1e0-200">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8c1e0-200">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="8c1e0-201">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-201">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="8c1e0-202">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-202">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="8c1e0-203">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-203">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="8c1e0-204">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-204">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-205">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="8c1e0-205">enterpriseIPRanges</span></span>|<span data-ttu-id="8c1e0-206">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8c1e0-206">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="8c1e0-207">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-207">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="8c1e0-208">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-208">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="8c1e0-209">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-209">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-210">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="8c1e0-210">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="8c1e0-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8c1e0-211">Boolean</span></span>|<span data-ttu-id="8c1e0-212">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-212">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="8c1e0-213">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-213">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-214">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="8c1e0-214">enterpriseProxyServers</span></span>|<span data-ttu-id="8c1e0-215">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c1e0-215">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c1e0-216">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-216">This is a list of proxy servers.</span></span> <span data-ttu-id="8c1e0-217">Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-217">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-218">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="8c1e0-218">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="8c1e0-219">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c1e0-219">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c1e0-220">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-220">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="8c1e0-221">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-221">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="8c1e0-222">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-222">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="8c1e0-223">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-223">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="8c1e0-224">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-224">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-225">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="8c1e0-225">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="8c1e0-226">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8c1e0-226">Boolean</span></span>|<span data-ttu-id="8c1e0-227">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-227">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="8c1e0-228">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-228">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-229">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="8c1e0-229">neutralDomainResources</span></span>|<span data-ttu-id="8c1e0-230">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c1e0-230">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c1e0-231">Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-231">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-232">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="8c1e0-232">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="8c1e0-233">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8c1e0-233">Boolean</span></span>|<span data-ttu-id="8c1e0-234">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-234">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-235">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="8c1e0-235">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="8c1e0-236">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c1e0-236">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c1e0-237">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-237">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c1e0-238">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8c1e0-238">isAssigned</span></span>|<span data-ttu-id="8c1e0-239">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8c1e0-239">Boolean</span></span>|<span data-ttu-id="8c1e0-240">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-240">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="8c1e0-241">Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c1e0-241">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8c1e0-242">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c1e0-242">Response</span></span>
<span data-ttu-id="8c1e0-243">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-243">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c1e0-244">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c1e0-244">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c1e0-245">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c1e0-245">Request</span></span>
<span data-ttu-id="8c1e0-246">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3905

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="8c1e0-247">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c1e0-247">Response</span></span>
<span data-ttu-id="8c1e0-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c1e0-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4077

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "8efb0c35-0c35-8efb-350c-fb8e350cfb8e",
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
  "isAssigned": true
}
```



