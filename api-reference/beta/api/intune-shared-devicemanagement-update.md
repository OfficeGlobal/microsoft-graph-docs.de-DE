---
title: Aktualisieren von „deviceManagement“
description: Aktualisieren der Eigenschaften eines deviceManagement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cd202c2a015b25234a7bf6ffdbedbd1b9f17eacd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846830"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="96023-103">Aktualisieren von „deviceManagement“</span><span class="sxs-lookup"><span data-stu-id="96023-103">Update deviceManagement</span></span>

> <span data-ttu-id="96023-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="96023-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96023-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="96023-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96023-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="96023-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96023-107">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="96023-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96023-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="96023-108">Prerequisites</span></span>

<span data-ttu-id="96023-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96023-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="96023-111">Beachten Sie, dass die Berechtigung abhängig vom Workflow variieren.</span><span class="sxs-lookup"><span data-stu-id="96023-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="96023-112">Berechtigung&nbsp;Typ&nbsp;(durch&nbsp;Workflow)</span><span class="sxs-lookup"><span data-stu-id="96023-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="96023-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96023-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="96023-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96023-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="96023-115">&nbsp;&nbsp; **Für die Arbeit android**</span><span class="sxs-lookup"><span data-stu-id="96023-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="96023-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="96023-117">&nbsp; &nbsp; **Überwachung**</span><span class="sxs-lookup"><span data-stu-id="96023-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="96023-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-119">&nbsp;&nbsp; **Unternehmen Begriffe**</span><span class="sxs-lookup"><span data-stu-id="96023-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="96023-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-121">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="96023-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="96023-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-123">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="96023-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="96023-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-125">&nbsp;&nbsp; **Elektronische SIM**</span><span class="sxs-lookup"><span data-stu-id="96023-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="96023-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-127">&nbsp; &nbsp; **Registrierung**</span><span class="sxs-lookup"><span data-stu-id="96023-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="96023-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-129">&nbsp;&nbsp; **Zauns**</span><span class="sxs-lookup"><span data-stu-id="96023-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="96023-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-131">&nbsp;&nbsp; **Benachrichtigung**</span><span class="sxs-lookup"><span data-stu-id="96023-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="96023-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-133">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="96023-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="96023-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-135">&nbsp;&nbsp; **Role-based Access Control (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="96023-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="96023-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-137">&nbsp;&nbsp; **Remotezugriff**</span><span class="sxs-lookup"><span data-stu-id="96023-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="96023-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96023-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="96023-139">&nbsp;&nbsp; **Remoteunterstützung**</span><span class="sxs-lookup"><span data-stu-id="96023-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="96023-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-141">&nbsp;&nbsp; **Telekommunikation Ausgaben Management**</span><span class="sxs-lookup"><span data-stu-id="96023-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="96023-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-143">&nbsp;&nbsp; **Erleichterung**</span><span class="sxs-lookup"><span data-stu-id="96023-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="96023-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-145">&nbsp;&nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="96023-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="96023-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96023-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="96023-147">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96023-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96023-148">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96023-148">Not supported.</span></span>|
| <span data-ttu-id="96023-149">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96023-149">Application</span></span> | <span data-ttu-id="96023-150">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96023-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96023-151">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96023-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="96023-152">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96023-152">Request headers</span></span>

|<span data-ttu-id="96023-153">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="96023-153">Header</span></span>|<span data-ttu-id="96023-154">Wert</span><span class="sxs-lookup"><span data-stu-id="96023-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96023-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="96023-155">Authorization</span></span>|<span data-ttu-id="96023-156">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="96023-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96023-157">Annehmen</span><span class="sxs-lookup"><span data-stu-id="96023-157">Accept</span></span>|<span data-ttu-id="96023-158">application/json</span><span class="sxs-lookup"><span data-stu-id="96023-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96023-159">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96023-159">Request body</span></span>

<span data-ttu-id="96023-160">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="96023-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="96023-161">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="96023-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="96023-162">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96023-162">Property</span></span>|<span data-ttu-id="96023-163">Typ</span><span class="sxs-lookup"><span data-stu-id="96023-163">Type</span></span>|<span data-ttu-id="96023-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96023-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96023-165">id</span><span class="sxs-lookup"><span data-stu-id="96023-165">id</span></span>|<span data-ttu-id="96023-166">String</span><span class="sxs-lookup"><span data-stu-id="96023-166">String</span></span>|<span data-ttu-id="96023-167">Eindeutiger Bezeichner für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="96023-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="96023-168">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="96023-168">**Device configuration**</span></span>|
|<span data-ttu-id="96023-169">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="96023-169">intuneAccountId</span></span>|<span data-ttu-id="96023-170">GUID</span><span class="sxs-lookup"><span data-stu-id="96023-170">GUID</span></span>|<span data-ttu-id="96023-171">Intune Konto-ID für die angegebenen Mandanten</span><span class="sxs-lookup"><span data-stu-id="96023-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="96023-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="96023-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="96023-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="96023-173">Boolean</span></span>|<span data-ttu-id="96023-174">Die Eigenschaft zum Aktivieren von nicht-MDM verwaltet legacy PC-Verwaltung für dieses Konto.</span><span class="sxs-lookup"><span data-stu-id="96023-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="96023-175">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="96023-175">This property is read-only.</span></span>|
|<span data-ttu-id="96023-176">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="96023-176">maximumDepTokens</span></span>|<span data-ttu-id="96023-177">Int32</span><span class="sxs-lookup"><span data-stu-id="96023-177">Int32</span></span>|<span data-ttu-id="96023-178">Maximal zulässige Anzahl von DEP Token pro Mandant.</span><span class="sxs-lookup"><span data-stu-id="96023-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="96023-179">settings</span><span class="sxs-lookup"><span data-stu-id="96023-179">settings</span></span>|[<span data-ttu-id="96023-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="96023-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="96023-181">Einstellungen auf Kontoebene</span><span class="sxs-lookup"><span data-stu-id="96023-181">Account level settings.</span></span>|
|<span data-ttu-id="96023-182">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="96023-182">**Device management**</span></span>|
|<span data-ttu-id="96023-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="96023-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="96023-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96023-184">DateTimeOffset</span></span>|<span data-ttu-id="96023-185">Datum & Zeit bei Mandantendaten zwischen Scaleunits verschoben.</span><span class="sxs-lookup"><span data-stu-id="96023-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="96023-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="96023-186">adminConsent</span></span>|[<span data-ttu-id="96023-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="96023-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="96023-188">Informationen zum Unternehmensadministrator Zustimmung.</span><span class="sxs-lookup"><span data-stu-id="96023-188">Admin consent information.</span></span>|
|<span data-ttu-id="96023-189">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="96023-189">deviceProtectionOverview</span></span>|[<span data-ttu-id="96023-190">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="96023-190">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="96023-191">Gerät Protection Overview.</span><span class="sxs-lookup"><span data-stu-id="96023-191">Device protection overview.</span></span>|
|<span data-ttu-id="96023-192">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="96023-192">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="96023-193">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="96023-193">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="96023-194">Cleanup-Regel</span><span class="sxs-lookup"><span data-stu-id="96023-194">Device cleanup rule</span></span>|
|<span data-ttu-id="96023-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="96023-195">subscriptionState</span></span>|[<span data-ttu-id="96023-196">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="96023-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="96023-197">Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="96023-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="96023-198">Mögliche Werte sind: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked` und `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="96023-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="96023-199">Abonnements</span><span class="sxs-lookup"><span data-stu-id="96023-199">subscriptions</span></span>|[<span data-ttu-id="96023-200">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="96023-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="96023-201">Mandanten-Abonnement.</span><span class="sxs-lookup"><span data-stu-id="96023-201">Tenant's Subscription.</span></span> <span data-ttu-id="96023-202">Mögliche Werte sind: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU` und `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="96023-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="96023-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="96023-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="96023-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="96023-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="96023-205">Übersicht über die Malware für Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="96023-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="96023-206">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="96023-206">**Onboarding**</span></span>|
|<span data-ttu-id="96023-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="96023-207">intuneBrand</span></span>|[<span data-ttu-id="96023-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="96023-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="96023-209">„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.</span><span class="sxs-lookup"><span data-stu-id="96023-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="96023-210">Anforderung Body-Eigenschaft Unterstützung variiert je nach Workflow.</span><span class="sxs-lookup"><span data-stu-id="96023-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="96023-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="96023-211">Response</span></span>
<span data-ttu-id="96023-212">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="96023-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96023-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96023-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="96023-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96023-214">Request</span></span>

<span data-ttu-id="96023-215">Es folgt ein Beispiel für eine Anforderung nach des Geräts-Workflows:</span><span class="sxs-lookup"><span data-stu-id="96023-215">Here is an example of a request following the device management workflow:</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a><span data-ttu-id="96023-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="96023-216">Response</span></span>

<span data-ttu-id="96023-217">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="96023-217">Here is an example of the response.</span></span> 

<span data-ttu-id="96023-218">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="96023-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="96023-219">Zurückgegebene Eigenschaften variieren je nach Workflow und Kontext.</span><span class="sxs-lookup"><span data-stu-id="96023-219">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```



