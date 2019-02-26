---
title: Erstellen von „mdmWindowsInformationProtectionPolicy“
description: Erstellt neue Objekte des Typs mdmWindowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: edc7f8bfdec331dcb69899b925eb3c0206783f25
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251181"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="32cbe-103">Erstellen von „mdmWindowsInformationProtectionPolicy“</span><span class="sxs-lookup"><span data-stu-id="32cbe-103">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="32cbe-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="32cbe-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32cbe-105">Diese Methode erstellt ein neues Objekt des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-105">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32cbe-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="32cbe-106">Prerequisites</span></span>
<span data-ttu-id="32cbe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="32cbe-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32cbe-109">Permission type</span></span>|<span data-ttu-id="32cbe-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32cbe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32cbe-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32cbe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="32cbe-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32cbe-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32cbe-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32cbe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32cbe-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32cbe-114">Not supported.</span></span>|
|<span data-ttu-id="32cbe-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32cbe-115">Application</span></span>|<span data-ttu-id="32cbe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32cbe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32cbe-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32cbe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="32cbe-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32cbe-118">Request headers</span></span>
|<span data-ttu-id="32cbe-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="32cbe-119">Header</span></span>|<span data-ttu-id="32cbe-120">Wert</span><span class="sxs-lookup"><span data-stu-id="32cbe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32cbe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="32cbe-121">Authorization</span></span>|<span data-ttu-id="32cbe-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="32cbe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32cbe-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="32cbe-123">Accept</span></span>|<span data-ttu-id="32cbe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="32cbe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32cbe-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32cbe-125">Request body</span></span>
<span data-ttu-id="32cbe-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mdmWindowsInformationProtectionPolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="32cbe-126">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="32cbe-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mdmWindowsInformationProtectionPolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="32cbe-127">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="32cbe-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32cbe-128">Property</span></span>|<span data-ttu-id="32cbe-129">Typ</span><span class="sxs-lookup"><span data-stu-id="32cbe-129">Type</span></span>|<span data-ttu-id="32cbe-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32cbe-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32cbe-131">displayName</span><span class="sxs-lookup"><span data-stu-id="32cbe-131">displayName</span></span>|<span data-ttu-id="32cbe-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="32cbe-132">String</span></span>|<span data-ttu-id="32cbe-133">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="32cbe-133">Policy display name.</span></span> <span data-ttu-id="32cbe-134">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="32cbe-135">description</span><span class="sxs-lookup"><span data-stu-id="32cbe-135">description</span></span>|<span data-ttu-id="32cbe-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="32cbe-136">String</span></span>|<span data-ttu-id="32cbe-137">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="32cbe-137">The policy's description.</span></span> <span data-ttu-id="32cbe-138">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="32cbe-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32cbe-139">createdDateTime</span></span>|<span data-ttu-id="32cbe-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32cbe-140">DateTimeOffset</span></span>|<span data-ttu-id="32cbe-141">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="32cbe-141">The date and time the policy was created.</span></span> <span data-ttu-id="32cbe-142">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="32cbe-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32cbe-143">lastModifiedDateTime</span></span>|<span data-ttu-id="32cbe-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32cbe-144">DateTimeOffset</span></span>|<span data-ttu-id="32cbe-145">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="32cbe-145">Last time the policy was modified.</span></span> <span data-ttu-id="32cbe-146">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="32cbe-147">id</span><span class="sxs-lookup"><span data-stu-id="32cbe-147">id</span></span>|<span data-ttu-id="32cbe-148">string</span><span class="sxs-lookup"><span data-stu-id="32cbe-148">String</span></span>|<span data-ttu-id="32cbe-149">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="32cbe-149">Key of the entity.</span></span> <span data-ttu-id="32cbe-150">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="32cbe-151">Version</span><span class="sxs-lookup"><span data-stu-id="32cbe-151">version</span></span>|<span data-ttu-id="32cbe-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="32cbe-152">String</span></span>|<span data-ttu-id="32cbe-153">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="32cbe-153">Version of the entity.</span></span> <span data-ttu-id="32cbe-154">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="32cbe-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="32cbe-155">enforcementLevel</span></span>|[<span data-ttu-id="32cbe-156">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="32cbe-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="32cbe-157">WIP-Erzwingung. Siehe Enum-Definition für unterstützte Werte, die von [WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)geerbt wurden.</span><span class="sxs-lookup"><span data-stu-id="32cbe-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="32cbe-158">Mögliche Werte: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="32cbe-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="32cbe-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="32cbe-159">enterpriseDomain</span></span>|<span data-ttu-id="32cbe-160">String</span><span class="sxs-lookup"><span data-stu-id="32cbe-160">String</span></span>|<span data-ttu-id="32cbe-161">Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="32cbe-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="32cbe-163">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="32cbe-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="32cbe-164">Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="32cbe-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="32cbe-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="32cbe-166">Boolean</span></span>|<span data-ttu-id="32cbe-167">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="32cbe-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="32cbe-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="32cbe-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="32cbe-170">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="32cbe-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="32cbe-171">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="32cbe-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="32cbe-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="32cbe-173">Boolean</span></span>|<span data-ttu-id="32cbe-174">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="32cbe-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="32cbe-175">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="32cbe-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="32cbe-176">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="32cbe-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="32cbe-177">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="32cbe-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="32cbe-179">Guid</span><span class="sxs-lookup"><span data-stu-id="32cbe-179">Guid</span></span>|<span data-ttu-id="32cbe-180">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="32cbe-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="32cbe-181">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="32cbe-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="32cbe-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="32cbe-183">Boolean</span></span>|<span data-ttu-id="32cbe-184">Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="32cbe-185">iconsVisible</span></span>|<span data-ttu-id="32cbe-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="32cbe-186">Boolean</span></span>|<span data-ttu-id="32cbe-187">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="32cbe-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="32cbe-188">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="32cbe-189">protectedApps</span></span>|<span data-ttu-id="32cbe-190">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="32cbe-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="32cbe-191">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="32cbe-192">exemptApps</span></span>|<span data-ttu-id="32cbe-193">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="32cbe-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="32cbe-194">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="32cbe-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="32cbe-195">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="32cbe-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="32cbe-196">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="32cbe-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="32cbe-198">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="32cbe-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="32cbe-199">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="32cbe-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="32cbe-200">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="32cbe-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="32cbe-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="32cbe-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="32cbe-203">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="32cbe-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="32cbe-204">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="32cbe-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="32cbe-205">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="32cbe-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="32cbe-206">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="32cbe-207">enterpriseIPRanges</span></span>|<span data-ttu-id="32cbe-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="32cbe-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="32cbe-209">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="32cbe-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="32cbe-210">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="32cbe-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="32cbe-211">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="32cbe-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="32cbe-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="32cbe-213">Boolean</span></span>|<span data-ttu-id="32cbe-214">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="32cbe-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="32cbe-215">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="32cbe-216">enterpriseProxyServers</span></span>|<span data-ttu-id="32cbe-217">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="32cbe-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="32cbe-218">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="32cbe-218">This is a list of proxy servers.</span></span> <span data-ttu-id="32cbe-219">Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="32cbe-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="32cbe-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="32cbe-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="32cbe-222">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="32cbe-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="32cbe-223">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="32cbe-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="32cbe-224">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="32cbe-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="32cbe-225">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="32cbe-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="32cbe-226">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="32cbe-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="32cbe-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="32cbe-228">Boolean</span></span>|<span data-ttu-id="32cbe-229">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="32cbe-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="32cbe-230">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="32cbe-231">neutralDomainResources</span></span>|<span data-ttu-id="32cbe-232">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="32cbe-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="32cbe-233">Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="32cbe-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="32cbe-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="32cbe-235">Boolean</span></span>|<span data-ttu-id="32cbe-236">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="32cbe-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="32cbe-238">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="32cbe-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="32cbe-239">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="32cbe-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="32cbe-240">isAssigned</span></span>|<span data-ttu-id="32cbe-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="32cbe-241">Boolean</span></span>|<span data-ttu-id="32cbe-242">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="32cbe-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="32cbe-243">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="32cbe-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="32cbe-244">Antwort</span><span class="sxs-lookup"><span data-stu-id="32cbe-244">Response</span></span>
<span data-ttu-id="32cbe-245">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="32cbe-245">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32cbe-246">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32cbe-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="32cbe-247">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32cbe-247">Request</span></span>
<span data-ttu-id="32cbe-248">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32cbe-248">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32cbe-249">Antwort</span><span class="sxs-lookup"><span data-stu-id="32cbe-249">Response</span></span>
<span data-ttu-id="32cbe-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32cbe-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



