---
title: Aktualisieren von „mdmWindowsInformationProtectionPolicy“
description: Aktualisiert die Eigenschaften von Objekten des Typs mdmWindowsInformationProtectionPolicy.
author: tfitzmac
ms.openlocfilehash: e4b05831f91336cb5adafb6840b77a2120e6a42b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308631"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="2c4d5-103">Aktualisieren von „mdmWindowsInformationProtectionPolicy“</span><span class="sxs-lookup"><span data-stu-id="2c4d5-103">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="2c4d5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c4d5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c4d5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c4d5-107">Aktualisiert die Eigenschaften von Objekten des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-107">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2c4d5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2c4d5-108">Prerequisites</span></span>
<span data-ttu-id="2c4d5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c4d5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2c4d5-111">Permission type</span></span>|<span data-ttu-id="2c4d5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2c4d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c4d5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2c4d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c4d5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c4d5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2c4d5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2c4d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c4d5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c4d5-116">Not supported.</span></span>|
|<span data-ttu-id="2c4d5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2c4d5-117">Application</span></span>|<span data-ttu-id="2c4d5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c4d5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c4d5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c4d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="2c4d5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2c4d5-120">Request headers</span></span>
|<span data-ttu-id="2c4d5-121">Header</span><span class="sxs-lookup"><span data-stu-id="2c4d5-121">Header</span></span>|<span data-ttu-id="2c4d5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2c4d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c4d5-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2c4d5-123">Authorization</span></span>|<span data-ttu-id="2c4d5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2c4d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c4d5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2c4d5-125">Accept</span></span>|<span data-ttu-id="2c4d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c4d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c4d5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2c4d5-127">Request body</span></span>
<span data-ttu-id="2c4d5-128">Geben Sie als Anforderungstext eine JSON-Darstellung eines [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-128">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="2c4d5-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)-Objekt erstellen.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-129">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="2c4d5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2c4d5-130">Property</span></span>|<span data-ttu-id="2c4d5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2c4d5-131">Type</span></span>|<span data-ttu-id="2c4d5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c4d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c4d5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2c4d5-133">displayName</span></span>|<span data-ttu-id="2c4d5-134">String</span><span class="sxs-lookup"><span data-stu-id="2c4d5-134">String</span></span>|<span data-ttu-id="2c4d5-135">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2c4d5-135">Policy display name.</span></span> <span data-ttu-id="2c4d5-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c4d5-137">description</span><span class="sxs-lookup"><span data-stu-id="2c4d5-137">description</span></span>|<span data-ttu-id="2c4d5-138">String</span><span class="sxs-lookup"><span data-stu-id="2c4d5-138">String</span></span>|<span data-ttu-id="2c4d5-139">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2c4d5-139">The policy's description.</span></span> <span data-ttu-id="2c4d5-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c4d5-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c4d5-141">createdDateTime</span></span>|<span data-ttu-id="2c4d5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c4d5-142">DateTimeOffset</span></span>|<span data-ttu-id="2c4d5-143">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2c4d5-143">The date and time the policy was created.</span></span> <span data-ttu-id="2c4d5-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c4d5-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c4d5-145">lastModifiedDateTime</span></span>|<span data-ttu-id="2c4d5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c4d5-146">DateTimeOffset</span></span>|<span data-ttu-id="2c4d5-147">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2c4d5-147">Last time the policy was modified.</span></span> <span data-ttu-id="2c4d5-148">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c4d5-149">id</span><span class="sxs-lookup"><span data-stu-id="2c4d5-149">id</span></span>|<span data-ttu-id="2c4d5-150">String</span><span class="sxs-lookup"><span data-stu-id="2c4d5-150">String</span></span>|<span data-ttu-id="2c4d5-151">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2c4d5-151">Key of the entity.</span></span> <span data-ttu-id="2c4d5-152">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c4d5-153">Version</span><span class="sxs-lookup"><span data-stu-id="2c4d5-153">version</span></span>|<span data-ttu-id="2c4d5-154">String</span><span class="sxs-lookup"><span data-stu-id="2c4d5-154">String</span></span>|<span data-ttu-id="2c4d5-155">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="2c4d5-155">Version of the entity.</span></span> <span data-ttu-id="2c4d5-156">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c4d5-157">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="2c4d5-157">enforcementLevel</span></span>|[<span data-ttu-id="2c4d5-158">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="2c4d5-158">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="2c4d5-159">WIP Erzwingung-Ebene. Siehe die Enum-Definition für unterstützte Werte Inherited aus [WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-159">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="2c4d5-160">Mögliche Werte: sind `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt` und `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-160">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="2c4d5-161">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="2c4d5-161">enterpriseDomain</span></span>|<span data-ttu-id="2c4d5-162">String</span><span class="sxs-lookup"><span data-stu-id="2c4d5-162">String</span></span>|<span data-ttu-id="2c4d5-163">Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-163">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-164">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="2c4d5-164">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="2c4d5-165">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="2c4d5-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2c4d5-166">Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-166">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-167">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="2c4d5-167">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="2c4d5-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2c4d5-168">Boolean</span></span>|<span data-ttu-id="2c4d5-169">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-169">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-170">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="2c4d5-170">dataRecoveryCertificate</span></span>|[<span data-ttu-id="2c4d5-171">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="2c4d5-171">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="2c4d5-172">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-172">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="2c4d5-173">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-173">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-174">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="2c4d5-174">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="2c4d5-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2c4d5-175">Boolean</span></span>|<span data-ttu-id="2c4d5-176">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-176">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="2c4d5-177">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-177">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="2c4d5-178">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-178">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="2c4d5-179">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-179">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-180">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="2c4d5-180">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="2c4d5-181">Guid</span><span class="sxs-lookup"><span data-stu-id="2c4d5-181">Guid</span></span>|<span data-ttu-id="2c4d5-182">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-182">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="2c4d5-183">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-183">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-184">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="2c4d5-184">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="2c4d5-185">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2c4d5-185">Boolean</span></span>|<span data-ttu-id="2c4d5-186">Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-186">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-187">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="2c4d5-187">iconsVisible</span></span>|<span data-ttu-id="2c4d5-188">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2c4d5-188">Boolean</span></span>|<span data-ttu-id="2c4d5-189">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-189">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="2c4d5-190">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-190">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-191">protectedApps</span><span class="sxs-lookup"><span data-stu-id="2c4d5-191">protectedApps</span></span>|<span data-ttu-id="2c4d5-192">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c4d5-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="2c4d5-193">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-193">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-194">exemptApps</span><span class="sxs-lookup"><span data-stu-id="2c4d5-194">exemptApps</span></span>|<span data-ttu-id="2c4d5-195">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c4d5-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="2c4d5-196">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-196">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="2c4d5-197">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-197">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="2c4d5-198">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-198">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-199">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="2c4d5-199">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="2c4d5-200">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="2c4d5-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2c4d5-201">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-201">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="2c4d5-202">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-202">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-203">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="2c4d5-203">enterpriseProxiedDomains</span></span>|<span data-ttu-id="2c4d5-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2c4d5-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="2c4d5-205">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-205">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="2c4d5-206">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-206">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="2c4d5-207">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-207">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="2c4d5-208">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-208">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-209">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="2c4d5-209">enterpriseIPRanges</span></span>|<span data-ttu-id="2c4d5-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2c4d5-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="2c4d5-211">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-211">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="2c4d5-212">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-212">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="2c4d5-213">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-213">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-214">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="2c4d5-214">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="2c4d5-215">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2c4d5-215">Boolean</span></span>|<span data-ttu-id="2c4d5-216">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-216">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="2c4d5-217">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-217">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-218">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="2c4d5-218">enterpriseProxyServers</span></span>|<span data-ttu-id="2c4d5-219">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="2c4d5-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2c4d5-220">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-220">This is a list of proxy servers.</span></span> <span data-ttu-id="2c4d5-221">Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-221">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-222">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="2c4d5-222">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="2c4d5-223">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="2c4d5-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2c4d5-224">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-224">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="2c4d5-225">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-225">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="2c4d5-226">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-226">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="2c4d5-227">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-227">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="2c4d5-228">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-228">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-229">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="2c4d5-229">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="2c4d5-230">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2c4d5-230">Boolean</span></span>|<span data-ttu-id="2c4d5-231">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-231">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="2c4d5-232">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-232">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-233">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="2c4d5-233">neutralDomainResources</span></span>|<span data-ttu-id="2c4d5-234">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="2c4d5-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2c4d5-235">Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-235">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-236">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="2c4d5-236">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="2c4d5-237">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2c4d5-237">Boolean</span></span>|<span data-ttu-id="2c4d5-238">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-238">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-239">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="2c4d5-239">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="2c4d5-240">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="2c4d5-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="2c4d5-241">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-241">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="2c4d5-242">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2c4d5-242">isAssigned</span></span>|<span data-ttu-id="2c4d5-243">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2c4d5-243">Boolean</span></span>|<span data-ttu-id="2c4d5-244">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-244">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="2c4d5-245">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2c4d5-245">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2c4d5-246">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c4d5-246">Response</span></span>
<span data-ttu-id="2c4d5-247">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-247">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c4d5-248">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2c4d5-248">Example</span></span>
### <a name="request"></a><span data-ttu-id="2c4d5-249">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c4d5-249">Request</span></span>
<span data-ttu-id="2c4d5-250">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 3893

{
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

### <a name="response"></a><span data-ttu-id="2c4d5-251">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c4d5-251">Response</span></span>
<span data-ttu-id="2c4d5-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2c4d5-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





