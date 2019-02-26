---
title: Aktualisieren von „windows10EndpointProtectionConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8070bbce1849aa2797a45989baf550bd581b558
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260529"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="eddc2-103">Aktualisieren von „windows10EndpointProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="eddc2-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="eddc2-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="eddc2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eddc2-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eddc2-105">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eddc2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eddc2-106">Prerequisites</span></span>
<span data-ttu-id="eddc2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="eddc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eddc2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eddc2-109">Permission type</span></span>|<span data-ttu-id="eddc2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eddc2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eddc2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eddc2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eddc2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eddc2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eddc2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eddc2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eddc2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eddc2-114">Not supported.</span></span>|
|<span data-ttu-id="eddc2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eddc2-115">Application</span></span>|<span data-ttu-id="eddc2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eddc2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eddc2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eddc2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="eddc2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eddc2-118">Request headers</span></span>
|<span data-ttu-id="eddc2-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eddc2-119">Header</span></span>|<span data-ttu-id="eddc2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="eddc2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eddc2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eddc2-121">Authorization</span></span>|<span data-ttu-id="eddc2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eddc2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eddc2-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eddc2-123">Accept</span></span>|<span data-ttu-id="eddc2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eddc2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eddc2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eddc2-125">Request body</span></span>
<span data-ttu-id="eddc2-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="eddc2-126">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="eddc2-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="eddc2-127">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="eddc2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eddc2-128">Property</span></span>|<span data-ttu-id="eddc2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="eddc2-129">Type</span></span>|<span data-ttu-id="eddc2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eddc2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eddc2-131">id</span><span class="sxs-lookup"><span data-stu-id="eddc2-131">id</span></span>|<span data-ttu-id="eddc2-132">string</span><span class="sxs-lookup"><span data-stu-id="eddc2-132">String</span></span>|<span data-ttu-id="eddc2-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="eddc2-133">Key of the entity.</span></span> <span data-ttu-id="eddc2-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eddc2-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eddc2-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eddc2-135">lastModifiedDateTime</span></span>|<span data-ttu-id="eddc2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eddc2-136">DateTimeOffset</span></span>|<span data-ttu-id="eddc2-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="eddc2-137">DateTime the object was last modified.</span></span> <span data-ttu-id="eddc2-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eddc2-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eddc2-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eddc2-139">createdDateTime</span></span>|<span data-ttu-id="eddc2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eddc2-140">DateTimeOffset</span></span>|<span data-ttu-id="eddc2-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="eddc2-141">DateTime the object was created.</span></span> <span data-ttu-id="eddc2-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eddc2-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eddc2-143">description</span><span class="sxs-lookup"><span data-stu-id="eddc2-143">description</span></span>|<span data-ttu-id="eddc2-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eddc2-144">String</span></span>|<span data-ttu-id="eddc2-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="eddc2-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eddc2-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eddc2-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eddc2-147">displayName</span><span class="sxs-lookup"><span data-stu-id="eddc2-147">displayName</span></span>|<span data-ttu-id="eddc2-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eddc2-148">String</span></span>|<span data-ttu-id="eddc2-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="eddc2-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eddc2-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eddc2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eddc2-151">Version</span><span class="sxs-lookup"><span data-stu-id="eddc2-151">version</span></span>|<span data-ttu-id="eddc2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="eddc2-152">Int32</span></span>|<span data-ttu-id="eddc2-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="eddc2-153">Version of the device configuration.</span></span> <span data-ttu-id="eddc2-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eddc2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eddc2-155">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="eddc2-155">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="eddc2-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-156">Boolean</span></span>|<span data-ttu-id="eddc2-157">Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="eddc2-157">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="eddc2-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="eddc2-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="eddc2-159">Int32</span><span class="sxs-lookup"><span data-stu-id="eddc2-159">Int32</span></span>|<span data-ttu-id="eddc2-160">Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600.</span><span class="sxs-lookup"><span data-stu-id="eddc2-160">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="eddc2-161">Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="eddc2-161">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="eddc2-162">Gültige Werte: 300 bis 3600.</span><span class="sxs-lookup"><span data-stu-id="eddc2-162">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="eddc2-163">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="eddc2-163">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="eddc2-164">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="eddc2-164">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="eddc2-165">Wählen Sie die zu verwendende vorinstallierte Tasten Codierung aus.</span><span class="sxs-lookup"><span data-stu-id="eddc2-165">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="eddc2-166">Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.</span><span class="sxs-lookup"><span data-stu-id="eddc2-166">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="eddc2-167">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="eddc2-167">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="eddc2-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-168">Boolean</span></span>|<span data-ttu-id="eddc2-169">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="eddc2-169">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="eddc2-170">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="eddc2-170">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="eddc2-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-171">Boolean</span></span>|<span data-ttu-id="eddc2-172">Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="eddc2-172">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="eddc2-173">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="eddc2-173">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="eddc2-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-174">Boolean</span></span>|<span data-ttu-id="eddc2-175">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="eddc2-175">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="eddc2-176">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="eddc2-176">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="eddc2-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-177">Boolean</span></span>|<span data-ttu-id="eddc2-178">Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="eddc2-178">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="eddc2-179">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="eddc2-179">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="eddc2-180">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="eddc2-180">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="eddc2-181">Geben Sie an, wie die Zertifikatssperrliste erzwungen werden soll.</span><span class="sxs-lookup"><span data-stu-id="eddc2-181">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="eddc2-182">Mögliche Werte: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="eddc2-182">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="eddc2-183">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="eddc2-183">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="eddc2-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-184">Boolean</span></span>|<span data-ttu-id="eddc2-185">Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.</span><span class="sxs-lookup"><span data-stu-id="eddc2-185">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="eddc2-186">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="eddc2-186">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="eddc2-187">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="eddc2-187">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="eddc2-188">Konfiguriert, wie Paketwarteschlangen im Tunnel Gateway-Szenario angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="eddc2-188">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="eddc2-189">Mögliche Werte: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="eddc2-189">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="eddc2-190">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="eddc2-190">firewallProfileDomain</span></span>|[<span data-ttu-id="eddc2-191">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="eddc2-191">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="eddc2-192">Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.</span><span class="sxs-lookup"><span data-stu-id="eddc2-192">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="eddc2-193">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="eddc2-193">firewallProfilePublic</span></span>|[<span data-ttu-id="eddc2-194">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="eddc2-194">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="eddc2-195">Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="eddc2-195">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="eddc2-196">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="eddc2-196">firewallProfilePrivate</span></span>|[<span data-ttu-id="eddc2-197">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="eddc2-197">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="eddc2-198">Konfiguriert die Firewallprofileinstellungen für private Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="eddc2-198">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="eddc2-199">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="eddc2-199">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="eddc2-200">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="eddc2-200">String collection</span></span>|<span data-ttu-id="eddc2-201">Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="eddc2-201">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="eddc2-202">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="eddc2-202">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="eddc2-203">String collection</span><span class="sxs-lookup"><span data-stu-id="eddc2-203">String collection</span></span>|<span data-ttu-id="eddc2-204">Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen.
</span><span class="sxs-lookup"><span data-stu-id="eddc2-204">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="eddc2-205">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="eddc2-205">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="eddc2-206">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="eddc2-206">String collection</span></span>|<span data-ttu-id="eddc2-207">Liste von Ordnerpfaden, die der Liste geschützter Ordner hinzugefügt werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="eddc2-207">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="eddc2-208">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="eddc2-208">defenderExploitProtectionXml</span></span>|<span data-ttu-id="eddc2-209">Binär</span><span class="sxs-lookup"><span data-stu-id="eddc2-209">Binary</span></span>|<span data-ttu-id="eddc2-210">XML-Inhalte mit Details zum Exploit-Schutz.
</span><span class="sxs-lookup"><span data-stu-id="eddc2-210">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="eddc2-211">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="eddc2-211">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="eddc2-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eddc2-212">String</span></span>|<span data-ttu-id="eddc2-213">Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde.
</span><span class="sxs-lookup"><span data-stu-id="eddc2-213">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="eddc2-214">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="eddc2-214">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="eddc2-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-215">Boolean</span></span>|<span data-ttu-id="eddc2-216">Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.</span><span class="sxs-lookup"><span data-stu-id="eddc2-216">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="eddc2-217">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="eddc2-217">appLockerApplicationControl</span></span>|[<span data-ttu-id="eddc2-218">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="eddc2-218">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="eddc2-219">Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps.</span><span class="sxs-lookup"><span data-stu-id="eddc2-219">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="eddc2-220">Mögliche Werte: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="eddc2-220">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="eddc2-221">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="eddc2-221">smartScreenEnableInShell</span></span>|<span data-ttu-id="eddc2-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-222">Boolean</span></span>|<span data-ttu-id="eddc2-223">Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.</span><span class="sxs-lookup"><span data-stu-id="eddc2-223">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="eddc2-224">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="eddc2-224">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="eddc2-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-225">Boolean</span></span>|<span data-ttu-id="eddc2-226">Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.</span><span class="sxs-lookup"><span data-stu-id="eddc2-226">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="eddc2-227">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="eddc2-227">applicationGuardEnabled</span></span>|<span data-ttu-id="eddc2-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-228">Boolean</span></span>|<span data-ttu-id="eddc2-229">Aktiviert Windows Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="eddc2-229">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="eddc2-230">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="eddc2-230">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="eddc2-231">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="eddc2-231">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="eddc2-232">Zwischenablage zum Übertragen der Bilddatei, Textdatei oder keiner dieser Dateien blockieren.</span><span class="sxs-lookup"><span data-stu-id="eddc2-232">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="eddc2-233">Mögliche Werte: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="eddc2-233">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="eddc2-234">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="eddc2-234">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="eddc2-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-235">Boolean</span></span>|<span data-ttu-id="eddc2-236">Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.</span><span class="sxs-lookup"><span data-stu-id="eddc2-236">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="eddc2-237">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="eddc2-237">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="eddc2-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-238">Boolean</span></span>|<span data-ttu-id="eddc2-239">Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).</span><span class="sxs-lookup"><span data-stu-id="eddc2-239">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="eddc2-240">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="eddc2-240">applicationGuardForceAuditing</span></span>|<span data-ttu-id="eddc2-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-241">Boolean</span></span>|<span data-ttu-id="eddc2-242">Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).</span><span class="sxs-lookup"><span data-stu-id="eddc2-242">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="eddc2-243">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="eddc2-243">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="eddc2-244">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="eddc2-244">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="eddc2-245">Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung.</span><span class="sxs-lookup"><span data-stu-id="eddc2-245">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="eddc2-246">Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="eddc2-246">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="eddc2-247">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="eddc2-247">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="eddc2-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-248">Boolean</span></span>|<span data-ttu-id="eddc2-249">Erlaubt das Drucken im PDF-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="eddc2-249">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="eddc2-250">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="eddc2-250">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="eddc2-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-251">Boolean</span></span>|<span data-ttu-id="eddc2-252">Erlaubt das Drucken im XPS-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="eddc2-252">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="eddc2-253">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="eddc2-253">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="eddc2-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-254">Boolean</span></span>|<span data-ttu-id="eddc2-255">Erlaubt das Drucken auf lokalen Druckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="eddc2-255">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="eddc2-256">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="eddc2-256">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="eddc2-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-257">Boolean</span></span>|<span data-ttu-id="eddc2-258">Erlaubt das Drucken auf Netzwerkdruckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="eddc2-258">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="eddc2-259">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="eddc2-259">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="eddc2-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-260">Boolean</span></span>|<span data-ttu-id="eddc2-261">Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="eddc2-261">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="eddc2-262">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="eddc2-262">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="eddc2-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-263">Boolean</span></span>|<span data-ttu-id="eddc2-264">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="eddc2-264">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="eddc2-265">Diese Richtlinie gilt nur für Mobilgeräte-SKUs.</span><span class="sxs-lookup"><span data-stu-id="eddc2-265">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="eddc2-266">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="eddc2-266">bitLockerEncryptDevice</span></span>|<span data-ttu-id="eddc2-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="eddc2-267">Boolean</span></span>|<span data-ttu-id="eddc2-268">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="eddc2-268">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="eddc2-269">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="eddc2-269">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="eddc2-270">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="eddc2-270">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="eddc2-271">BitLocker-Richtlinie für Wechseldatenträger</span><span class="sxs-lookup"><span data-stu-id="eddc2-271">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="eddc2-272">Antwort</span><span class="sxs-lookup"><span data-stu-id="eddc2-272">Response</span></span>
<span data-ttu-id="eddc2-273">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eddc2-273">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eddc2-274">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eddc2-274">Example</span></span>

### <a name="request"></a><span data-ttu-id="eddc2-275">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eddc2-275">Request</span></span>
<span data-ttu-id="eddc2-276">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eddc2-276">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4245

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a><span data-ttu-id="eddc2-277">Antwort</span><span class="sxs-lookup"><span data-stu-id="eddc2-277">Response</span></span>
<span data-ttu-id="eddc2-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eddc2-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4417

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```



