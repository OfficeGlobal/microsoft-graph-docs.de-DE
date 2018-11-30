---
title: Erstellen von windowsInformationProtectionPolicy
description: Erstellt neue Objekte des Typs windowsInformationProtectionPolicy.
ms.openlocfilehash: dc13c12fc0174f8dc677f2b319be69502112f707
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017436"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="dc2d4-103">Erstellen von windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="dc2d4-103">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="dc2d4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc2d4-105">Erstellt neue Objekte des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-105">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc2d4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dc2d4-106">Prerequisites</span></span>
<span data-ttu-id="dc2d4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc2d4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dc2d4-109">Permission type</span></span>|<span data-ttu-id="dc2d4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dc2d4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc2d4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dc2d4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc2d4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc2d4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dc2d4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dc2d4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc2d4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc2d4-114">Not supported.</span></span>|
|<span data-ttu-id="dc2d4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dc2d4-115">Application</span></span>|<span data-ttu-id="dc2d4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc2d4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc2d4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc2d4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="dc2d4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dc2d4-118">Request headers</span></span>
|<span data-ttu-id="dc2d4-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dc2d4-119">Header</span></span>|<span data-ttu-id="dc2d4-120">Wert</span><span class="sxs-lookup"><span data-stu-id="dc2d4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc2d4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc2d4-121">Authorization</span></span>|<span data-ttu-id="dc2d4-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dc2d4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc2d4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dc2d4-123">Accept</span></span>|<span data-ttu-id="dc2d4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dc2d4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc2d4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dc2d4-125">Request body</span></span>
<span data-ttu-id="dc2d4-126">Geben Sie als Anforderungstext eine JSON-Darstellung eines Objekts des Typs windowsInformationProtectionPolicy an.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-126">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="dc2d4-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs windowsInformationProtectionPolicy erstellen.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-127">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="dc2d4-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dc2d4-128">Property</span></span>|<span data-ttu-id="dc2d4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="dc2d4-129">Type</span></span>|<span data-ttu-id="dc2d4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dc2d4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc2d4-131">displayName</span><span class="sxs-lookup"><span data-stu-id="dc2d4-131">displayName</span></span>|<span data-ttu-id="dc2d4-132">String</span><span class="sxs-lookup"><span data-stu-id="dc2d4-132">String</span></span>|<span data-ttu-id="dc2d4-133">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="dc2d4-133">Policy display name.</span></span> <span data-ttu-id="dc2d4-134">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dc2d4-135">description</span><span class="sxs-lookup"><span data-stu-id="dc2d4-135">description</span></span>|<span data-ttu-id="dc2d4-136">String</span><span class="sxs-lookup"><span data-stu-id="dc2d4-136">String</span></span>|<span data-ttu-id="dc2d4-137">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="dc2d4-137">The policy's description.</span></span> <span data-ttu-id="dc2d4-138">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dc2d4-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc2d4-139">createdDateTime</span></span>|<span data-ttu-id="dc2d4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc2d4-140">DateTimeOffset</span></span>|<span data-ttu-id="dc2d4-141">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="dc2d4-141">The date and time the policy was created.</span></span> <span data-ttu-id="dc2d4-142">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dc2d4-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc2d4-143">lastModifiedDateTime</span></span>|<span data-ttu-id="dc2d4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc2d4-144">DateTimeOffset</span></span>|<span data-ttu-id="dc2d4-145">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="dc2d4-145">Last time the policy was modified.</span></span> <span data-ttu-id="dc2d4-146">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dc2d4-147">id</span><span class="sxs-lookup"><span data-stu-id="dc2d4-147">id</span></span>|<span data-ttu-id="dc2d4-148">String</span><span class="sxs-lookup"><span data-stu-id="dc2d4-148">String</span></span>|<span data-ttu-id="dc2d4-149">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="dc2d4-149">Key of the entity.</span></span> <span data-ttu-id="dc2d4-150">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dc2d4-151">Version</span><span class="sxs-lookup"><span data-stu-id="dc2d4-151">version</span></span>|<span data-ttu-id="dc2d4-152">String</span><span class="sxs-lookup"><span data-stu-id="dc2d4-152">String</span></span>|<span data-ttu-id="dc2d4-153">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="dc2d4-153">Version of the entity.</span></span> <span data-ttu-id="dc2d4-154">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dc2d4-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="dc2d4-155">enforcementLevel</span></span>|[<span data-ttu-id="dc2d4-156">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="dc2d4-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="dc2d4-157">WIP Erzwingung-Ebene. Siehe die Enum-Definition für unterstützte Werte Inherited aus [WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="dc2d4-158">Mögliche Werte: sind `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt` und `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="dc2d4-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="dc2d4-159">enterpriseDomain</span></span>|<span data-ttu-id="dc2d4-160">String</span><span class="sxs-lookup"><span data-stu-id="dc2d4-160">String</span></span>|<span data-ttu-id="dc2d4-161">Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="dc2d4-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="dc2d4-163">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="dc2d4-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="dc2d4-164">Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="dc2d4-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="dc2d4-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc2d4-166">Boolean</span></span>|<span data-ttu-id="dc2d4-167">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="dc2d4-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="dc2d4-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="dc2d4-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="dc2d4-170">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="dc2d4-171">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="dc2d4-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="dc2d4-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc2d4-173">Boolean</span></span>|<span data-ttu-id="dc2d4-174">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="dc2d4-175">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="dc2d4-176">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="dc2d4-177">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="dc2d4-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="dc2d4-179">Guid</span><span class="sxs-lookup"><span data-stu-id="dc2d4-179">Guid</span></span>|<span data-ttu-id="dc2d4-180">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="dc2d4-181">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="dc2d4-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="dc2d4-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc2d4-183">Boolean</span></span>|<span data-ttu-id="dc2d4-184">Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="dc2d4-185">iconsVisible</span></span>|<span data-ttu-id="dc2d4-186">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc2d4-186">Boolean</span></span>|<span data-ttu-id="dc2d4-187">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="dc2d4-188">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="dc2d4-189">protectedApps</span></span>|<span data-ttu-id="dc2d4-190">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc2d4-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="dc2d4-191">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="dc2d4-192">exemptApps</span></span>|<span data-ttu-id="dc2d4-193">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc2d4-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="dc2d4-194">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="dc2d4-195">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="dc2d4-196">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="dc2d4-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="dc2d4-198">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="dc2d4-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="dc2d4-199">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="dc2d4-200">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="dc2d4-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="dc2d4-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="dc2d4-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="dc2d4-203">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="dc2d4-204">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="dc2d4-205">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="dc2d4-206">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="dc2d4-207">enterpriseIPRanges</span></span>|<span data-ttu-id="dc2d4-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="dc2d4-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="dc2d4-209">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="dc2d4-210">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="dc2d4-211">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="dc2d4-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="dc2d4-213">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc2d4-213">Boolean</span></span>|<span data-ttu-id="dc2d4-214">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="dc2d4-215">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="dc2d4-216">enterpriseProxyServers</span></span>|<span data-ttu-id="dc2d4-217">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="dc2d4-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="dc2d4-218">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-218">This is a list of proxy servers.</span></span> <span data-ttu-id="dc2d4-219">Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="dc2d4-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="dc2d4-221">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="dc2d4-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="dc2d4-222">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="dc2d4-223">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="dc2d4-224">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="dc2d4-225">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="dc2d4-226">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="dc2d4-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="dc2d4-228">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc2d4-228">Boolean</span></span>|<span data-ttu-id="dc2d4-229">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="dc2d4-230">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="dc2d4-231">neutralDomainResources</span></span>|<span data-ttu-id="dc2d4-232">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="dc2d4-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="dc2d4-233">Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="dc2d4-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="dc2d4-235">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc2d4-235">Boolean</span></span>|<span data-ttu-id="dc2d4-236">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="dc2d4-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="dc2d4-238">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="dc2d4-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="dc2d4-239">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="dc2d4-240">isAssigned</span></span>|<span data-ttu-id="dc2d4-241">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc2d4-241">Boolean</span></span>|<span data-ttu-id="dc2d4-242">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="dc2d4-243">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="dc2d4-244">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="dc2d4-244">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="dc2d4-245">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc2d4-245">Boolean</span></span>|<span data-ttu-id="dc2d4-246">Neue Eigenschaft in RS2. Dokumentation noch ausstehend.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-246">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="dc2d4-247">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="dc2d4-247">mdmEnrollmentUrl</span></span>|<span data-ttu-id="dc2d4-248">String</span><span class="sxs-lookup"><span data-stu-id="dc2d4-248">String</span></span>|<span data-ttu-id="dc2d4-249">URL zur Registrierung in der MDM-Lösung</span><span class="sxs-lookup"><span data-stu-id="dc2d4-249">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="dc2d4-250">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="dc2d4-250">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="dc2d4-251">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dc2d4-251">Boolean</span></span>|<span data-ttu-id="dc2d4-252">Boolescher Wert, der Windows Hello for Business als Methode für die Anmeldung bei Windows festlegt</span><span class="sxs-lookup"><span data-stu-id="dc2d4-252">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="dc2d4-253">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dc2d4-253">pinMinimumLength</span></span>|<span data-ttu-id="dc2d4-254">Int32</span><span class="sxs-lookup"><span data-stu-id="dc2d4-254">Int32</span></span>|<span data-ttu-id="dc2d4-255">Ganze Zahl, die festlegt, wie viele Zeichen die PIN mindestens haben muss.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-255">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="dc2d4-256">Der Standardwert ist „4“.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-256">Default value is 4.</span></span> <span data-ttu-id="dc2d4-257">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 4.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-257">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="dc2d4-258">Die größte Zahl, die Sie konfigurieren können, muss kleiner sein als die Zahl, die Sie für die Richtlinieneinstellung zur Festlegung der PIN-Maximallänge angegeben haben, oder kleiner als 127 (je nachdem, welche Zahl kleiner ist).</span><span class="sxs-lookup"><span data-stu-id="dc2d4-258">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="dc2d4-259">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="dc2d4-259">pinUppercaseLetters</span></span>|[<span data-ttu-id="dc2d4-260">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="dc2d4-260">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="dc2d4-261">Ganzzahlwert, der konfiguriert, ob Großbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-261">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="dc2d4-262">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-262">Default is NotAllow.</span></span> <span data-ttu-id="dc2d4-263">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-263">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="dc2d4-264">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="dc2d4-264">pinLowercaseLetters</span></span>|[<span data-ttu-id="dc2d4-265">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="dc2d4-265">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="dc2d4-266">Ganzzahlwert, der konfiguriert, ob Kleinbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-266">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="dc2d4-267">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-267">Default is NotAllow.</span></span> <span data-ttu-id="dc2d4-268">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-268">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="dc2d4-269">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="dc2d4-269">pinSpecialCharacters</span></span>|[<span data-ttu-id="dc2d4-270">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="dc2d4-270">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="dc2d4-271">Ganzzahlwert, der konfiguriert, ob Sonderzeichen in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-271">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="dc2d4-272">Zu den zulässigen Sonderzeichen für Windows Hello for Business-Gesten gehören: !</span><span class="sxs-lookup"><span data-stu-id="dc2d4-272">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="dc2d4-273">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="dc2d4-273">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="dc2d4-274">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="dc2d4-274">/ : ; < = > ?</span></span><span data-ttu-id="dc2d4-275"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="dc2d4-275"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="dc2d4-276">} ~.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-276">} ~.</span></span> <span data-ttu-id="dc2d4-277">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-277">Default is NotAllow.</span></span> <span data-ttu-id="dc2d4-278">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-278">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="dc2d4-279">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dc2d4-279">pinExpirationDays</span></span>|<span data-ttu-id="dc2d4-280">Int32</span><span class="sxs-lookup"><span data-stu-id="dc2d4-280">Int32</span></span>|<span data-ttu-id="dc2d4-281">Ganzzahlwert, der angibt, wie viele Tage die PIN verwendet werden darf, bevor das System den Benutzer auffordert, sie zu ändern.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-281">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="dc2d4-282">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 730.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-282">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="dc2d4-283">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-283">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="dc2d4-284">Wenn Sie für diese Richtlinie „0“ festlegen, läuft die PIN des Benutzers niemals ab.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-284">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="dc2d4-285">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-285">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="dc2d4-286">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-286">Default is 0.</span></span>|
|<span data-ttu-id="dc2d4-287">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="dc2d4-287">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="dc2d4-288">Int32</span><span class="sxs-lookup"><span data-stu-id="dc2d4-288">Int32</span></span>|<span data-ttu-id="dc2d4-289">Ganzzahlwert, der angibt, wie viele der zuletzt dem Benutzerkonto zugeordneten PINs nicht wiederverwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-289">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="dc2d4-290">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 50.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-290">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="dc2d4-291">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-291">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="dc2d4-292">Wenn Sie für diese Richtlinie „0“ festlegen, wird keine Speicherung früherer PINs erzwungen.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-292">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="dc2d4-293">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-293">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="dc2d4-294">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-294">Default is 0.</span></span>|
|<span data-ttu-id="dc2d4-295">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="dc2d4-295">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="dc2d4-296">Int32</span><span class="sxs-lookup"><span data-stu-id="dc2d4-296">Int32</span></span>|<span data-ttu-id="dc2d4-297">Legt fest, wie oft die Authentifizierung fehlschlagen darf, bevor das Gerät zurückgesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-297">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="dc2d4-298">Ein Wert von „0“ deaktiviert die Funktion zur Gerätezurücksetzung.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-298">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="dc2d4-299">Gültig sind Ganzzahlen X, wobei gilt 4 <= X <= 16 für Desktops und 0 <= X <= 999 für Mobilgeräte.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-299">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="dc2d4-300">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="dc2d4-300">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="dc2d4-301">Int32</span><span class="sxs-lookup"><span data-stu-id="dc2d4-301">Int32</span></span>|<span data-ttu-id="dc2d4-302">Gibt an, wie viele Minuten sich das Gerät maximal im Leerlauf befinden darf, bevor eine PIN- oder Kennwortsperre aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-302">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="dc2d4-303">Gültig sind Ganzzahlen X, wobei gilt 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-303">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="dc2d4-304">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="dc2d4-304">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="dc2d4-305">Int32</span><span class="sxs-lookup"><span data-stu-id="dc2d4-305">Int32</span></span>|<span data-ttu-id="dc2d4-306">Offline-Intervall (in Tagen), nach dem die App-Daten gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="dc2d4-306">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="dc2d4-307">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc2d4-307">Response</span></span>
<span data-ttu-id="dc2d4-308">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-308">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc2d4-309">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dc2d4-309">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc2d4-310">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc2d4-310">Request</span></span>
<span data-ttu-id="dc2d4-311">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-311">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc2d4-312">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc2d4-312">Response</span></span>
<span data-ttu-id="dc2d4-p131">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc2d4-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


