---
title: Erstellen von windowsInformationProtectionPolicy
description: Erstellt neue Objekte des Typs windowsInformationProtectionPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74d9e4a8ddd9ae0979a6360eaf229396b2e107bb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416608"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="84a22-103">Erstellen von windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="84a22-103">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="84a22-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="84a22-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84a22-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84a22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84a22-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="84a22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84a22-107">Erstellt neue Objekte des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-107">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84a22-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="84a22-108">Prerequisites</span></span>
<span data-ttu-id="84a22-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="84a22-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84a22-111">Permission type</span></span>|<span data-ttu-id="84a22-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84a22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84a22-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84a22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84a22-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a22-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="84a22-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84a22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84a22-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84a22-116">Not supported.</span></span>|
|<span data-ttu-id="84a22-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84a22-117">Application</span></span>|<span data-ttu-id="84a22-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84a22-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84a22-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84a22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="84a22-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84a22-120">Request headers</span></span>
|<span data-ttu-id="84a22-121">Header</span><span class="sxs-lookup"><span data-stu-id="84a22-121">Header</span></span>|<span data-ttu-id="84a22-122">Wert</span><span class="sxs-lookup"><span data-stu-id="84a22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84a22-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="84a22-123">Authorization</span></span>|<span data-ttu-id="84a22-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="84a22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84a22-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="84a22-125">Accept</span></span>|<span data-ttu-id="84a22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84a22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84a22-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84a22-127">Request body</span></span>
<span data-ttu-id="84a22-128">Geben Sie als Anforderungstext eine JSON-Darstellung eines Objekts des Typs windowsInformationProtectionPolicy an.</span><span class="sxs-lookup"><span data-stu-id="84a22-128">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="84a22-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs windowsInformationProtectionPolicy erstellen.</span><span class="sxs-lookup"><span data-stu-id="84a22-129">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="84a22-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="84a22-130">Property</span></span>|<span data-ttu-id="84a22-131">Typ</span><span class="sxs-lookup"><span data-stu-id="84a22-131">Type</span></span>|<span data-ttu-id="84a22-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84a22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84a22-133">displayName</span><span class="sxs-lookup"><span data-stu-id="84a22-133">displayName</span></span>|<span data-ttu-id="84a22-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84a22-134">String</span></span>|<span data-ttu-id="84a22-135">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="84a22-135">Policy display name.</span></span> <span data-ttu-id="84a22-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84a22-137">description</span><span class="sxs-lookup"><span data-stu-id="84a22-137">description</span></span>|<span data-ttu-id="84a22-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84a22-138">String</span></span>|<span data-ttu-id="84a22-139">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="84a22-139">The policy's description.</span></span> <span data-ttu-id="84a22-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84a22-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84a22-141">createdDateTime</span></span>|<span data-ttu-id="84a22-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84a22-142">DateTimeOffset</span></span>|<span data-ttu-id="84a22-143">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="84a22-143">The date and time the policy was created.</span></span> <span data-ttu-id="84a22-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84a22-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84a22-145">lastModifiedDateTime</span></span>|<span data-ttu-id="84a22-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84a22-146">DateTimeOffset</span></span>|<span data-ttu-id="84a22-147">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="84a22-147">Last time the policy was modified.</span></span> <span data-ttu-id="84a22-148">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84a22-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84a22-149">roleScopeTagIds</span></span>|<span data-ttu-id="84a22-150">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="84a22-150">String collection</span></span>|<span data-ttu-id="84a22-151">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="84a22-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="84a22-152">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84a22-153">id</span><span class="sxs-lookup"><span data-stu-id="84a22-153">id</span></span>|<span data-ttu-id="84a22-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84a22-154">String</span></span>|<span data-ttu-id="84a22-155">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="84a22-155">Key of the entity.</span></span> <span data-ttu-id="84a22-156">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84a22-157">Version</span><span class="sxs-lookup"><span data-stu-id="84a22-157">version</span></span>|<span data-ttu-id="84a22-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84a22-158">String</span></span>|<span data-ttu-id="84a22-159">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="84a22-159">Version of the entity.</span></span> <span data-ttu-id="84a22-160">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84a22-161">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="84a22-161">enforcementLevel</span></span>|[<span data-ttu-id="84a22-162">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="84a22-162">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="84a22-163">WIP Erzwingung-Ebene. Siehe die Enum-Definition für unterstützte Werte Inherited aus [WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-163">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="84a22-164">Mögliche Werte: sind `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt` und `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="84a22-164">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="84a22-165">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="84a22-165">enterpriseDomain</span></span>|<span data-ttu-id="84a22-166">String</span><span class="sxs-lookup"><span data-stu-id="84a22-166">String</span></span>|<span data-ttu-id="84a22-167">Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-167">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-168">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="84a22-168">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="84a22-169">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84a22-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84a22-170">Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-170">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-171">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="84a22-171">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="84a22-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a22-172">Boolean</span></span>|<span data-ttu-id="84a22-173">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-173">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-174">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="84a22-174">dataRecoveryCertificate</span></span>|[<span data-ttu-id="84a22-175">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="84a22-175">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="84a22-176">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="84a22-176">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="84a22-177">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-177">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-178">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="84a22-178">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="84a22-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a22-179">Boolean</span></span>|<span data-ttu-id="84a22-180">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="84a22-180">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="84a22-181">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="84a22-181">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="84a22-182">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="84a22-182">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="84a22-183">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-183">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-184">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="84a22-184">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="84a22-185">Guid</span><span class="sxs-lookup"><span data-stu-id="84a22-185">Guid</span></span>|<span data-ttu-id="84a22-186">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="84a22-186">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="84a22-187">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-187">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-188">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="84a22-188">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="84a22-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a22-189">Boolean</span></span>|<span data-ttu-id="84a22-190">Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-190">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-191">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="84a22-191">iconsVisible</span></span>|<span data-ttu-id="84a22-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a22-192">Boolean</span></span>|<span data-ttu-id="84a22-193">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="84a22-193">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="84a22-194">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-194">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-195">protectedApps</span><span class="sxs-lookup"><span data-stu-id="84a22-195">protectedApps</span></span>|<span data-ttu-id="84a22-196">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="84a22-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="84a22-197">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-197">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-198">exemptApps</span><span class="sxs-lookup"><span data-stu-id="84a22-198">exemptApps</span></span>|<span data-ttu-id="84a22-199">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="84a22-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="84a22-200">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="84a22-200">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="84a22-201">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="84a22-201">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="84a22-202">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-202">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-203">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="84a22-203">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="84a22-204">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84a22-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84a22-205">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="84a22-205">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="84a22-206">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-206">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-207">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="84a22-207">enterpriseProxiedDomains</span></span>|<span data-ttu-id="84a22-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="84a22-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="84a22-209">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="84a22-209">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="84a22-210">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="84a22-210">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="84a22-211">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="84a22-211">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="84a22-212">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-212">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-213">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="84a22-213">enterpriseIPRanges</span></span>|<span data-ttu-id="84a22-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="84a22-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="84a22-215">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="84a22-215">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="84a22-216">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="84a22-216">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="84a22-217">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-217">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-218">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="84a22-218">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="84a22-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a22-219">Boolean</span></span>|<span data-ttu-id="84a22-220">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="84a22-220">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="84a22-221">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-221">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-222">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="84a22-222">enterpriseProxyServers</span></span>|<span data-ttu-id="84a22-223">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84a22-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84a22-224">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="84a22-224">This is a list of proxy servers.</span></span> <span data-ttu-id="84a22-225">Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-225">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-226">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="84a22-226">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="84a22-227">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84a22-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84a22-228">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="84a22-228">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="84a22-229">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="84a22-229">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="84a22-230">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="84a22-230">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="84a22-231">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="84a22-231">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="84a22-232">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-232">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-233">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="84a22-233">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="84a22-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a22-234">Boolean</span></span>|<span data-ttu-id="84a22-235">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="84a22-235">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="84a22-236">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-236">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-237">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="84a22-237">neutralDomainResources</span></span>|<span data-ttu-id="84a22-238">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84a22-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84a22-239">Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-239">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-240">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="84a22-240">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="84a22-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a22-241">Boolean</span></span>|<span data-ttu-id="84a22-242">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-242">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-243">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="84a22-243">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="84a22-244">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84a22-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84a22-245">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-245">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-246">isAssigned</span><span class="sxs-lookup"><span data-stu-id="84a22-246">isAssigned</span></span>|<span data-ttu-id="84a22-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a22-247">Boolean</span></span>|<span data-ttu-id="84a22-248">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="84a22-248">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="84a22-249">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84a22-249">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84a22-250">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="84a22-250">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="84a22-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a22-251">Boolean</span></span>|<span data-ttu-id="84a22-252">Neue Eigenschaft in RS2. Dokumentation noch ausstehend.</span><span class="sxs-lookup"><span data-stu-id="84a22-252">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="84a22-253">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="84a22-253">mdmEnrollmentUrl</span></span>|<span data-ttu-id="84a22-254">String</span><span class="sxs-lookup"><span data-stu-id="84a22-254">String</span></span>|<span data-ttu-id="84a22-255">URL zur Registrierung in der MDM-Lösung</span><span class="sxs-lookup"><span data-stu-id="84a22-255">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="84a22-256">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="84a22-256">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="84a22-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a22-257">Boolean</span></span>|<span data-ttu-id="84a22-258">Boolescher Wert, der Windows Hello for Business als Methode für die Anmeldung bei Windows festlegt</span><span class="sxs-lookup"><span data-stu-id="84a22-258">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="84a22-259">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="84a22-259">pinMinimumLength</span></span>|<span data-ttu-id="84a22-260">Int32</span><span class="sxs-lookup"><span data-stu-id="84a22-260">Int32</span></span>|<span data-ttu-id="84a22-261">Ganze Zahl, die festlegt, wie viele Zeichen die PIN mindestens haben muss.</span><span class="sxs-lookup"><span data-stu-id="84a22-261">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="84a22-262">Der Standardwert ist „4“.</span><span class="sxs-lookup"><span data-stu-id="84a22-262">Default value is 4.</span></span> <span data-ttu-id="84a22-263">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 4.</span><span class="sxs-lookup"><span data-stu-id="84a22-263">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="84a22-264">Die größte Zahl, die Sie konfigurieren können, muss kleiner sein als die Zahl, die Sie für die Richtlinieneinstellung zur Festlegung der PIN-Maximallänge angegeben haben, oder kleiner als 127 (je nachdem, welche Zahl kleiner ist).</span><span class="sxs-lookup"><span data-stu-id="84a22-264">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="84a22-265">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="84a22-265">pinUppercaseLetters</span></span>|[<span data-ttu-id="84a22-266">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="84a22-266">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="84a22-267">Ganzzahlwert, der konfiguriert, ob Großbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="84a22-267">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="84a22-268">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="84a22-268">Default is NotAllow.</span></span> <span data-ttu-id="84a22-269">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="84a22-269">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="84a22-270">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="84a22-270">pinLowercaseLetters</span></span>|[<span data-ttu-id="84a22-271">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="84a22-271">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="84a22-272">Ganzzahlwert, der konfiguriert, ob Kleinbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="84a22-272">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="84a22-273">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="84a22-273">Default is NotAllow.</span></span> <span data-ttu-id="84a22-274">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="84a22-274">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="84a22-275">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="84a22-275">pinSpecialCharacters</span></span>|[<span data-ttu-id="84a22-276">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="84a22-276">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="84a22-277">Ganzzahlwert, der konfiguriert, ob Sonderzeichen in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="84a22-277">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="84a22-278">Zu den zulässigen Sonderzeichen für Windows Hello for Business-Gesten gehören: !</span><span class="sxs-lookup"><span data-stu-id="84a22-278">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="84a22-279">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="84a22-279">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="84a22-280">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="84a22-280">/ : ; < = > ?</span></span><span data-ttu-id="84a22-281"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="84a22-281"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="84a22-282">} ~.</span><span class="sxs-lookup"><span data-stu-id="84a22-282">} ~.</span></span> <span data-ttu-id="84a22-283">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="84a22-283">Default is NotAllow.</span></span> <span data-ttu-id="84a22-284">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="84a22-284">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="84a22-285">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="84a22-285">pinExpirationDays</span></span>|<span data-ttu-id="84a22-286">Int32</span><span class="sxs-lookup"><span data-stu-id="84a22-286">Int32</span></span>|<span data-ttu-id="84a22-287">Ganzzahlwert, der angibt, wie viele Tage die PIN verwendet werden darf, bevor das System den Benutzer auffordert, sie zu ändern.</span><span class="sxs-lookup"><span data-stu-id="84a22-287">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="84a22-288">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 730.</span><span class="sxs-lookup"><span data-stu-id="84a22-288">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="84a22-289">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="84a22-289">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="84a22-290">Wenn Sie für diese Richtlinie „0“ festlegen, läuft die PIN des Benutzers niemals ab.</span><span class="sxs-lookup"><span data-stu-id="84a22-290">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="84a22-291">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="84a22-291">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="84a22-292">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="84a22-292">Default is 0.</span></span>|
|<span data-ttu-id="84a22-293">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="84a22-293">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="84a22-294">Int32</span><span class="sxs-lookup"><span data-stu-id="84a22-294">Int32</span></span>|<span data-ttu-id="84a22-295">Ganzzahlwert, der angibt, wie viele der zuletzt dem Benutzerkonto zugeordneten PINs nicht wiederverwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="84a22-295">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="84a22-296">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 50.</span><span class="sxs-lookup"><span data-stu-id="84a22-296">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="84a22-297">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="84a22-297">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="84a22-298">Wenn Sie für diese Richtlinie „0“ festlegen, wird keine Speicherung früherer PINs erzwungen.</span><span class="sxs-lookup"><span data-stu-id="84a22-298">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="84a22-299">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="84a22-299">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="84a22-300">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="84a22-300">Default is 0.</span></span>|
|<span data-ttu-id="84a22-301">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="84a22-301">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="84a22-302">Int32</span><span class="sxs-lookup"><span data-stu-id="84a22-302">Int32</span></span>|<span data-ttu-id="84a22-303">Legt fest, wie oft die Authentifizierung fehlschlagen darf, bevor das Gerät zurückgesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="84a22-303">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="84a22-304">Ein Wert von „0“ deaktiviert die Funktion zur Gerätezurücksetzung.</span><span class="sxs-lookup"><span data-stu-id="84a22-304">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="84a22-305">Gültig sind Ganzzahlen X, wobei gilt 4 <= X <= 16 für Desktops und 0 <= X <= 999 für Mobilgeräte.</span><span class="sxs-lookup"><span data-stu-id="84a22-305">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="84a22-306">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="84a22-306">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="84a22-307">Int32</span><span class="sxs-lookup"><span data-stu-id="84a22-307">Int32</span></span>|<span data-ttu-id="84a22-308">Gibt an, wie viele Minuten sich das Gerät maximal im Leerlauf befinden darf, bevor eine PIN- oder Kennwortsperre aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="84a22-308">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="84a22-309">Gültig sind Ganzzahlen X, wobei gilt 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="84a22-309">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="84a22-310">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="84a22-310">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="84a22-311">Int32</span><span class="sxs-lookup"><span data-stu-id="84a22-311">Int32</span></span>|<span data-ttu-id="84a22-312">Offline-Intervall (in Tagen), nach dem die App-Daten gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="84a22-312">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="84a22-313">Antwort</span><span class="sxs-lookup"><span data-stu-id="84a22-313">Response</span></span>
<span data-ttu-id="84a22-314">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="84a22-314">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84a22-315">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84a22-315">Example</span></span>

### <a name="request"></a><span data-ttu-id="84a22-316">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84a22-316">Request</span></span>
<span data-ttu-id="84a22-317">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84a22-317">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
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

### <a name="response"></a><span data-ttu-id="84a22-318">Antwort</span><span class="sxs-lookup"><span data-stu-id="84a22-318">Response</span></span>
<span data-ttu-id="84a22-p133">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84a22-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




