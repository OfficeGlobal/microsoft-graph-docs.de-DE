---
title: windowsInformationProtection-Ressourcentyp
description: Richtlinie für Windows Information Protection zum Konfigurieren detaillierter Verwaltungseinstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35cbb531b2e2a3a48345870a939d7d5e05492b05
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172653"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="77656-103">windowsInformationProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="77656-103">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="77656-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77656-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77656-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="77656-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77656-106">Richtlinie für Windows Information Protection zum Konfigurieren detaillierter Verwaltungseinstellungen</span><span class="sxs-lookup"><span data-stu-id="77656-106">Policy for Windows information protection to configure detailed management settings</span></span>


<span data-ttu-id="77656-107">Erbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="77656-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="77656-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="77656-108">Methods</span></span>
|<span data-ttu-id="77656-109">Methode</span><span class="sxs-lookup"><span data-stu-id="77656-109">Method</span></span>|<span data-ttu-id="77656-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="77656-110">Return Type</span></span>|<span data-ttu-id="77656-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77656-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="77656-112">windowsInformationProtections auflisten</span><span class="sxs-lookup"><span data-stu-id="77656-112">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="77656-113">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="77656-113">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="77656-114">Listet die Eigenschaften und Beziehungen der [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)-Objekte auf.</span><span class="sxs-lookup"><span data-stu-id="77656-114">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="77656-115">windowsInformationProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="77656-115">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="77656-116">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="77656-116">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="77656-117">Liest die Eigenschaften und Beziehungen des [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)-Objekts auf.</span><span class="sxs-lookup"><span data-stu-id="77656-117">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="77656-118">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="77656-118">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="77656-119">Keine</span><span class="sxs-lookup"><span data-stu-id="77656-119">None</span></span>|<span data-ttu-id="77656-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="77656-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="77656-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77656-121">Properties</span></span>
|<span data-ttu-id="77656-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77656-122">Property</span></span>|<span data-ttu-id="77656-123">Typ</span><span class="sxs-lookup"><span data-stu-id="77656-123">Type</span></span>|<span data-ttu-id="77656-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77656-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77656-125">displayName</span><span class="sxs-lookup"><span data-stu-id="77656-125">displayName</span></span>|<span data-ttu-id="77656-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77656-126">String</span></span>|<span data-ttu-id="77656-127">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="77656-127">Policy display name.</span></span> <span data-ttu-id="77656-128">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="77656-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77656-129">description</span><span class="sxs-lookup"><span data-stu-id="77656-129">description</span></span>|<span data-ttu-id="77656-130">String</span><span class="sxs-lookup"><span data-stu-id="77656-130">String</span></span>|<span data-ttu-id="77656-131">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="77656-131">The policy's description.</span></span> <span data-ttu-id="77656-132">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="77656-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77656-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77656-133">createdDateTime</span></span>|<span data-ttu-id="77656-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77656-134">DateTimeOffset</span></span>|<span data-ttu-id="77656-135">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="77656-135">The date and time the policy was created.</span></span> <span data-ttu-id="77656-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="77656-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77656-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77656-137">lastModifiedDateTime</span></span>|<span data-ttu-id="77656-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77656-138">DateTimeOffset</span></span>|<span data-ttu-id="77656-139">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="77656-139">Last time the policy was modified.</span></span> <span data-ttu-id="77656-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="77656-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77656-141">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="77656-141">roleScopeTagIds</span></span>|<span data-ttu-id="77656-142">String collection</span><span class="sxs-lookup"><span data-stu-id="77656-142">String collection</span></span>|<span data-ttu-id="77656-143">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="77656-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="77656-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="77656-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77656-145">id</span><span class="sxs-lookup"><span data-stu-id="77656-145">id</span></span>|<span data-ttu-id="77656-146">string</span><span class="sxs-lookup"><span data-stu-id="77656-146">String</span></span>|<span data-ttu-id="77656-147">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="77656-147">Key of the entity.</span></span> <span data-ttu-id="77656-148">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="77656-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77656-149">Version</span><span class="sxs-lookup"><span data-stu-id="77656-149">version</span></span>|<span data-ttu-id="77656-150">String</span><span class="sxs-lookup"><span data-stu-id="77656-150">String</span></span>|<span data-ttu-id="77656-151">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="77656-151">Version of the entity.</span></span> <span data-ttu-id="77656-152">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="77656-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77656-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="77656-153">enforcementLevel</span></span>|[<span data-ttu-id="77656-154">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="77656-154">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="77656-155">WIP-Erzwingung. Siehe Enum-Definition für unterstützte Werte.</span><span class="sxs-lookup"><span data-stu-id="77656-155">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="77656-156">Mögliche Werte: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="77656-156">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="77656-157">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="77656-157">enterpriseDomain</span></span>|<span data-ttu-id="77656-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77656-158">String</span></span>|<span data-ttu-id="77656-159">Primäre Unternehmensdomäne</span><span class="sxs-lookup"><span data-stu-id="77656-159">Primary enterprise domain</span></span>|
|<span data-ttu-id="77656-160">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="77656-160">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="77656-161">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="77656-161">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="77656-162">Liste von Unternehmensdomänen, die geschützt werden sollen</span><span class="sxs-lookup"><span data-stu-id="77656-162">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="77656-163">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="77656-163">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="77656-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77656-164">Boolean</span></span>|<span data-ttu-id="77656-165">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss.</span><span class="sxs-lookup"><span data-stu-id="77656-165">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="77656-166">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="77656-166">dataRecoveryCertificate</span></span>|[<span data-ttu-id="77656-167">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="77656-167">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="77656-168">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="77656-168">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="77656-169">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem).</span><span class="sxs-lookup"><span data-stu-id="77656-169">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="77656-170">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="77656-170">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="77656-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77656-171">Boolean</span></span>|<span data-ttu-id="77656-172">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="77656-172">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="77656-173">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="77656-173">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="77656-174">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="77656-174">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="77656-175">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="77656-175">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="77656-176">Guid</span><span class="sxs-lookup"><span data-stu-id="77656-176">Guid</span></span>|<span data-ttu-id="77656-177">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="77656-177">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="77656-178">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind.</span><span class="sxs-lookup"><span data-stu-id="77656-178">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="77656-179">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="77656-179">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="77656-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="77656-180">Boolean</span></span>|<span data-ttu-id="77656-181">Gibt an, ob Azure RMS-Verschlüsselung für WIP zugelassen werden soll.</span><span class="sxs-lookup"><span data-stu-id="77656-181">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="77656-182">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="77656-182">iconsVisible</span></span>|<span data-ttu-id="77656-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77656-183">Boolean</span></span>|<span data-ttu-id="77656-184">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="77656-184">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="77656-185">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps.</span><span class="sxs-lookup"><span data-stu-id="77656-185">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="77656-186">protectedApps</span><span class="sxs-lookup"><span data-stu-id="77656-186">protectedApps</span></span>|<span data-ttu-id="77656-187">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="77656-187">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="77656-188">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt.</span><span class="sxs-lookup"><span data-stu-id="77656-188">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="77656-189">exemptApps</span><span class="sxs-lookup"><span data-stu-id="77656-189">exemptApps</span></span>|<span data-ttu-id="77656-190">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="77656-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="77656-191">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="77656-191">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="77656-192">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="77656-192">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="77656-193">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="77656-193">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="77656-194">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="77656-194">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="77656-195">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="77656-195">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="77656-196">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet.</span><span class="sxs-lookup"><span data-stu-id="77656-196">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="77656-197">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="77656-197">enterpriseProxiedDomains</span></span>|<span data-ttu-id="77656-198">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="77656-198">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="77656-199">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="77656-199">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="77656-200">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="77656-200">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="77656-201">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="77656-201">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="77656-202">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein.</span><span class="sxs-lookup"><span data-stu-id="77656-202">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="77656-203">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="77656-203">enterpriseIPRanges</span></span>|<span data-ttu-id="77656-204">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="77656-204">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="77656-205">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="77656-205">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="77656-206">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="77656-206">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="77656-207">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="77656-207">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="77656-208">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="77656-208">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="77656-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77656-209">Boolean</span></span>|<span data-ttu-id="77656-210">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="77656-210">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="77656-211">Der Standardwert ist „FALSE“.</span><span class="sxs-lookup"><span data-stu-id="77656-211">Default is false</span></span>|
|<span data-ttu-id="77656-212">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="77656-212">enterpriseProxyServers</span></span>|<span data-ttu-id="77656-213">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="77656-213">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="77656-214">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="77656-214">This is a list of proxy servers.</span></span> <span data-ttu-id="77656-215">Ein Server, der sich nicht in dieser Liste befindet, wird als unternehmensfremd betrachtet.</span><span class="sxs-lookup"><span data-stu-id="77656-215">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="77656-216">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="77656-216">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="77656-217">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="77656-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="77656-218">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="77656-218">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="77656-219">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="77656-219">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="77656-220">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="77656-220">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="77656-221">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="77656-221">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="77656-222">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="77656-222">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="77656-223">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="77656-223">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="77656-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="77656-224">Boolean</span></span>|<span data-ttu-id="77656-225">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="77656-225">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="77656-226">Der Standardwert ist „FALSE“.</span><span class="sxs-lookup"><span data-stu-id="77656-226">Default is false</span></span>|
|<span data-ttu-id="77656-227">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="77656-227">neutralDomainResources</span></span>|<span data-ttu-id="77656-228">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="77656-228">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="77656-229">Liste von Domänennamen, die für geschäftliche oder persönliche Ressourcen verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="77656-229">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="77656-230">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="77656-230">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="77656-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="77656-231">Boolean</span></span>|<span data-ttu-id="77656-232">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="77656-232">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="77656-233">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="77656-233">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="77656-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="77656-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="77656-235">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="77656-235">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="77656-236">isAssigned</span><span class="sxs-lookup"><span data-stu-id="77656-236">isAssigned</span></span>|<span data-ttu-id="77656-237">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77656-237">Boolean</span></span>|<span data-ttu-id="77656-238">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="77656-238">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77656-239">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="77656-239">Relationships</span></span>
|<span data-ttu-id="77656-240">Beziehung</span><span class="sxs-lookup"><span data-stu-id="77656-240">Relationship</span></span>|<span data-ttu-id="77656-241">Typ</span><span class="sxs-lookup"><span data-stu-id="77656-241">Type</span></span>|<span data-ttu-id="77656-242">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77656-242">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77656-243">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="77656-243">protectedAppLockerFiles</span></span>|<span data-ttu-id="77656-244">Sammlung von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="77656-244">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="77656-245">Eine weitere Möglichkeit zur Eingabe geschützter Apps über XML-Dateien.</span><span class="sxs-lookup"><span data-stu-id="77656-245">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="77656-246">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="77656-246">exemptAppLockerFiles</span></span>|<span data-ttu-id="77656-247">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="77656-247">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="77656-248">Eine weitere Möglichkeit zur Eingabe ausgenommener Apps über XML-Dateien.</span><span class="sxs-lookup"><span data-stu-id="77656-248">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="77656-249">assignments</span><span class="sxs-lookup"><span data-stu-id="77656-249">assignments</span></span>|<span data-ttu-id="77656-250">Sammlung von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="77656-250">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="77656-251">Navigationseigenschaft zu einer Liste der Sicherheitsgruppen, für die die Richtlinie gilt.</span><span class="sxs-lookup"><span data-stu-id="77656-251">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77656-252">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77656-252">JSON Representation</span></span>
<span data-ttu-id="77656-253">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77656-253">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true
}
```




