---
title: windowsInformationProtection-Ressourcentyp
description: Richtlinie für Windows Information Protection zum Konfigurieren detaillierter Verwaltungseinstellungen
ms.openlocfilehash: fed8a72a3d90a5dd016292272f691e025abe1a57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018271"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="be691-103">windowsInformationProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="be691-103">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="be691-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="be691-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be691-105">Richtlinie für Windows Information Protection zum Konfigurieren detaillierter Verwaltungseinstellungen</span><span class="sxs-lookup"><span data-stu-id="be691-105">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="be691-106">Erbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="be691-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="be691-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="be691-107">Methods</span></span>
|<span data-ttu-id="be691-108">Methode</span><span class="sxs-lookup"><span data-stu-id="be691-108">Method</span></span>|<span data-ttu-id="be691-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="be691-109">Return Type</span></span>|<span data-ttu-id="be691-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be691-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be691-111">windowsInformationProtections auflisten</span><span class="sxs-lookup"><span data-stu-id="be691-111">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="be691-112">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="be691-112">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="be691-113">Listet die Eigenschaften und Beziehungen der [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)-Objekte auf.</span><span class="sxs-lookup"><span data-stu-id="be691-113">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="be691-114">windowsInformationProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="be691-114">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="be691-115">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="be691-115">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="be691-116">Liest die Eigenschaften und Beziehungen des [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)-Objekts auf.</span><span class="sxs-lookup"><span data-stu-id="be691-116">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="be691-117">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="be691-117">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="be691-118">Keine</span><span class="sxs-lookup"><span data-stu-id="be691-118">None</span></span>|<span data-ttu-id="be691-119">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="be691-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="be691-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="be691-120">Properties</span></span>
|<span data-ttu-id="be691-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="be691-121">Property</span></span>|<span data-ttu-id="be691-122">Typ</span><span class="sxs-lookup"><span data-stu-id="be691-122">Type</span></span>|<span data-ttu-id="be691-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be691-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be691-124">displayName</span><span class="sxs-lookup"><span data-stu-id="be691-124">displayName</span></span>|<span data-ttu-id="be691-125">String</span><span class="sxs-lookup"><span data-stu-id="be691-125">String</span></span>|<span data-ttu-id="be691-126">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="be691-126">Policy display name.</span></span> <span data-ttu-id="be691-127">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="be691-127">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="be691-128">description</span><span class="sxs-lookup"><span data-stu-id="be691-128">description</span></span>|<span data-ttu-id="be691-129">String</span><span class="sxs-lookup"><span data-stu-id="be691-129">String</span></span>|<span data-ttu-id="be691-130">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="be691-130">The policy's description.</span></span> <span data-ttu-id="be691-131">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="be691-131">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="be691-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be691-132">createdDateTime</span></span>|<span data-ttu-id="be691-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be691-133">DateTimeOffset</span></span>|<span data-ttu-id="be691-134">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="be691-134">The date and time the policy was created.</span></span> <span data-ttu-id="be691-135">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="be691-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="be691-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be691-136">lastModifiedDateTime</span></span>|<span data-ttu-id="be691-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be691-137">DateTimeOffset</span></span>|<span data-ttu-id="be691-138">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="be691-138">Last time the policy was modified.</span></span> <span data-ttu-id="be691-139">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="be691-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="be691-140">id</span><span class="sxs-lookup"><span data-stu-id="be691-140">id</span></span>|<span data-ttu-id="be691-141">String</span><span class="sxs-lookup"><span data-stu-id="be691-141">String</span></span>|<span data-ttu-id="be691-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="be691-142">Key of the entity.</span></span> <span data-ttu-id="be691-143">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="be691-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="be691-144">Version</span><span class="sxs-lookup"><span data-stu-id="be691-144">version</span></span>|<span data-ttu-id="be691-145">String</span><span class="sxs-lookup"><span data-stu-id="be691-145">String</span></span>|<span data-ttu-id="be691-146">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="be691-146">Version of the entity.</span></span> <span data-ttu-id="be691-147">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="be691-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="be691-148">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="be691-148">enforcementLevel</span></span>|[<span data-ttu-id="be691-149">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="be691-149">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="be691-150">WIP Erzwingung-Ebene. Siehe die Enum-Definition für unterstützten Werte.</span><span class="sxs-lookup"><span data-stu-id="be691-150">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="be691-151">Mögliche Werte: sind `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt` und `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="be691-151">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="be691-152">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="be691-152">enterpriseDomain</span></span>|<span data-ttu-id="be691-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="be691-153">String</span></span>|<span data-ttu-id="be691-154">Primäre Unternehmensdomäne</span><span class="sxs-lookup"><span data-stu-id="be691-154">Primary enterprise domain</span></span>|
|<span data-ttu-id="be691-155">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="be691-155">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="be691-156">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="be691-156">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="be691-157">Liste von Unternehmensdomänen, die geschützt werden sollen</span><span class="sxs-lookup"><span data-stu-id="be691-157">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="be691-158">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="be691-158">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="be691-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="be691-159">Boolean</span></span>|<span data-ttu-id="be691-160">Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss.</span><span class="sxs-lookup"><span data-stu-id="be691-160">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="be691-161">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="be691-161">dataRecoveryCertificate</span></span>|[<span data-ttu-id="be691-162">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="be691-162">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="be691-163">Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="be691-163">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="be691-164">Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem).</span><span class="sxs-lookup"><span data-stu-id="be691-164">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="be691-165">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="be691-165">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="be691-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="be691-166">Boolean</span></span>|<span data-ttu-id="be691-167">Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="be691-167">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="be691-168">Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien.</span><span class="sxs-lookup"><span data-stu-id="be691-168">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="be691-169">Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="be691-169">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="be691-170">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="be691-170">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="be691-171">Guid</span><span class="sxs-lookup"><span data-stu-id="be691-171">Guid</span></span>|<span data-ttu-id="be691-172">GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="be691-172">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="be691-173">Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind.</span><span class="sxs-lookup"><span data-stu-id="be691-173">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="be691-174">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="be691-174">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="be691-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="be691-175">Boolean</span></span>|<span data-ttu-id="be691-176">Gibt an, ob Azure RMS-Verschlüsselung für WIP zugelassen werden soll.</span><span class="sxs-lookup"><span data-stu-id="be691-176">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="be691-177">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="be691-177">iconsVisible</span></span>|<span data-ttu-id="be691-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="be691-178">Boolean</span></span>|<span data-ttu-id="be691-179">Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="be691-179">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="be691-180">Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps.</span><span class="sxs-lookup"><span data-stu-id="be691-180">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="be691-181">protectedApps</span><span class="sxs-lookup"><span data-stu-id="be691-181">protectedApps</span></span>|<span data-ttu-id="be691-182">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="be691-182">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="be691-183">Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt.</span><span class="sxs-lookup"><span data-stu-id="be691-183">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="be691-184">exemptApps</span><span class="sxs-lookup"><span data-stu-id="be691-184">exemptApps</span></span>|<span data-ttu-id="be691-185">Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="be691-185">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="be691-186">Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt.</span><span class="sxs-lookup"><span data-stu-id="be691-186">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="be691-187">Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben.</span><span class="sxs-lookup"><span data-stu-id="be691-187">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="be691-188">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="be691-188">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="be691-189">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="be691-189">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="be691-190">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="be691-190">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="be691-191">Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet.</span><span class="sxs-lookup"><span data-stu-id="be691-191">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="be691-192">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="be691-192">enterpriseProxiedDomains</span></span>|<span data-ttu-id="be691-193">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="be691-193">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="be691-194">Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="be691-194">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="be691-195">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="be691-195">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="be691-196">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="be691-196">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="be691-197">Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein.</span><span class="sxs-lookup"><span data-stu-id="be691-197">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="be691-198">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="be691-198">enterpriseIPRanges</span></span>|<span data-ttu-id="be691-199">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="be691-199">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="be691-200">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="be691-200">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="be691-201">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="be691-201">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="be691-202">Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="be691-202">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="be691-203">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="be691-203">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="be691-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="be691-204">Boolean</span></span>|<span data-ttu-id="be691-205">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="be691-205">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="be691-206">Der Standardwert ist „FALSE“.</span><span class="sxs-lookup"><span data-stu-id="be691-206">Default is false</span></span>|
|<span data-ttu-id="be691-207">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="be691-207">enterpriseProxyServers</span></span>|<span data-ttu-id="be691-208">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="be691-208">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="be691-209">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="be691-209">This is a list of proxy servers.</span></span> <span data-ttu-id="be691-210">Ein Server, der sich nicht in dieser Liste befindet, wird als unternehmensfremd betrachtet.</span><span class="sxs-lookup"><span data-stu-id="be691-210">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="be691-211">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="be691-211">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="be691-212">Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="be691-212">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="be691-213">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="be691-213">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="be691-214">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="be691-214">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="be691-215">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="be691-215">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="be691-216">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="be691-216">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="be691-217">Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="be691-217">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="be691-218">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="be691-218">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="be691-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="be691-219">Boolean</span></span>|<span data-ttu-id="be691-220">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="be691-220">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="be691-221">Der Standardwert ist „FALSE“.</span><span class="sxs-lookup"><span data-stu-id="be691-221">Default is false</span></span>|
|<span data-ttu-id="be691-222">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="be691-222">neutralDomainResources</span></span>|<span data-ttu-id="be691-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="be691-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="be691-224">Liste von Domänennamen, die für geschäftliche oder persönliche Ressourcen verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="be691-224">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="be691-225">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="be691-225">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="be691-226">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="be691-226">Boolean</span></span>|<span data-ttu-id="be691-227">Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="be691-227">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="be691-228">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="be691-228">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="be691-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="be691-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="be691-230">Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="be691-230">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="be691-231">isAssigned</span><span class="sxs-lookup"><span data-stu-id="be691-231">isAssigned</span></span>|<span data-ttu-id="be691-232">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="be691-232">Boolean</span></span>|<span data-ttu-id="be691-233">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="be691-233">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be691-234">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="be691-234">Relationships</span></span>
|<span data-ttu-id="be691-235">Beziehung</span><span class="sxs-lookup"><span data-stu-id="be691-235">Relationship</span></span>|<span data-ttu-id="be691-236">Typ</span><span class="sxs-lookup"><span data-stu-id="be691-236">Type</span></span>|<span data-ttu-id="be691-237">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be691-237">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be691-238">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="be691-238">protectedAppLockerFiles</span></span>|<span data-ttu-id="be691-239">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="be691-239">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="be691-240">Eine weitere Möglichkeit zur Eingabe geschützter Apps über XML-Dateien.</span><span class="sxs-lookup"><span data-stu-id="be691-240">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="be691-241">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="be691-241">exemptAppLockerFiles</span></span>|<span data-ttu-id="be691-242">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="be691-242">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="be691-243">Eine weitere Möglichkeit zur Eingabe ausgenommener Apps über XML-Dateien.</span><span class="sxs-lookup"><span data-stu-id="be691-243">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="be691-244">assignments</span><span class="sxs-lookup"><span data-stu-id="be691-244">assignments</span></span>|<span data-ttu-id="be691-245">Sammlung von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="be691-245">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="be691-246">Navigationseigenschaft zu einer Liste der Sicherheitsgruppen, für die die Richtlinie gilt.</span><span class="sxs-lookup"><span data-stu-id="be691-246">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be691-247">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="be691-247">JSON Representation</span></span>
<span data-ttu-id="be691-248">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="be691-248">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
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



