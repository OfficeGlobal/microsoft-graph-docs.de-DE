# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="f981a-101">Aktualisieren von „windows10EndpointProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="f981a-101">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="f981a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f981a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f981a-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f981a-103">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f981a-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f981a-104">Prerequisites</span></span>
<span data-ttu-id="f981a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f981a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f981a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f981a-107">Permission type</span></span>|<span data-ttu-id="f981a-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f981a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f981a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f981a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f981a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f981a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f981a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f981a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f981a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f981a-112">Not supported.</span></span>|
|<span data-ttu-id="f981a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f981a-113">Application</span></span>|<span data-ttu-id="f981a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f981a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f981a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f981a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f981a-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f981a-116">Request headers</span></span>
|<span data-ttu-id="f981a-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f981a-117">Header</span></span>|<span data-ttu-id="f981a-118">Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f981a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f981a-119">Authorization</span></span>|<span data-ttu-id="f981a-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f981a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f981a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f981a-121">Accept</span></span>|<span data-ttu-id="f981a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f981a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f981a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f981a-123">Request body</span></span>
<span data-ttu-id="f981a-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="f981a-124">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="f981a-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f981a-125">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="f981a-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f981a-126">Property</span></span>|<span data-ttu-id="f981a-127">Typ</span><span class="sxs-lookup"><span data-stu-id="f981a-127">Type</span></span>|<span data-ttu-id="f981a-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f981a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f981a-129">id</span><span class="sxs-lookup"><span data-stu-id="f981a-129">id</span></span>|<span data-ttu-id="f981a-130">String</span><span class="sxs-lookup"><span data-stu-id="f981a-130">String</span></span>|<span data-ttu-id="f981a-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="f981a-131">Key of the entity.</span></span> <span data-ttu-id="f981a-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f981a-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f981a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f981a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f981a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f981a-134">DateTimeOffset</span></span>|<span data-ttu-id="f981a-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f981a-135">DateTime the object was last modified.</span></span> <span data-ttu-id="f981a-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f981a-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f981a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f981a-137">createdDateTime</span></span>|<span data-ttu-id="f981a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f981a-138">DateTimeOffset</span></span>|<span data-ttu-id="f981a-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f981a-139">DateTime the object was created.</span></span> <span data-ttu-id="f981a-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f981a-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f981a-141">description</span><span class="sxs-lookup"><span data-stu-id="f981a-141">description</span></span>|<span data-ttu-id="f981a-142">String</span><span class="sxs-lookup"><span data-stu-id="f981a-142">String</span></span>|<span data-ttu-id="f981a-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f981a-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f981a-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f981a-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f981a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f981a-145">displayName</span></span>|<span data-ttu-id="f981a-146">String</span><span class="sxs-lookup"><span data-stu-id="f981a-146">String</span></span>|<span data-ttu-id="f981a-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f981a-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f981a-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f981a-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f981a-149">version</span><span class="sxs-lookup"><span data-stu-id="f981a-149">version</span></span>|<span data-ttu-id="f981a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f981a-150">Int32</span></span>|<span data-ttu-id="f981a-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f981a-151">Version of the device configuration.</span></span> <span data-ttu-id="f981a-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f981a-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f981a-153">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="f981a-153">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="f981a-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="f981a-154">Boolean</span></span>|<span data-ttu-id="f981a-155">Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="f981a-155">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="f981a-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="f981a-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="f981a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f981a-157">Int32</span></span>|<span data-ttu-id="f981a-158">Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600.</span><span class="sxs-lookup"><span data-stu-id="f981a-158">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="f981a-159">Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="f981a-159">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="f981a-160">Gültige Werte: 300 bis 3600.</span><span class="sxs-lookup"><span data-stu-id="f981a-160">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="f981a-161">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="f981a-161">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="f981a-162">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="f981a-162">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune_deviceconfig_firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="f981a-163">Wählen Sie den vorinstallierten Schlüssel um zu verwendende Codierung.</span><span class="sxs-lookup"><span data-stu-id="f981a-163">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="f981a-164">Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.</span><span class="sxs-lookup"><span data-stu-id="f981a-164">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="f981a-165">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="f981a-165">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="f981a-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-166">Boolean</span></span>|<span data-ttu-id="f981a-167">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="f981a-167">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="f981a-168">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="f981a-168">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="f981a-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-169">Boolean</span></span>|<span data-ttu-id="f981a-170">Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="f981a-170">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="f981a-171">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="f981a-171">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="f981a-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-172">Boolean</span></span>|<span data-ttu-id="f981a-173">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="f981a-173">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="f981a-174">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="f981a-174">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="f981a-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-175">Boolean</span></span>|<span data-ttu-id="f981a-176">Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="f981a-176">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="f981a-177">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="f981a-177">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="f981a-178">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="f981a-178">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune_deviceconfig_firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="f981a-179">Geben Sie an, wie die Certificate Revocation List erzwungen werden.</span><span class="sxs-lookup"><span data-stu-id="f981a-179">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="f981a-180">Mögliche Werte: sind `deviceDefault`, `none`, `attempt` und `require`.</span><span class="sxs-lookup"><span data-stu-id="f981a-180">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="f981a-181">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="f981a-181">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="f981a-182">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-182">Boolean</span></span>|<span data-ttu-id="f981a-183">Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.</span><span class="sxs-lookup"><span data-stu-id="f981a-183">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="f981a-184">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="f981a-184">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="f981a-185">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="f981a-185">firewallPacketQueueingMethodType</span></span>](../resources/intune_deviceconfig_firewallpacketqueueingmethodtype.md)|<span data-ttu-id="f981a-186">Konfiguriert, wie vom Warteschlangensystem Paket im Szenario mit Tunnel Gateway angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f981a-186">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="f981a-187">Mögliche Werte sind: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound` und `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="f981a-187">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="f981a-188">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="f981a-188">firewallProfileDomain</span></span>|[<span data-ttu-id="f981a-189">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f981a-189">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="f981a-190">Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.</span><span class="sxs-lookup"><span data-stu-id="f981a-190">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="f981a-191">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="f981a-191">firewallProfilePublic</span></span>|[<span data-ttu-id="f981a-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f981a-192">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="f981a-193">Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="f981a-193">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="f981a-194">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="f981a-194">firewallProfilePrivate</span></span>|[<span data-ttu-id="f981a-195">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f981a-195">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="f981a-196">Konfiguriert die Firewallprofileinstellungen für private Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="f981a-196">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="f981a-197">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="f981a-197">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="f981a-198">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f981a-198">String collection</span></span>|<span data-ttu-id="f981a-199">Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="f981a-199">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="f981a-200">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="f981a-200">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="f981a-201">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f981a-201">String collection</span></span>|<span data-ttu-id="f981a-202">Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen.
</span><span class="sxs-lookup"><span data-stu-id="f981a-202">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="f981a-203">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="f981a-203">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="f981a-204">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f981a-204">String collection</span></span>|<span data-ttu-id="f981a-205">Liste von Ordnerpfaden, die der Liste geschützter Ordner hinzugefügt werden sollen.
</span><span class="sxs-lookup"><span data-stu-id="f981a-205">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="f981a-206">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="f981a-206">defenderExploitProtectionXml</span></span>|<span data-ttu-id="f981a-207">Binär</span><span class="sxs-lookup"><span data-stu-id="f981a-207">Binary</span></span>|<span data-ttu-id="f981a-208">XML-Inhalte mit Details zum Exploit-Schutz.
</span><span class="sxs-lookup"><span data-stu-id="f981a-208">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="f981a-209">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="f981a-209">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="f981a-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f981a-210">String</span></span>|<span data-ttu-id="f981a-211">Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde.
</span><span class="sxs-lookup"><span data-stu-id="f981a-211">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="f981a-212">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="f981a-212">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="f981a-213">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-213">Boolean</span></span>|<span data-ttu-id="f981a-214">Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.</span><span class="sxs-lookup"><span data-stu-id="f981a-214">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="f981a-215">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="f981a-215">appLockerApplicationControl</span></span>|[<span data-ttu-id="f981a-216">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="f981a-216">appLockerApplicationControlType</span></span>](../resources/intune_deviceconfig_applockerapplicationcontroltype.md)|<span data-ttu-id="f981a-217">Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps.</span><span class="sxs-lookup"><span data-stu-id="f981a-217">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="f981a-218">Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker` und `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="f981a-218">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="f981a-219">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="f981a-219">smartScreenEnableInShell</span></span>|<span data-ttu-id="f981a-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-220">Boolean</span></span>|<span data-ttu-id="f981a-221">Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.</span><span class="sxs-lookup"><span data-stu-id="f981a-221">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="f981a-222">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="f981a-222">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="f981a-223">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-223">Boolean</span></span>|<span data-ttu-id="f981a-224">Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.</span><span class="sxs-lookup"><span data-stu-id="f981a-224">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="f981a-225">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="f981a-225">applicationGuardEnabled</span></span>|<span data-ttu-id="f981a-226">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-226">Boolean</span></span>|<span data-ttu-id="f981a-227">Aktiviert Windows Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="f981a-227">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="f981a-228">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="f981a-228">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="f981a-229">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="f981a-229">applicationGuardBlockFileTransferType</span></span>](../resources/intune_deviceconfig_applicationguardblockfiletransfertype.md)|<span data-ttu-id="f981a-230">Block Zwischenablage Übertragung Bilddatei, Textdatei oder dürfen.</span><span class="sxs-lookup"><span data-stu-id="f981a-230">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="f981a-231">Mögliche Werte sind: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone` und `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="f981a-231">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="f981a-232">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="f981a-232">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="f981a-233">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-233">Boolean</span></span>|<span data-ttu-id="f981a-234">Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.</span><span class="sxs-lookup"><span data-stu-id="f981a-234">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="f981a-235">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="f981a-235">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="f981a-236">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-236">Boolean</span></span>|<span data-ttu-id="f981a-237">Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).</span><span class="sxs-lookup"><span data-stu-id="f981a-237">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="f981a-238">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="f981a-238">applicationGuardForceAuditing</span></span>|<span data-ttu-id="f981a-239">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-239">Boolean</span></span>|<span data-ttu-id="f981a-240">Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).</span><span class="sxs-lookup"><span data-stu-id="f981a-240">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="f981a-241">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="f981a-241">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="f981a-242">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="f981a-242">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune_deviceconfig_applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="f981a-243">Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung.</span><span class="sxs-lookup"><span data-stu-id="f981a-243">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="f981a-244">Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="f981a-244">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="f981a-245">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="f981a-245">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="f981a-246">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-246">Boolean</span></span>|<span data-ttu-id="f981a-247">Erlaubt das Drucken im PDF-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="f981a-247">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="f981a-248">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="f981a-248">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="f981a-249">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-249">Boolean</span></span>|<span data-ttu-id="f981a-250">Erlaubt das Drucken im XPS-Format aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="f981a-250">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="f981a-251">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="f981a-251">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="f981a-252">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-252">Boolean</span></span>|<span data-ttu-id="f981a-253">Erlaubt das Drucken auf lokalen Druckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="f981a-253">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="f981a-254">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="f981a-254">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="f981a-255">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-255">Boolean</span></span>|<span data-ttu-id="f981a-256">Erlaubt das Drucken auf Netzwerkdruckern aus dem Container.
</span><span class="sxs-lookup"><span data-stu-id="f981a-256">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="f981a-257">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="f981a-257">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="f981a-258">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-258">Boolean</span></span>|<span data-ttu-id="f981a-259">Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="f981a-259">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="f981a-260">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="f981a-260">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="f981a-261">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-261">Boolean</span></span>|<span data-ttu-id="f981a-262">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="f981a-262">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="f981a-263">Diese Richtlinie gilt nur für Mobilgeräte-SKUs.</span><span class="sxs-lookup"><span data-stu-id="f981a-263">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="f981a-264">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="f981a-264">bitLockerEncryptDevice</span></span>|<span data-ttu-id="f981a-265">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f981a-265">Boolean</span></span>|<span data-ttu-id="f981a-266">Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.
</span><span class="sxs-lookup"><span data-stu-id="f981a-266">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="f981a-267">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f981a-267">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="f981a-268">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f981a-268">bitLockerRemovableDrivePolicy</span></span>](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|<span data-ttu-id="f981a-269">BitLocker-Richtlinie für Wechseldatenträger</span><span class="sxs-lookup"><span data-stu-id="f981a-269">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="f981a-270">Antwort</span><span class="sxs-lookup"><span data-stu-id="f981a-270">Response</span></span>
<span data-ttu-id="f981a-271">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f981a-271">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f981a-272">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f981a-272">Example</span></span>
### <a name="request"></a><span data-ttu-id="f981a-273">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f981a-273">Request</span></span>
<span data-ttu-id="f981a-274">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f981a-274">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f981a-275">Antwort</span><span class="sxs-lookup"><span data-stu-id="f981a-275">Response</span></span>
<span data-ttu-id="f981a-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f981a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



