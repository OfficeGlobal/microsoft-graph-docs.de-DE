---
title: Erstellen von „mdmWindowsInformationProtectionPolicy“
description: Erstellt neue Objekte des Typs mdmWindowsInformationProtectionPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74d2957925d168afca325f3b161e71d336cd4f7b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393158"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="3a13e-103">Erstellen von „mdmWindowsInformationProtectionPolicy“</span><span class="sxs-lookup"><span data-stu-id="3a13e-103">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="3a13e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3a13e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3a13e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3a13e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a13e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a13e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a13e-107">Diese Methode erstellt ein neues Objekt des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-107">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a13e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3a13e-108">Prerequisites</span></span>
<span data-ttu-id="3a13e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3a13e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a13e-111">Permission type</span></span>|<span data-ttu-id="3a13e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a13e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a13e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a13e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a13e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a13e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3a13e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a13e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a13e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a13e-116">Not supported.</span></span>|
|<span data-ttu-id="3a13e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a13e-117">Application</span></span>|<span data-ttu-id="3a13e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a13e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a13e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a13e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="3a13e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a13e-120">Request headers</span></span>
|<span data-ttu-id="3a13e-121">Header</span><span class="sxs-lookup"><span data-stu-id="3a13e-121">Header</span></span>|<span data-ttu-id="3a13e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3a13e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a13e-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3a13e-123">Authorization</span></span>|<span data-ttu-id="3a13e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3a13e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a13e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3a13e-125">Accept</span></span>|<span data-ttu-id="3a13e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a13e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a13e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a13e-127">Request body</span></span>
<span data-ttu-id="3a13e-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mdmWindowsInformationProtectionPolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="3a13e-128">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="3a13e-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mdmWindowsInformationProtectionPolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="3a13e-129">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="3a13e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3a13e-130">Property</span></span>|<span data-ttu-id="3a13e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3a13e-131">Type</span></span>|<span data-ttu-id="3a13e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a13e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a13e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3a13e-133">displayName</span></span>|<span data-ttu-id="3a13e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a13e-134">String</span></span>|<span data-ttu-id="3a13e-135">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3a13e-135">Policy display name.</span></span> <span data-ttu-id="3a13e-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a13e-137">description</span><span class="sxs-lookup"><span data-stu-id="3a13e-137">description</span></span>|<span data-ttu-id="3a13e-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a13e-138">String</span></span>|<span data-ttu-id="3a13e-139">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3a13e-139">The policy's description.</span></span> <span data-ttu-id="3a13e-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a13e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a13e-141">createdDateTime</span></span>|<span data-ttu-id="3a13e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a13e-142">DateTimeOffset</span></span>|<span data-ttu-id="3a13e-143">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3a13e-143">The date and time the policy was created.</span></span> <span data-ttu-id="3a13e-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a13e-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a13e-145">lastModifiedDateTime</span></span>|<span data-ttu-id="3a13e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a13e-146">DateTimeOffset</span></span>|<span data-ttu-id="3a13e-147">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3a13e-147">Last time the policy was modified.</span></span> <span data-ttu-id="3a13e-148">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a13e-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a13e-149">roleScopeTagIds</span></span>|<span data-ttu-id="3a13e-150">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="3a13e-150">String collection</span></span>|<span data-ttu-id="3a13e-151">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="3a13e-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3a13e-152">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a13e-153">id</span><span class="sxs-lookup"><span data-stu-id="3a13e-153">id</span></span>|<span data-ttu-id="3a13e-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a13e-154">String</span></span>|<span data-ttu-id="3a13e-155">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3a13e-155">Key of the entity.</span></span> <span data-ttu-id="3a13e-156">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a13e-157">Version</span><span class="sxs-lookup"><span data-stu-id="3a13e-157">version</span></span>|<span data-ttu-id="3a13e-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3a13e-158">String</span></span>|<span data-ttu-id="3a13e-159">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="3a13e-159">Version of the entity.</span></span> <span data-ttu-id="3a13e-160">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3a13e-161">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="3a13e-161">enforcementLevel</span></span>|[<span data-ttu-id="3a13e-162">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="3a13e-162">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="3a13e-163">WIP Erzwingung-Ebene. Siehe die Enum-Definition für unterstützte Werte Inherited aus [WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-163">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="3a13e-164">Mögliche Werte: sind `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt` und `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="3a13e-164">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="3a13e-165">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="3a13e-165">enterpriseDomain</span></span>|<span data-ttu-id="3a13e-166">String</span><span class="sxs-lookup"><span data-stu-id="3a13e-166">String</span></span>|<span data-ttu-id="3a13e-167">Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-167">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-168">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="3a13e-168">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="3a13e-169">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="3a13e-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3a13e-170">Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-170">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-171">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="3a13e-171">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="3a13e-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a13e-172">Boolean</span></span>|<span data-ttu-id="3a13e-173">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-173">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-174">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="3a13e-174">dataRecoveryCertificate</span></span>|[<span data-ttu-id="3a13e-175">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="3a13e-175">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="3a13e-176">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="3a13e-176">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="3a13e-177">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-177">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-178">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="3a13e-178">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="3a13e-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a13e-179">Boolean</span></span>|<span data-ttu-id="3a13e-180">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="3a13e-180">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="3a13e-181">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="3a13e-181">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="3a13e-182">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="3a13e-182">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="3a13e-183">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-183">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-184">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="3a13e-184">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="3a13e-185">Guid</span><span class="sxs-lookup"><span data-stu-id="3a13e-185">Guid</span></span>|<span data-ttu-id="3a13e-186">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="3a13e-186">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="3a13e-187">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-187">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-188">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="3a13e-188">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="3a13e-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a13e-189">Boolean</span></span>|<span data-ttu-id="3a13e-190">Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-190">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-191">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="3a13e-191">iconsVisible</span></span>|<span data-ttu-id="3a13e-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a13e-192">Boolean</span></span>|<span data-ttu-id="3a13e-193">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="3a13e-193">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="3a13e-194">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-194">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-195">protectedApps</span><span class="sxs-lookup"><span data-stu-id="3a13e-195">protectedApps</span></span>|<span data-ttu-id="3a13e-196">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="3a13e-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="3a13e-197">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-197">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-198">exemptApps</span><span class="sxs-lookup"><span data-stu-id="3a13e-198">exemptApps</span></span>|<span data-ttu-id="3a13e-199">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="3a13e-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="3a13e-200">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="3a13e-200">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="3a13e-201">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="3a13e-201">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="3a13e-202">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-202">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-203">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="3a13e-203">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="3a13e-204">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="3a13e-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3a13e-205">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="3a13e-205">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="3a13e-206">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-206">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-207">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="3a13e-207">enterpriseProxiedDomains</span></span>|<span data-ttu-id="3a13e-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3a13e-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="3a13e-209">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="3a13e-209">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="3a13e-210">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="3a13e-210">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="3a13e-211">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="3a13e-211">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="3a13e-212">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-212">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-213">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="3a13e-213">enterpriseIPRanges</span></span>|<span data-ttu-id="3a13e-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3a13e-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="3a13e-215">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="3a13e-215">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="3a13e-216">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="3a13e-216">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="3a13e-217">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-217">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-218">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="3a13e-218">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="3a13e-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a13e-219">Boolean</span></span>|<span data-ttu-id="3a13e-220">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="3a13e-220">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="3a13e-221">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-221">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-222">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="3a13e-222">enterpriseProxyServers</span></span>|<span data-ttu-id="3a13e-223">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="3a13e-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3a13e-224">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="3a13e-224">This is a list of proxy servers.</span></span> <span data-ttu-id="3a13e-225">Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-225">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-226">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="3a13e-226">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="3a13e-227">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="3a13e-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3a13e-228">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="3a13e-228">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="3a13e-229">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="3a13e-229">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="3a13e-230">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="3a13e-230">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="3a13e-231">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="3a13e-231">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="3a13e-232">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-232">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-233">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="3a13e-233">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="3a13e-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a13e-234">Boolean</span></span>|<span data-ttu-id="3a13e-235">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="3a13e-235">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="3a13e-236">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-236">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-237">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="3a13e-237">neutralDomainResources</span></span>|<span data-ttu-id="3a13e-238">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="3a13e-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3a13e-239">Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-239">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-240">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="3a13e-240">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="3a13e-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a13e-241">Boolean</span></span>|<span data-ttu-id="3a13e-242">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-242">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-243">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="3a13e-243">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="3a13e-244">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="3a13e-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3a13e-245">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-245">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3a13e-246">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3a13e-246">isAssigned</span></span>|<span data-ttu-id="3a13e-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a13e-247">Boolean</span></span>|<span data-ttu-id="3a13e-248">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3a13e-248">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="3a13e-249">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3a13e-249">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3a13e-250">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a13e-250">Response</span></span>
<span data-ttu-id="3a13e-251">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3a13e-251">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a13e-252">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a13e-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a13e-253">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a13e-253">Request</span></span>
<span data-ttu-id="3a13e-254">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a13e-254">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3967

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="3a13e-255">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a13e-255">Response</span></span>
<span data-ttu-id="3a13e-p124">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a13e-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4139

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




