---
title: Aktualisieren von windowsInformationProtectionPolicy
description: Aktualisiert die Eigenschaften von Objekten des Typs windowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: be1572ee72dad3bca83390290d4b45a39c82404c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949206"
---
# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="de8e4-103">Aktualisieren von windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="de8e4-103">Update windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="de8e4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="de8e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de8e4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="de8e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de8e4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="de8e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de8e4-107">Aktualisiert die Eigenschaften von Objekten des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-107">Update the properties of a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de8e4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="de8e4-108">Prerequisites</span></span>
<span data-ttu-id="de8e4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de8e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de8e4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="de8e4-111">Permission type</span></span>|<span data-ttu-id="de8e4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="de8e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de8e4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="de8e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de8e4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de8e4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="de8e4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="de8e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de8e4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de8e4-116">Not supported.</span></span>|
|<span data-ttu-id="de8e4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="de8e4-117">Application</span></span>|<span data-ttu-id="de8e4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de8e4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de8e4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="de8e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="de8e4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de8e4-120">Request headers</span></span>
|<span data-ttu-id="de8e4-121">Header</span><span class="sxs-lookup"><span data-stu-id="de8e4-121">Header</span></span>|<span data-ttu-id="de8e4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="de8e4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de8e4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de8e4-123">Authorization</span></span>|<span data-ttu-id="de8e4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="de8e4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de8e4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="de8e4-125">Accept</span></span>|<span data-ttu-id="de8e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de8e4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de8e4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de8e4-127">Request body</span></span>
<span data-ttu-id="de8e4-128">Geben Sie als Anforderungstext eine JSON-Darstellung eines Objekts des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) an.</span><span class="sxs-lookup"><span data-stu-id="de8e4-128">In the request body, supply a JSON representation for the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="de8e4-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="de8e4-129">The following table shows the properties that are required when you create the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="de8e4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="de8e4-130">Property</span></span>|<span data-ttu-id="de8e4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="de8e4-131">Type</span></span>|<span data-ttu-id="de8e4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de8e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de8e4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="de8e4-133">displayName</span></span>|<span data-ttu-id="de8e4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de8e4-134">String</span></span>|<span data-ttu-id="de8e4-135">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="de8e4-135">Policy display name.</span></span> <span data-ttu-id="de8e4-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de8e4-137">description</span><span class="sxs-lookup"><span data-stu-id="de8e4-137">description</span></span>|<span data-ttu-id="de8e4-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de8e4-138">String</span></span>|<span data-ttu-id="de8e4-139">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="de8e4-139">The policy's description.</span></span> <span data-ttu-id="de8e4-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de8e4-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de8e4-141">createdDateTime</span></span>|<span data-ttu-id="de8e4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de8e4-142">DateTimeOffset</span></span>|<span data-ttu-id="de8e4-143">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="de8e4-143">The date and time the policy was created.</span></span> <span data-ttu-id="de8e4-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de8e4-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de8e4-145">lastModifiedDateTime</span></span>|<span data-ttu-id="de8e4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de8e4-146">DateTimeOffset</span></span>|<span data-ttu-id="de8e4-147">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="de8e4-147">Last time the policy was modified.</span></span> <span data-ttu-id="de8e4-148">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de8e4-149">id</span><span class="sxs-lookup"><span data-stu-id="de8e4-149">id</span></span>|<span data-ttu-id="de8e4-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de8e4-150">String</span></span>|<span data-ttu-id="de8e4-151">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="de8e4-151">Key of the entity.</span></span> <span data-ttu-id="de8e4-152">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de8e4-153">Version</span><span class="sxs-lookup"><span data-stu-id="de8e4-153">version</span></span>|<span data-ttu-id="de8e4-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de8e4-154">String</span></span>|<span data-ttu-id="de8e4-155">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="de8e4-155">Version of the entity.</span></span> <span data-ttu-id="de8e4-156">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de8e4-157">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="de8e4-157">enforcementLevel</span></span>|[<span data-ttu-id="de8e4-158">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="de8e4-158">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="de8e4-159">WIP Erzwingung-Ebene. Siehe die Enum-Definition für unterstützte Werte Inherited aus [WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-159">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="de8e4-160">Mögliche Werte: sind `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt` und `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="de8e4-160">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="de8e4-161">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="de8e4-161">enterpriseDomain</span></span>|<span data-ttu-id="de8e4-162">String</span><span class="sxs-lookup"><span data-stu-id="de8e4-162">String</span></span>|<span data-ttu-id="de8e4-163">Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-163">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-164">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="de8e4-164">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="de8e4-165">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="de8e4-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de8e4-166">Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-166">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-167">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="de8e4-167">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="de8e4-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de8e4-168">Boolean</span></span>|<span data-ttu-id="de8e4-169">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-169">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-170">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="de8e4-170">dataRecoveryCertificate</span></span>|[<span data-ttu-id="de8e4-171">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="de8e4-171">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="de8e4-172">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="de8e4-172">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="de8e4-173">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-173">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-174">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="de8e4-174">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="de8e4-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de8e4-175">Boolean</span></span>|<span data-ttu-id="de8e4-176">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="de8e4-176">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="de8e4-177">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="de8e4-177">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="de8e4-178">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="de8e4-178">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="de8e4-179">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-179">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-180">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="de8e4-180">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="de8e4-181">Guid</span><span class="sxs-lookup"><span data-stu-id="de8e4-181">Guid</span></span>|<span data-ttu-id="de8e4-182">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="de8e4-182">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="de8e4-183">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-183">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-184">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="de8e4-184">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="de8e4-185">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de8e4-185">Boolean</span></span>|<span data-ttu-id="de8e4-186">Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-186">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-187">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="de8e4-187">iconsVisible</span></span>|<span data-ttu-id="de8e4-188">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de8e4-188">Boolean</span></span>|<span data-ttu-id="de8e4-189">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="de8e4-189">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="de8e4-190">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-190">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-191">protectedApps</span><span class="sxs-lookup"><span data-stu-id="de8e4-191">protectedApps</span></span>|<span data-ttu-id="de8e4-192">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="de8e4-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="de8e4-193">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-193">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-194">exemptApps</span><span class="sxs-lookup"><span data-stu-id="de8e4-194">exemptApps</span></span>|<span data-ttu-id="de8e4-195">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="de8e4-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="de8e4-196">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="de8e4-196">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="de8e4-197">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="de8e4-197">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="de8e4-198">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-198">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-199">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="de8e4-199">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="de8e4-200">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="de8e4-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de8e4-201">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="de8e4-201">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="de8e4-202">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-202">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-203">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="de8e4-203">enterpriseProxiedDomains</span></span>|<span data-ttu-id="de8e4-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="de8e4-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="de8e4-205">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="de8e4-205">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="de8e4-206">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="de8e4-206">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="de8e4-207">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="de8e4-207">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="de8e4-208">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-208">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-209">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="de8e4-209">enterpriseIPRanges</span></span>|<span data-ttu-id="de8e4-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="de8e4-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="de8e4-211">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="de8e4-211">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="de8e4-212">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="de8e4-212">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="de8e4-213">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-213">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-214">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="de8e4-214">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="de8e4-215">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de8e4-215">Boolean</span></span>|<span data-ttu-id="de8e4-216">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="de8e4-216">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="de8e4-217">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-217">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-218">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="de8e4-218">enterpriseProxyServers</span></span>|<span data-ttu-id="de8e4-219">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="de8e4-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de8e4-220">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="de8e4-220">This is a list of proxy servers.</span></span> <span data-ttu-id="de8e4-221">Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-221">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-222">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="de8e4-222">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="de8e4-223">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="de8e4-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de8e4-224">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="de8e4-224">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="de8e4-225">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="de8e4-225">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="de8e4-226">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="de8e4-226">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="de8e4-227">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="de8e4-227">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="de8e4-228">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-228">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-229">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="de8e4-229">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="de8e4-230">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de8e4-230">Boolean</span></span>|<span data-ttu-id="de8e4-231">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="de8e4-231">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="de8e4-232">Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-232">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-233">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="de8e4-233">neutralDomainResources</span></span>|<span data-ttu-id="de8e4-234">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="de8e4-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de8e4-235">Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-235">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-236">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="de8e4-236">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="de8e4-237">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de8e4-237">Boolean</span></span>|<span data-ttu-id="de8e4-238">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-238">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-239">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="de8e4-239">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="de8e4-240">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="de8e4-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de8e4-241">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-241">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-242">isAssigned</span><span class="sxs-lookup"><span data-stu-id="de8e4-242">isAssigned</span></span>|<span data-ttu-id="de8e4-243">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de8e4-243">Boolean</span></span>|<span data-ttu-id="de8e4-244">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="de8e4-244">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="de8e4-245">Geerbt von [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="de8e4-245">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de8e4-246">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="de8e4-246">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="de8e4-247">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de8e4-247">Boolean</span></span>|<span data-ttu-id="de8e4-248">Neue Eigenschaft in RS2. Dokumentation noch ausstehend.</span><span class="sxs-lookup"><span data-stu-id="de8e4-248">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="de8e4-249">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="de8e4-249">mdmEnrollmentUrl</span></span>|<span data-ttu-id="de8e4-250">String</span><span class="sxs-lookup"><span data-stu-id="de8e4-250">String</span></span>|<span data-ttu-id="de8e4-251">URL zur Registrierung in der MDM-Lösung</span><span class="sxs-lookup"><span data-stu-id="de8e4-251">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="de8e4-252">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="de8e4-252">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="de8e4-253">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de8e4-253">Boolean</span></span>|<span data-ttu-id="de8e4-254">Boolescher Wert, der Windows Hello for Business als Methode für die Anmeldung bei Windows festlegt</span><span class="sxs-lookup"><span data-stu-id="de8e4-254">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="de8e4-255">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="de8e4-255">pinMinimumLength</span></span>|<span data-ttu-id="de8e4-256">Int32</span><span class="sxs-lookup"><span data-stu-id="de8e4-256">Int32</span></span>|<span data-ttu-id="de8e4-257">Ganze Zahl, die festlegt, wie viele Zeichen die PIN mindestens haben muss.</span><span class="sxs-lookup"><span data-stu-id="de8e4-257">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="de8e4-258">Der Standardwert ist „4“.</span><span class="sxs-lookup"><span data-stu-id="de8e4-258">Default value is 4.</span></span> <span data-ttu-id="de8e4-259">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 4.</span><span class="sxs-lookup"><span data-stu-id="de8e4-259">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="de8e4-260">Die größte Zahl, die Sie konfigurieren können, muss kleiner sein als die Zahl, die Sie für die Richtlinieneinstellung zur Festlegung der PIN-Maximallänge angegeben haben, oder kleiner als 127 (je nachdem, welche Zahl kleiner ist).</span><span class="sxs-lookup"><span data-stu-id="de8e4-260">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="de8e4-261">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="de8e4-261">pinUppercaseLetters</span></span>|[<span data-ttu-id="de8e4-262">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="de8e4-262">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="de8e4-263">Ganzzahlwert, der konfiguriert, ob Großbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="de8e4-263">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="de8e4-264">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="de8e4-264">Default is NotAllow.</span></span> <span data-ttu-id="de8e4-265">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="de8e4-265">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="de8e4-266">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="de8e4-266">pinLowercaseLetters</span></span>|[<span data-ttu-id="de8e4-267">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="de8e4-267">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="de8e4-268">Ganzzahlwert, der konfiguriert, ob Kleinbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="de8e4-268">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="de8e4-269">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="de8e4-269">Default is NotAllow.</span></span> <span data-ttu-id="de8e4-270">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="de8e4-270">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="de8e4-271">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="de8e4-271">pinSpecialCharacters</span></span>|[<span data-ttu-id="de8e4-272">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="de8e4-272">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="de8e4-273">Ganzzahlwert, der konfiguriert, ob Sonderzeichen in der Windows Hello for Business-PIN verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="de8e4-273">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="de8e4-274">Zu den zulässigen Sonderzeichen für Windows Hello for Business-Gesten gehören: !</span><span class="sxs-lookup"><span data-stu-id="de8e4-274">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="de8e4-275">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="de8e4-275">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="de8e4-276">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="de8e4-276">/ : ; < = > ?</span></span><span data-ttu-id="de8e4-277"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="de8e4-277"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="de8e4-278">} ~.</span><span class="sxs-lookup"><span data-stu-id="de8e4-278">} ~.</span></span> <span data-ttu-id="de8e4-279">Der Standardwert lautet „NotAllow“.</span><span class="sxs-lookup"><span data-stu-id="de8e4-279">Default is NotAllow.</span></span> <span data-ttu-id="de8e4-280">Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.</span><span class="sxs-lookup"><span data-stu-id="de8e4-280">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="de8e4-281">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="de8e4-281">pinExpirationDays</span></span>|<span data-ttu-id="de8e4-282">Int32</span><span class="sxs-lookup"><span data-stu-id="de8e4-282">Int32</span></span>|<span data-ttu-id="de8e4-283">Ganzzahlwert, der angibt, wie viele Tage die PIN verwendet werden darf, bevor das System den Benutzer auffordert, sie zu ändern.</span><span class="sxs-lookup"><span data-stu-id="de8e4-283">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="de8e4-284">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 730.</span><span class="sxs-lookup"><span data-stu-id="de8e4-284">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="de8e4-285">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="de8e4-285">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="de8e4-286">Wenn Sie für diese Richtlinie „0“ festlegen, läuft die PIN des Benutzers niemals ab.</span><span class="sxs-lookup"><span data-stu-id="de8e4-286">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="de8e4-287">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="de8e4-287">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="de8e4-288">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="de8e4-288">Default is 0.</span></span>|
|<span data-ttu-id="de8e4-289">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="de8e4-289">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="de8e4-290">Int32</span><span class="sxs-lookup"><span data-stu-id="de8e4-290">Int32</span></span>|<span data-ttu-id="de8e4-291">Ganzzahlwert, der angibt, wie viele der zuletzt dem Benutzerkonto zugeordneten PINs nicht wiederverwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="de8e4-291">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="de8e4-292">Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 50.</span><span class="sxs-lookup"><span data-stu-id="de8e4-292">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="de8e4-293">Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0.</span><span class="sxs-lookup"><span data-stu-id="de8e4-293">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="de8e4-294">Wenn Sie für diese Richtlinie „0“ festlegen, wird keine Speicherung früherer PINs erzwungen.</span><span class="sxs-lookup"><span data-stu-id="de8e4-294">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="de8e4-295">Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="de8e4-295">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="de8e4-296">Der Standardwert lautet „0“.</span><span class="sxs-lookup"><span data-stu-id="de8e4-296">Default is 0.</span></span>|
|<span data-ttu-id="de8e4-297">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="de8e4-297">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="de8e4-298">Int32</span><span class="sxs-lookup"><span data-stu-id="de8e4-298">Int32</span></span>|<span data-ttu-id="de8e4-299">Legt fest, wie oft die Authentifizierung fehlschlagen darf, bevor das Gerät zurückgesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="de8e4-299">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="de8e4-300">Ein Wert von „0“ deaktiviert die Funktion zur Gerätezurücksetzung.</span><span class="sxs-lookup"><span data-stu-id="de8e4-300">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="de8e4-301">Gültig sind Ganzzahlen X, wobei gilt 4 <= X <= 16 für Desktops und 0 <= X <= 999 für Mobilgeräte.</span><span class="sxs-lookup"><span data-stu-id="de8e4-301">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="de8e4-302">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="de8e4-302">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="de8e4-303">Int32</span><span class="sxs-lookup"><span data-stu-id="de8e4-303">Int32</span></span>|<span data-ttu-id="de8e4-304">Gibt an, wie viele Minuten sich das Gerät maximal im Leerlauf befinden darf, bevor eine PIN- oder Kennwortsperre aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="de8e4-304">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="de8e4-305">Gültig sind Ganzzahlen X, wobei gilt 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="de8e4-305">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="de8e4-306">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="de8e4-306">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="de8e4-307">Int32</span><span class="sxs-lookup"><span data-stu-id="de8e4-307">Int32</span></span>|<span data-ttu-id="de8e4-308">Offline-Intervall (in Tagen), nach dem die App-Daten gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="de8e4-308">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="de8e4-309">Antwort</span><span class="sxs-lookup"><span data-stu-id="de8e4-309">Response</span></span>
<span data-ttu-id="de8e4-310">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="de8e4-310">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de8e4-311">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de8e4-311">Example</span></span>
### <a name="request"></a><span data-ttu-id="de8e4-312">Anforderung</span><span class="sxs-lookup"><span data-stu-id="de8e4-312">Request</span></span>
<span data-ttu-id="de8e4-313">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de8e4-313">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 4396

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

### <a name="response"></a><span data-ttu-id="de8e4-314">Antwort</span><span class="sxs-lookup"><span data-stu-id="de8e4-314">Response</span></span>
<span data-ttu-id="de8e4-p132">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de8e4-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





