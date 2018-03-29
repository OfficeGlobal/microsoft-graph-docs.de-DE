# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="76311-101">Erstellen von „windows10EndpointProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="76311-101">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="76311-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="76311-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76311-103">Diese Methode erstellt ein neues Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76311-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="76311-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="76311-104">Prerequisites</span></span>
<span data-ttu-id="76311-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="76311-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="76311-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="76311-107">Permission type</span></span>|<span data-ttu-id="76311-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="76311-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76311-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="76311-109">Delegated (work or school account)</span></span>|<span data-ttu-id="76311-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76311-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76311-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="76311-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76311-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76311-112">Not supported.</span></span>|
|<span data-ttu-id="76311-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="76311-113">Application</span></span>|<span data-ttu-id="76311-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76311-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76311-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="76311-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="76311-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="76311-116">Request headers</span></span>
|<span data-ttu-id="76311-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="76311-117">Header</span></span>|<span data-ttu-id="76311-118">Wert</span><span class="sxs-lookup"><span data-stu-id="76311-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76311-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="76311-119">Authorization</span></span>|<span data-ttu-id="76311-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="76311-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="76311-121">Accept</span><span class="sxs-lookup"><span data-stu-id="76311-121">Accept</span></span>|<span data-ttu-id="76311-122">application/json</span><span class="sxs-lookup"><span data-stu-id="76311-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76311-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="76311-123">Request body</span></span>
<span data-ttu-id="76311-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10EndpointProtectionConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="76311-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="76311-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10EndpointProtectionConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="76311-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="76311-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="76311-126">Property</span></span>|<span data-ttu-id="76311-127">Typ</span><span class="sxs-lookup"><span data-stu-id="76311-127">Type</span></span>|<span data-ttu-id="76311-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76311-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76311-129">id</span><span class="sxs-lookup"><span data-stu-id="76311-129">id</span></span>|<span data-ttu-id="76311-130">String</span><span class="sxs-lookup"><span data-stu-id="76311-130">String</span></span>|<span data-ttu-id="76311-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="76311-131">Key of the setting.</span></span> <span data-ttu-id="76311-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76311-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76311-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76311-133">lastModifiedDateTime</span></span>|<span data-ttu-id="76311-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76311-134">DateTimeOffset</span></span>|<span data-ttu-id="76311-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="76311-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="76311-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76311-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76311-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76311-137">createdDateTime</span></span>|<span data-ttu-id="76311-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76311-138">DateTimeOffset</span></span>|<span data-ttu-id="76311-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="76311-139">DateTime the object was created.</span></span> <span data-ttu-id="76311-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76311-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76311-141">description</span><span class="sxs-lookup"><span data-stu-id="76311-141">description</span></span>|<span data-ttu-id="76311-142">String</span><span class="sxs-lookup"><span data-stu-id="76311-142">String</span></span>|<span data-ttu-id="76311-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="76311-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="76311-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76311-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76311-145">displayName</span><span class="sxs-lookup"><span data-stu-id="76311-145">displayName</span></span>|<span data-ttu-id="76311-146">String</span><span class="sxs-lookup"><span data-stu-id="76311-146">String</span></span>|<span data-ttu-id="76311-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="76311-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="76311-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76311-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76311-149">version</span><span class="sxs-lookup"><span data-stu-id="76311-149">version</span></span>|<span data-ttu-id="76311-150">Int32</span><span class="sxs-lookup"><span data-stu-id="76311-150">Int32</span></span>|<span data-ttu-id="76311-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="76311-151">Version of the device configuration.</span></span> <span data-ttu-id="76311-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76311-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76311-153">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="76311-153">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="76311-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-154">Boolean</span></span>|<span data-ttu-id="76311-155">Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="76311-155">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="76311-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="76311-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="76311-157">Int32</span><span class="sxs-lookup"><span data-stu-id="76311-157">Int32</span></span>|<span data-ttu-id="76311-158">Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600.</span><span class="sxs-lookup"><span data-stu-id="76311-158">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="76311-159">Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="76311-159">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="76311-160">Gültige Werte: 300 bis 3600.</span><span class="sxs-lookup"><span data-stu-id="76311-160">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="76311-161">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="76311-161">firewallPreSharedKeyEncodingMethod</span></span>|<span data-ttu-id="76311-162">String</span><span class="sxs-lookup"><span data-stu-id="76311-162">String</span></span>|<span data-ttu-id="76311-163">Diese Eigenschaft legt die Codierung des vorinstallierten Schlüssels fest. Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.</span><span class="sxs-lookup"><span data-stu-id="76311-163">Select the preshared key encoding to be used Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="76311-164">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="76311-164">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="76311-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-165">Boolean</span></span>|<span data-ttu-id="76311-166">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="76311-166">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="76311-167">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="76311-167">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="76311-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-168">Boolean</span></span>|<span data-ttu-id="76311-169">Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="76311-169">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="76311-170">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="76311-170">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="76311-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-171">Boolean</span></span>|<span data-ttu-id="76311-172">Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="76311-172">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="76311-173">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="76311-173">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="76311-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-174">Boolean</span></span>|<span data-ttu-id="76311-175">Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="76311-175">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="76311-176">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="76311-176">firewallCertificateRevocationListCheckMethod</span></span>|<span data-ttu-id="76311-177">String</span><span class="sxs-lookup"><span data-stu-id="76311-177">String</span></span>|<span data-ttu-id="76311-178">Gibt an, wie die Zertifikatssperrliste erzwungen werden soll. Mögliche Werte sind: `deviceDefault`, `none`, `attempt` und `require`.</span><span class="sxs-lookup"><span data-stu-id="76311-178">Specify how the certificate revocation list is to be enforced Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="76311-179">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="76311-179">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="76311-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-180">Boolean</span></span>|<span data-ttu-id="76311-181">Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.</span><span class="sxs-lookup"><span data-stu-id="76311-181">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="76311-182">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="76311-182">firewallPacketQueueingMethod</span></span>|<span data-ttu-id="76311-183">String</span><span class="sxs-lookup"><span data-stu-id="76311-183">String</span></span>|<span data-ttu-id="76311-184">Konfiguriert, wie Paketwarteschlangen im Tunnelgatewayszenario implementiert werden sollen. Mögliche Werte sind: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound` und `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="76311-184">Configures how packet queueing should be applied in the tunnel gateway scenario Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="76311-185">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="76311-185">firewallProfileDomain</span></span>|[<span data-ttu-id="76311-186">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="76311-186">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="76311-187">Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.</span><span class="sxs-lookup"><span data-stu-id="76311-187">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="76311-188">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="76311-188">firewallProfilePublic</span></span>|[<span data-ttu-id="76311-189">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="76311-189">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="76311-190">Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="76311-190">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="76311-191">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="76311-191">firewallProfilePrivate</span></span>|[<span data-ttu-id="76311-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="76311-192">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="76311-193">Konfiguriert die Firewallprofileinstellungen für private Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="76311-193">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="76311-194">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="76311-194">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="76311-195">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="76311-195">String collection</span></span>|<span data-ttu-id="76311-196">Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen</span><span class="sxs-lookup"><span data-stu-id="76311-196">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="76311-197">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="76311-197">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="76311-198">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="76311-198">String collection</span></span>|<span data-ttu-id="76311-199">Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen</span><span class="sxs-lookup"><span data-stu-id="76311-199">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="76311-200">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="76311-200">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="76311-201">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="76311-201">String collection</span></span>|<span data-ttu-id="76311-202">Liste von Ordnerpfaden, die der Liste der geschützter Ordner hinzugefügt werden sollen</span><span class="sxs-lookup"><span data-stu-id="76311-202">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="76311-203">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="76311-203">defenderExploitProtectionXml</span></span>|<span data-ttu-id="76311-204">Binary</span><span class="sxs-lookup"><span data-stu-id="76311-204">Binary</span></span>|<span data-ttu-id="76311-205">XML-Inhalte mit Details zum Exploit-Schutz</span><span class="sxs-lookup"><span data-stu-id="76311-205">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="76311-206">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="76311-206">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="76311-207">String</span><span class="sxs-lookup"><span data-stu-id="76311-207">String</span></span>|<span data-ttu-id="76311-208">Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde</span><span class="sxs-lookup"><span data-stu-id="76311-208">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="76311-209">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="76311-209">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="76311-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-210">Boolean</span></span>|<span data-ttu-id="76311-211">Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.</span><span class="sxs-lookup"><span data-stu-id="76311-211">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="76311-212">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="76311-212">appLockerApplicationControl</span></span>|<span data-ttu-id="76311-213">String</span><span class="sxs-lookup"><span data-stu-id="76311-213">String</span></span>|<span data-ttu-id="76311-214">Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps.</span><span class="sxs-lookup"><span data-stu-id="76311-214">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="76311-215">Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker` und `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="76311-215">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="76311-216">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="76311-216">smartScreenEnableInShell</span></span>|<span data-ttu-id="76311-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-217">Boolean</span></span>|<span data-ttu-id="76311-218">Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.</span><span class="sxs-lookup"><span data-stu-id="76311-218">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="76311-219">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="76311-219">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="76311-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-220">Boolean</span></span>|<span data-ttu-id="76311-221">Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.</span><span class="sxs-lookup"><span data-stu-id="76311-221">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="76311-222">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="76311-222">applicationGuardEnabled</span></span>|<span data-ttu-id="76311-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-223">Boolean</span></span>|<span data-ttu-id="76311-224">Aktiviert Windows Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="76311-224">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="76311-225">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="76311-225">applicationGuardBlockFileTransfer</span></span>|<span data-ttu-id="76311-226">String</span><span class="sxs-lookup"><span data-stu-id="76311-226">String</span></span>|<span data-ttu-id="76311-227">Blockiert die Übertragung von Bilddateien oder Textdateien oder beiden Dateitypen durch die Zwischenablage. Mögliche Werte sind: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone` und `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="76311-227">Block clipboard to transfer image file, text file or neither of them Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="76311-228">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="76311-228">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="76311-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-229">Boolean</span></span>|<span data-ttu-id="76311-230">Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.</span><span class="sxs-lookup"><span data-stu-id="76311-230">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="76311-231">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="76311-231">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="76311-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-232">Boolean</span></span>|<span data-ttu-id="76311-233">Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).</span><span class="sxs-lookup"><span data-stu-id="76311-233">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="76311-234">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="76311-234">applicationGuardForceAuditing</span></span>|<span data-ttu-id="76311-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-235">Boolean</span></span>|<span data-ttu-id="76311-236">Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).</span><span class="sxs-lookup"><span data-stu-id="76311-236">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="76311-237">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="76311-237">applicationGuardBlockClipboardSharing</span></span>|<span data-ttu-id="76311-238">String</span><span class="sxs-lookup"><span data-stu-id="76311-238">String</span></span>|<span data-ttu-id="76311-239">Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung.</span><span class="sxs-lookup"><span data-stu-id="76311-239">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="76311-240">Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="76311-240">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="76311-241">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="76311-241">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="76311-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-242">Boolean</span></span>|<span data-ttu-id="76311-243">Erlaubt das Drucken im PDF-Format über Container.</span><span class="sxs-lookup"><span data-stu-id="76311-243">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="76311-244">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="76311-244">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="76311-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-245">Boolean</span></span>|<span data-ttu-id="76311-246">Erlaubt das Drucken im XPS-Format über Container.</span><span class="sxs-lookup"><span data-stu-id="76311-246">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="76311-247">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="76311-247">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="76311-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-248">Boolean</span></span>|<span data-ttu-id="76311-249">Erlaubt das Drucken mit lokalen Druckern über Container.</span><span class="sxs-lookup"><span data-stu-id="76311-249">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="76311-250">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="76311-250">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="76311-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-251">Boolean</span></span>|<span data-ttu-id="76311-252">Erlaubt das Drucken mit Netzwerkdruckern über Container.</span><span class="sxs-lookup"><span data-stu-id="76311-252">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="76311-253">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="76311-253">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="76311-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-254">Boolean</span></span>|<span data-ttu-id="76311-255">Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="76311-255">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="76311-256">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="76311-256">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="76311-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-257">Boolean</span></span>|<span data-ttu-id="76311-258">Ermöglicht, dass der Administrator die Aktivierung der Verschlüsselung mittels BitLocker fordert.</span><span class="sxs-lookup"><span data-stu-id="76311-258">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="76311-259">Diese Richtlinie gilt nur für Mobilgeräte-SKUs.</span><span class="sxs-lookup"><span data-stu-id="76311-259">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="76311-260">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="76311-260">bitLockerEncryptDevice</span></span>|<span data-ttu-id="76311-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="76311-261">Boolean</span></span>|<span data-ttu-id="76311-262">Ermöglicht, dass der Administrator die Aktivierung der Verschlüsselung mittels BitLocker fordert.</span><span class="sxs-lookup"><span data-stu-id="76311-262">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="76311-263">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="76311-263">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="76311-264">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="76311-264">bitLockerRemovableDrivePolicy</span></span>](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|<span data-ttu-id="76311-265">BitLocker-Richtlinie für Wechseldatenträger</span><span class="sxs-lookup"><span data-stu-id="76311-265">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="76311-266">Antwort</span><span class="sxs-lookup"><span data-stu-id="76311-266">Response</span></span>
<span data-ttu-id="76311-267">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="76311-267">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76311-268">Beispiel</span><span class="sxs-lookup"><span data-stu-id="76311-268">Example</span></span>
### <a name="request"></a><span data-ttu-id="76311-269">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76311-269">Request</span></span>
<span data-ttu-id="76311-270">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76311-270">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4309

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="76311-271">Antwort</span><span class="sxs-lookup"><span data-stu-id="76311-271">Response</span></span>
<span data-ttu-id="76311-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76311-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



