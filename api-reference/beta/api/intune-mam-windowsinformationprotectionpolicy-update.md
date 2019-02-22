---
title: Aktualisieren von windowsInformationProtectionPolicy
description: Aktualisiert die Eigenschaften von Objekten des Typs windowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab1beb262120c8d50f1ec53c6ea30a7037ce469f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144065"
---
# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="06838-103">Aktualisieren von windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="06838-103">Update windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="06838-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06838-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06838-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="06838-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06838-106">Aktualisiert die Eigenschaften von Objekten des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06838-106">Update the properties of a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06838-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="06838-107">Prerequisites</span></span>
<span data-ttu-id="06838-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="06838-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="06838-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06838-110">Permission type</span></span>|<span data-ttu-id="06838-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06838-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06838-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06838-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06838-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06838-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06838-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06838-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06838-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06838-115">Not supported.</span></span>|
|<span data-ttu-id="06838-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06838-116">Application</span></span>|<span data-ttu-id="06838-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06838-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06838-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06838-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="06838-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06838-119">Request headers</span></span>
|<span data-ttu-id="06838-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="06838-120">Header</span></span>|<span data-ttu-id="06838-121">Wert</span><span class="sxs-lookup"><span data-stu-id="06838-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06838-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06838-122">Authorization</span></span>|<span data-ttu-id="06838-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="06838-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06838-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="06838-124">Accept</span></span>|<span data-ttu-id="06838-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06838-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06838-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06838-126">Request body</span></span>
<span data-ttu-id="06838-127">Geben Sie als Anforderungstext eine JSON-Darstellung eines Objekts des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) an.</span><span class="sxs-lookup"><span data-stu-id="06838-127">In the request body, supply a JSON representation for the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="06838-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="06838-128">The following table shows the properties that are required when you create the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="06838-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06838-129">Property</span></span>|<span data-ttu-id="06838-130">Typ</span><span class="sxs-lookup"><span data-stu-id="06838-130">Type</span></span>|<span data-ttu-id="06838-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06838-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06838-132">displayName</span><span class="sxs-lookup"><span data-stu-id="06838-132">displayName</span></span>|<span data-ttu-id="06838-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06838-133">String</span></span>|<span data-ttu-id="06838-134">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="06838-134">Policy display name.</span></span> <span data-ttu-id="06838-135">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06838-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="06838-136">description</span><span class="sxs-lookup"><span data-stu-id="06838-136">description</span></span>|<span data-ttu-id="06838-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06838-137">String</span></span>|<span data-ttu-id="06838-138">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="06838-138">The policy's description.</span></span> <span data-ttu-id="06838-139">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06838-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="06838-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06838-140">createdDateTime</span></span>|<span data-ttu-id="06838-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06838-141">DateTimeOffset</span></span>|<span data-ttu-id="06838-142">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="06838-142">The date and time the policy was created.</span></span> <span data-ttu-id="06838-143">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06838-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="06838-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06838-144">lastModifiedDateTime</span></span>|<span data-ttu-id="06838-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06838-145">DateTimeOffset</span></span>|<span data-ttu-id="06838-146">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="06838-146">Last time the policy was modified.</span></span> <span data-ttu-id="06838-147">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06838-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="06838-148">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="06838-148">roleScopeTagIds</span></span>|<span data-ttu-id="06838-149">String collection</span><span class="sxs-lookup"><span data-stu-id="06838-149">String collection</span></span>|<span data-ttu-id="06838-150">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="06838-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="06838-151">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06838-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="06838-152">id</span><span class="sxs-lookup"><span data-stu-id="06838-152">id</span></span>|<span data-ttu-id="06838-153">string</span><span class="sxs-lookup"><span data-stu-id="06838-153">String</span></span>|<span data-ttu-id="06838-154">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="06838-154">Key of the entity.</span></span> <span data-ttu-id="06838-155">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06838-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="06838-156">Version</span><span class="sxs-lookup"><span data-stu-id="06838-156">version</span></span>|<span data-ttu-id="06838-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06838-157">String</span></span>|<span data-ttu-id="06838-158">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="06838-158">Version of the entity.</span></span> <span data-ttu-id="06838-159">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06838-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="06838-160">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="06838-160">enforcementLevel</span></span>|[<span data-ttu-id="06838-161">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="06838-161">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="06838-162">WIP-Erzwingung. Siehe Enum-Definition für unterstützte Werte, die von [WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)geerbt wurden.</span><span class="sxs-lookup"><span data-stu-id="06838-162">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="06838-163">Mögliche Werte: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="06838-163">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="06838-164">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="06838-164">enterpriseDomain</span></span>|<span data-ttu-id="06838-165">String</span><span class="sxs-lookup"><span data-stu-id="06838-165">String</span></span>|<span data-ttu-id="06838-166">Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-166">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-167">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="06838-167">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="06838-168">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="06838-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="06838-169">Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-169">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-170">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="06838-170">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="06838-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06838-171">Boolean</span></span>|<span data-ttu-id="06838-172">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-172">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-173">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="06838-173">dataRecoveryCertificate</span></span>|[<span data-ttu-id="06838-174">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="06838-174">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="06838-175">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="06838-175">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="06838-176">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-176">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-177">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="06838-177">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="06838-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06838-178">Boolean</span></span>|<span data-ttu-id="06838-179">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="06838-179">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="06838-180">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="06838-180">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="06838-181">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="06838-181">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="06838-182">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-182">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-183">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="06838-183">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="06838-184">Guid</span><span class="sxs-lookup"><span data-stu-id="06838-184">Guid</span></span>|<span data-ttu-id="06838-185">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="06838-185">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="06838-186">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-186">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-187">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="06838-187">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="06838-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="06838-188">Boolean</span></span>|<span data-ttu-id="06838-189">Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-189">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-190">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="06838-190">iconsVisible</span></span>|<span data-ttu-id="06838-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="06838-191">Boolean</span></span>|<span data-ttu-id="06838-192">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="06838-192">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="06838-193">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-193">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-194">protectedApps</span><span class="sxs-lookup"><span data-stu-id="06838-194">protectedApps</span></span>|<span data-ttu-id="06838-195">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="06838-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="06838-196">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-196">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-197">exemptApps</span><span class="sxs-lookup"><span data-stu-id="06838-197">exemptApps</span></span>|<span data-ttu-id="06838-198">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="06838-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="06838-199">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="06838-199">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="06838-200">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="06838-200">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="06838-201">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-201">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-202">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="06838-202">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="06838-203">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="06838-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="06838-204">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="06838-204">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="06838-205">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-205">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-206">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="06838-206">enterpriseProxiedDomains</span></span>|<span data-ttu-id="06838-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06838-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="06838-208">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="06838-208">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="06838-209">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="06838-209">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="06838-210">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="06838-210">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="06838-211">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-211">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-212">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="06838-212">enterpriseIPRanges</span></span>|<span data-ttu-id="06838-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06838-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="06838-214">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="06838-214">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="06838-215">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="06838-215">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="06838-216">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-216">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-217">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="06838-217">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="06838-218">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06838-218">Boolean</span></span>|<span data-ttu-id="06838-219">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="06838-219">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="06838-220">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-220">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-221">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="06838-221">enterpriseProxyServers</span></span>|<span data-ttu-id="06838-222">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="06838-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="06838-223">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="06838-223">This is a list of proxy servers.</span></span> <span data-ttu-id="06838-224">Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-224">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-225">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="06838-225">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="06838-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06838-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="06838-227">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="06838-227">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="06838-228">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="06838-228">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="06838-229">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="06838-229">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="06838-230">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="06838-230">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="06838-231">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-231">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-232">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="06838-232">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="06838-233">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06838-233">Boolean</span></span>|<span data-ttu-id="06838-234">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="06838-234">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="06838-235">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-235">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-236">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="06838-236">neutralDomainResources</span></span>|<span data-ttu-id="06838-237">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="06838-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="06838-238">Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-238">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-239">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="06838-239">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="06838-240">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06838-240">Boolean</span></span>|<span data-ttu-id="06838-241">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-241">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-242">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="06838-242">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="06838-243">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="06838-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="06838-244">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-244">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-245">isAssigned</span><span class="sxs-lookup"><span data-stu-id="06838-245">isAssigned</span></span>|<span data-ttu-id="06838-246">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06838-246">Boolean</span></span>|<span data-ttu-id="06838-247">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="06838-247">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="06838-248">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06838-248">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="06838-249">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="06838-249">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="06838-250">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06838-250">Boolean</span></span>|<span data-ttu-id="06838-251">Neue Eigenschaft in RS2. Dokumentation noch ausstehend.</span><span class="sxs-lookup"><span data-stu-id="06838-251">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="06838-252">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="06838-252">mdmEnrollmentUrl</span></span>|<span data-ttu-id="06838-253">String</span><span class="sxs-lookup"><span data-stu-id="06838-253">String</span></span>|<span data-ttu-id="06838-254">URL zur Registrierung in der MDM-Lösung</span><span class="sxs-lookup"><span data-stu-id="06838-254">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="06838-255">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="06838-255">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="06838-256">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06838-256">Boolean</span></span>|<span data-ttu-id="06838-257">Boolescher Wert, der Windows Hello for Business als Methode für die Anmeldung bei Windows festlegt</span><span class="sxs-lookup"><span data-stu-id="06838-257">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="06838-258">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="06838-258">pinMinimumLength</span></span>|<span data-ttu-id="06838-259">Int32</span><span class="sxs-lookup"><span data-stu-id="06838-259">Int32</span></span>|<span data-ttu-id="06838-260">Ganze Zahl, die festlegt, wie viele Zeichen die PIN mindestens haben muss.</span><span class="sxs-lookup"><span data-stu-id="06838-260">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="06838-261">Der Standardwert ist „4“.</span><span class="sxs-lookup"><span data-stu-id="06838-261">Default value is 4.</span></span> <span data-ttu-id="06838-262">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 4.</span><span class="sxs-lookup"><span data-stu-id="06838-262">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="06838-263">Die größte Zahl, die Sie konfigurieren können, muss kleiner sein als die Zahl, die Sie für die Richtlinieneinstellung zur Festlegung der PIN-Maximallänge angegeben haben, oder kleiner als 127 (je nachdem, welche Zahl kleiner ist).</span><span class="sxs-lookup"><span data-stu-id="06838-263">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="06838-264">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="06838-264">pinUppercaseLetters</span></span>|[<span data-ttu-id="06838-265">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="06838-265">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="06838-266">Ganzzahlwert, der konfiguriert, ob Großbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="06838-266">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="06838-267">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="06838-267">Default is NotAllow.</span></span> <span data-ttu-id="06838-268">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="06838-268">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="06838-269">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="06838-269">pinLowercaseLetters</span></span>|[<span data-ttu-id="06838-270">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="06838-270">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="06838-271">Ganzzahlwert, der konfiguriert, ob Kleinbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="06838-271">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="06838-272">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="06838-272">Default is NotAllow.</span></span> <span data-ttu-id="06838-273">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="06838-273">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="06838-274">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="06838-274">pinSpecialCharacters</span></span>|[<span data-ttu-id="06838-275">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="06838-275">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="06838-276">Ganzzahlwert, der konfiguriert, ob Sonderzeichen in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="06838-276">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="06838-277">Zu den zulässigen Sonderzeichen für Windows Hello for Business-Gesten gehören: !</span><span class="sxs-lookup"><span data-stu-id="06838-277">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="06838-278">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="06838-278">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="06838-279">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="06838-279">/ : ; < = > ?</span></span><span data-ttu-id="06838-280"> @ \[ \ \]^ _ ` { | } ~. Default is NotAllow. Possible values are: \`notalg`, \`requireAtLeastOne`, \`Allow '.</span><span class="sxs-lookup"><span data-stu-id="06838-280"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: \`notAllow`, \`requireAtLeastOne`, \`allow\`.</span></span>|
|<span data-ttu-id="06838-281">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="06838-281">pinExpirationDays</span></span>|<span data-ttu-id="06838-282">Int32</span><span class="sxs-lookup"><span data-stu-id="06838-282">Int32</span></span>|<span data-ttu-id="06838-283">Ganzzahlwert, der angibt, wie viele Tage die PIN verwendet werden darf, bevor das System den Benutzer auffordert, sie zu ändern.</span><span class="sxs-lookup"><span data-stu-id="06838-283">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="06838-284">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 730.</span><span class="sxs-lookup"><span data-stu-id="06838-284">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="06838-285">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="06838-285">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="06838-286">Wenn Sie für diese Richtlinie „0“ festlegen, läuft die PIN des Benutzers niemals ab.</span><span class="sxs-lookup"><span data-stu-id="06838-286">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="06838-287">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="06838-287">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="06838-288">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="06838-288">Default is 0.</span></span>|
|<span data-ttu-id="06838-289">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="06838-289">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="06838-290">Int32</span><span class="sxs-lookup"><span data-stu-id="06838-290">Int32</span></span>|<span data-ttu-id="06838-291">Ganzzahlwert, der angibt, wie viele der zuletzt dem Benutzerkonto zugeordneten PINs nicht wiederverwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="06838-291">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="06838-292">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 50.</span><span class="sxs-lookup"><span data-stu-id="06838-292">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="06838-293">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="06838-293">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="06838-294">Wenn Sie für diese Richtlinie „0“ festlegen, wird keine Speicherung früherer PINs erzwungen.</span><span class="sxs-lookup"><span data-stu-id="06838-294">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="06838-295">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="06838-295">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="06838-296">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="06838-296">Default is 0.</span></span>|
|<span data-ttu-id="06838-297">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="06838-297">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="06838-298">Int32</span><span class="sxs-lookup"><span data-stu-id="06838-298">Int32</span></span>|<span data-ttu-id="06838-299">Legt fest, wie oft die Authentifizierung fehlschlagen darf, bevor das Gerät zurückgesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="06838-299">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="06838-300">Ein Wert von „0“ deaktiviert die Funktion zur Gerätezurücksetzung.</span><span class="sxs-lookup"><span data-stu-id="06838-300">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="06838-301">Gültig sind Ganzzahlen X, wobei gilt 4 <= X <= 16 für Desktops und 0 <= X <= 999 für Mobilgeräte.</span><span class="sxs-lookup"><span data-stu-id="06838-301">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="06838-302">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="06838-302">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="06838-303">Int32</span><span class="sxs-lookup"><span data-stu-id="06838-303">Int32</span></span>|<span data-ttu-id="06838-304">Gibt an, wie viele Minuten sich das Gerät maximal im Leerlauf befinden darf, bevor eine PIN- oder Kennwortsperre aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="06838-304">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="06838-305">Gültig sind Ganzzahlen X, wobei gilt 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="06838-305">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="06838-306">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="06838-306">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="06838-307">Int32</span><span class="sxs-lookup"><span data-stu-id="06838-307">Int32</span></span>|<span data-ttu-id="06838-308">Offline-Intervall (in Tagen), nach dem die App-Daten gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="06838-308">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="06838-309">Antwort</span><span class="sxs-lookup"><span data-stu-id="06838-309">Response</span></span>
<span data-ttu-id="06838-310">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="06838-310">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06838-311">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06838-311">Example</span></span>

### <a name="request"></a><span data-ttu-id="06838-312">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06838-312">Request</span></span>
<span data-ttu-id="06838-313">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06838-313">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 4467

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="06838-314">Antwort</span><span class="sxs-lookup"><span data-stu-id="06838-314">Response</span></span>
<span data-ttu-id="06838-p131">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06838-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4639

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




