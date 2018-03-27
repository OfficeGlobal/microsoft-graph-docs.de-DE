# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="d9129-101">Erstellen von windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d9129-101">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="d9129-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d9129-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9129-103">Erstellt neue Objekte des Typs [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-103">Create a new [plannerBucket](../resources/intune_mam_windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9129-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d9129-104">Prerequisites</span></span>
<span data-ttu-id="d9129-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d9129-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9129-107">Permission type</span></span>|<span data-ttu-id="d9129-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9129-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9129-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9129-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d9129-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9129-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9129-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9129-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9129-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9129-112">Not supported.</span></span>|
|<span data-ttu-id="d9129-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9129-113">Application</span></span>|<span data-ttu-id="d9129-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9129-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9129-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9129-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="d9129-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9129-116">Request headers</span></span>
|<span data-ttu-id="d9129-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d9129-117">Header</span></span>|<span data-ttu-id="d9129-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d9129-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9129-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d9129-119">Authorization</span></span>|<span data-ttu-id="d9129-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d9129-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d9129-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d9129-121">Accept</span></span>|<span data-ttu-id="d9129-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d9129-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9129-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9129-123">Request body</span></span>
<span data-ttu-id="d9129-124">Geben Sie als Anforderungstext eine JSON-Darstellung eines Objekts des Typs windowsInformationProtectionPolicy an.</span><span class="sxs-lookup"><span data-stu-id="d9129-124">In the request body, supply a JSON representation of calendar object.</span></span>

<span data-ttu-id="d9129-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs windowsInformationProtectionPolicy erstellen.</span><span class="sxs-lookup"><span data-stu-id="d9129-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d9129-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d9129-126">Property</span></span>|<span data-ttu-id="d9129-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d9129-127">Type</span></span>|<span data-ttu-id="d9129-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9129-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9129-129">displayName</span><span class="sxs-lookup"><span data-stu-id="d9129-129">displayName</span></span>|<span data-ttu-id="d9129-130">String</span><span class="sxs-lookup"><span data-stu-id="d9129-130">String</span></span>|<span data-ttu-id="d9129-131">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d9129-131">Policy display name.</span></span> <span data-ttu-id="d9129-132">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9129-133">description</span><span class="sxs-lookup"><span data-stu-id="d9129-133">description</span></span>|<span data-ttu-id="d9129-134">String</span><span class="sxs-lookup"><span data-stu-id="d9129-134">String</span></span>|<span data-ttu-id="d9129-135">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d9129-135">The policy's description.</span></span> <span data-ttu-id="d9129-136">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9129-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9129-137">createdDateTime</span></span>|<span data-ttu-id="d9129-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9129-138">DateTimeOffset</span></span>|<span data-ttu-id="d9129-139">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d9129-139">The date and time the group was created.</span></span> <span data-ttu-id="d9129-140">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9129-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9129-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d9129-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9129-142">DateTimeOffset</span></span>|<span data-ttu-id="d9129-143">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d9129-143">Last time the policy was modified.</span></span> <span data-ttu-id="d9129-144">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9129-145">id</span><span class="sxs-lookup"><span data-stu-id="d9129-145">id</span></span>|<span data-ttu-id="d9129-146">String</span><span class="sxs-lookup"><span data-stu-id="d9129-146">String</span></span>|<span data-ttu-id="d9129-147">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d9129-147">Key of the setting.</span></span> <span data-ttu-id="d9129-148">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9129-149">Version</span><span class="sxs-lookup"><span data-stu-id="d9129-149">version</span></span>|<span data-ttu-id="d9129-150">String</span><span class="sxs-lookup"><span data-stu-id="d9129-150">String</span></span>|<span data-ttu-id="d9129-151">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="d9129-151">Version of the entity.</span></span> <span data-ttu-id="d9129-152">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9129-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="d9129-153">enforcementLevel</span></span>|<span data-ttu-id="d9129-154">String</span><span class="sxs-lookup"><span data-stu-id="d9129-154">String</span></span>|<span data-ttu-id="d9129-155">WIP-Erzwingungsstufe. Die unterstützten Werte finden Sie in der Enum-Definition. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md). Mögliche Werte sind: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt` und `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="d9129-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="d9129-156">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="d9129-156">enterpriseDomain</span></span>|<span data-ttu-id="d9129-157">String</span><span class="sxs-lookup"><span data-stu-id="d9129-157">String</span></span>|<span data-ttu-id="d9129-158">Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-158">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-159">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="d9129-159">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="d9129-160">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d9129-160">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d9129-161">Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-161">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-162">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="d9129-162">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="d9129-163">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9129-163">Boolean</span></span>|<span data-ttu-id="d9129-164">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-164">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-165">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d9129-165">dataRecoveryCertificate</span></span>|[<span data-ttu-id="d9129-166">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d9129-166">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="d9129-167">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="d9129-167">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="d9129-168">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-168">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-169">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="d9129-169">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="d9129-170">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9129-170">Boolean</span></span>|<span data-ttu-id="d9129-171">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="d9129-171">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="d9129-172">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="d9129-172">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="d9129-173">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d9129-173">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="d9129-174">Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-174">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-175">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="d9129-175">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="d9129-176">Guid</span><span class="sxs-lookup"><span data-stu-id="d9129-176">Guid</span></span>|<span data-ttu-id="d9129-177">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="d9129-177">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="d9129-178">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-178">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-179">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="d9129-179">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="d9129-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9129-180">Boolean</span></span>|<span data-ttu-id="d9129-181">Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-181">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-182">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="d9129-182">iconsVisible</span></span>|<span data-ttu-id="d9129-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9129-183">Boolean</span></span>|<span data-ttu-id="d9129-184">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="d9129-184">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="d9129-185">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-185">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-186">protectedApps</span><span class="sxs-lookup"><span data-stu-id="d9129-186">protectedApps</span></span>|<span data-ttu-id="d9129-187">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9129-187">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="d9129-188">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-188">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-189">exemptApps</span><span class="sxs-lookup"><span data-stu-id="d9129-189">exemptApps</span></span>|<span data-ttu-id="d9129-190">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9129-190">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="d9129-191">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="d9129-191">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="d9129-192">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="d9129-192">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="d9129-193">Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-193">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-194">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="d9129-194">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="d9129-195">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d9129-195">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d9129-196">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="d9129-196">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="d9129-197">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-197">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-198">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="d9129-198">enterpriseProxiedDomains</span></span>|<span data-ttu-id="d9129-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d9129-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="d9129-200">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="d9129-200">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="d9129-201">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="d9129-201">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="d9129-202">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="d9129-202">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="d9129-203">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-203">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-204">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="d9129-204">enterpriseIPRanges</span></span>|<span data-ttu-id="d9129-205">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d9129-205">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="d9129-206">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="d9129-206">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="d9129-207">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="d9129-207">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="d9129-208">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-208">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-209">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="d9129-209">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="d9129-210">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9129-210">Boolean</span></span>|<span data-ttu-id="d9129-211">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="d9129-211">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="d9129-212">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-212">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-213">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="d9129-213">enterpriseProxyServers</span></span>|<span data-ttu-id="d9129-214">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d9129-214">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d9129-215">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="d9129-215">This is a list of proxy servers.</span></span> <span data-ttu-id="d9129-216">Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-216">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-217">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="d9129-217">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="d9129-218">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d9129-218">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d9129-219">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="d9129-219">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="d9129-220">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="d9129-220">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="d9129-221">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="d9129-221">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="d9129-222">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="d9129-222">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="d9129-223">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-223">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-224">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="d9129-224">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="d9129-225">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9129-225">Boolean</span></span>|<span data-ttu-id="d9129-226">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="d9129-226">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="d9129-227">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-227">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-228">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="d9129-228">neutralDomainResources</span></span>|<span data-ttu-id="d9129-229">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d9129-229">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d9129-230">Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-230">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-231">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="d9129-231">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="d9129-232">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9129-232">Boolean</span></span>|<span data-ttu-id="d9129-233">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-233">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-234">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="d9129-234">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="d9129-235">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d9129-235">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d9129-236">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-236">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-237">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d9129-237">isAssigned</span></span>|<span data-ttu-id="d9129-238">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9129-238">Boolean</span></span>|<span data-ttu-id="d9129-239">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="d9129-239">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="d9129-240">Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d9129-240">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d9129-241">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="d9129-241">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="d9129-242">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9129-242">Boolean</span></span>|<span data-ttu-id="d9129-243">Neue Eigenschaft in RS2. Dokumentation noch ausstehend.</span><span class="sxs-lookup"><span data-stu-id="d9129-243">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="d9129-244">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="d9129-244">mdmEnrollmentUrl</span></span>|<span data-ttu-id="d9129-245">String</span><span class="sxs-lookup"><span data-stu-id="d9129-245">String</span></span>|<span data-ttu-id="d9129-246">URL zur Registrierung in der MDM-Lösung</span><span class="sxs-lookup"><span data-stu-id="d9129-246">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="d9129-247">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="d9129-247">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="d9129-248">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9129-248">Boolean</span></span>|<span data-ttu-id="d9129-249">Boolescher Wert, der Windows Hello for Business als Methode für die Anmeldung bei Windows festlegt</span><span class="sxs-lookup"><span data-stu-id="d9129-249">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="d9129-250">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d9129-250">pinMinimumLength</span></span>|<span data-ttu-id="d9129-251">Int32</span><span class="sxs-lookup"><span data-stu-id="d9129-251">Int32</span></span>|<span data-ttu-id="d9129-252">Ganze Zahl, die festlegt, wie viele Zeichen die PIN mindestens haben muss.</span><span class="sxs-lookup"><span data-stu-id="d9129-252">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="d9129-253">Der Standardwert ist „4“.</span><span class="sxs-lookup"><span data-stu-id="d9129-253">Default value is 4.</span></span> <span data-ttu-id="d9129-254">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 4.</span><span class="sxs-lookup"><span data-stu-id="d9129-254">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="d9129-255">Die größte Zahl, die Sie konfigurieren können, muss kleiner sein als die Zahl, die Sie für die Richtlinieneinstellung zur Festlegung der PIN-Maximallänge angegeben haben, oder kleiner als 127 (je nachdem, welche Zahl kleiner ist).</span><span class="sxs-lookup"><span data-stu-id="d9129-255">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="d9129-256">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="d9129-256">pinUppercaseLetters</span></span>|<span data-ttu-id="d9129-257">String</span><span class="sxs-lookup"><span data-stu-id="d9129-257">String</span></span>|<span data-ttu-id="d9129-258">Ganzzahlwert, der konfiguriert, ob Großbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d9129-258">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d9129-259">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="d9129-259">Default is NotAllow.</span></span> <span data-ttu-id="d9129-260">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="d9129-260">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="d9129-261">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="d9129-261">pinLowercaseLetters</span></span>|<span data-ttu-id="d9129-262">String</span><span class="sxs-lookup"><span data-stu-id="d9129-262">String</span></span>|<span data-ttu-id="d9129-263">Ganzzahlwert, der konfiguriert, ob Kleinbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d9129-263">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d9129-264">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="d9129-264">Default is NotAllow.</span></span> <span data-ttu-id="d9129-265">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="d9129-265">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="d9129-266">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="d9129-266">pinSpecialCharacters</span></span>|<span data-ttu-id="d9129-267">String</span><span class="sxs-lookup"><span data-stu-id="d9129-267">String</span></span>|<span data-ttu-id="d9129-268">Ganzzahlwert, der konfiguriert, ob Sonderzeichen in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d9129-268">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d9129-269">Zu den zulässigen Sonderzeichen für Windows Hello for Business-Gesten gehören: !</span><span class="sxs-lookup"><span data-stu-id="d9129-269">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="d9129-270">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="d9129-270">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="d9129-271">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="d9129-271">/ : ; < = > ?</span></span><span data-ttu-id="d9129-272"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="d9129-272"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="d9129-273">} ~.</span><span class="sxs-lookup"><span data-stu-id="d9129-273">=, ==</span></span> <span data-ttu-id="d9129-274">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="d9129-274">Default is NotAllow.</span></span> <span data-ttu-id="d9129-275">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="d9129-275">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="d9129-276">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d9129-276">pinExpirationDays</span></span>|<span data-ttu-id="d9129-277">Int32</span><span class="sxs-lookup"><span data-stu-id="d9129-277">Int32</span></span>|<span data-ttu-id="d9129-278">Ganzzahlwert, der angibt, wie viele Tage die PIN verwendet werden darf, bevor das System den Benutzer auffordert, sie zu ändern.</span><span class="sxs-lookup"><span data-stu-id="d9129-278">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="d9129-279">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 730.</span><span class="sxs-lookup"><span data-stu-id="d9129-279">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="d9129-280">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="d9129-280">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="d9129-281">Wenn Sie für diese Richtlinie „0“ festlegen, läuft die PIN des Benutzers niemals ab.</span><span class="sxs-lookup"><span data-stu-id="d9129-281">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="d9129-282">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d9129-282">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="d9129-283">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="d9129-283">Default is 0.</span></span>|
|<span data-ttu-id="d9129-284">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="d9129-284">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="d9129-285">Int32</span><span class="sxs-lookup"><span data-stu-id="d9129-285">Int32</span></span>|<span data-ttu-id="d9129-286">Ganzzahlwert, der angibt, wie viele der zuletzt dem Benutzerkonto zugeordneten PINs nicht wiederverwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d9129-286">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="d9129-287">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 50.</span><span class="sxs-lookup"><span data-stu-id="d9129-287">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="d9129-288">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="d9129-288">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="d9129-289">Wenn Sie für diese Richtlinie „0“ festlegen, wird keine Speicherung früherer PINs erzwungen.</span><span class="sxs-lookup"><span data-stu-id="d9129-289">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="d9129-290">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d9129-290">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="d9129-291">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="d9129-291">Default is 0.</span></span>|
|<span data-ttu-id="d9129-292">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="d9129-292">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="d9129-293">Int32</span><span class="sxs-lookup"><span data-stu-id="d9129-293">Int32</span></span>|<span data-ttu-id="d9129-294">Legt fest, wie oft die Authentifizierung fehlschlagen darf, bevor das Gerät zurückgesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="d9129-294">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="d9129-295">Ein Wert von „0“ deaktiviert die Funktion zur Gerätezurücksetzung.</span><span class="sxs-lookup"><span data-stu-id="d9129-295">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="d9129-296">Gültig sind Ganzzahlen X, wobei gilt 4 <= X <= 16 für Desktops und 0 <= X <= 999 für Mobilgeräte.</span><span class="sxs-lookup"><span data-stu-id="d9129-296">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="d9129-297">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="d9129-297">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="d9129-298">Int32</span><span class="sxs-lookup"><span data-stu-id="d9129-298">Int32</span></span>|<span data-ttu-id="d9129-299">Gibt an, wie viele Minuten sich das Gerät maximal im Leerlauf befinden darf, bevor eine PIN- oder Kennwortsperre aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="d9129-299">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="d9129-300">Gültig sind Ganzzahlen X, wobei gilt 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="d9129-300">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="d9129-301">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="d9129-301">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="d9129-302">Int32</span><span class="sxs-lookup"><span data-stu-id="d9129-302">Int32</span></span>|<span data-ttu-id="d9129-303">Offline-Intervall (in Tagen), nach dem die App-Daten gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="d9129-303">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="d9129-304">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9129-304">Response</span></span>
<span data-ttu-id="d9129-305">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d9129-305">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9129-306">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9129-306">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9129-307">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9129-307">Request</span></span>
<span data-ttu-id="d9129-308">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9129-308">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4466

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
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

### <a name="response"></a><span data-ttu-id="d9129-309">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9129-309">Response</span></span>
<span data-ttu-id="d9129-p130">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9129-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4574

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
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
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



