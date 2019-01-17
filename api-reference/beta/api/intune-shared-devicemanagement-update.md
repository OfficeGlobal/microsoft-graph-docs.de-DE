---
title: Aktualisieren von „deviceManagement“
description: Aktualisieren der Eigenschaften eines deviceManagement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d8465ee45a2a6c23dedc4fe049ef1f73bb25218
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924692"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="88a16-103">Aktualisieren von „deviceManagement“</span><span class="sxs-lookup"><span data-stu-id="88a16-103">Update deviceManagement</span></span>

> <span data-ttu-id="88a16-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="88a16-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88a16-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="88a16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88a16-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="88a16-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88a16-107">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="88a16-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88a16-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="88a16-108">Prerequisites</span></span>

<span data-ttu-id="88a16-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88a16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="88a16-111">Beachten Sie, dass die Berechtigung abhängig vom Workflow variieren.</span><span class="sxs-lookup"><span data-stu-id="88a16-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="88a16-112">Berechtigung&nbsp;Typ&nbsp;(durch&nbsp;Workflow)</span><span class="sxs-lookup"><span data-stu-id="88a16-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="88a16-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="88a16-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="88a16-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="88a16-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="88a16-115">&nbsp;&nbsp; **Für die Arbeit android**</span><span class="sxs-lookup"><span data-stu-id="88a16-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="88a16-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="88a16-117">&nbsp; &nbsp; **Überwachung**</span><span class="sxs-lookup"><span data-stu-id="88a16-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="88a16-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-119">&nbsp;&nbsp; **Unternehmen Begriffe**</span><span class="sxs-lookup"><span data-stu-id="88a16-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="88a16-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-121">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="88a16-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="88a16-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-123">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="88a16-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="88a16-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-125">&nbsp;&nbsp; **Elektronische SIM**</span><span class="sxs-lookup"><span data-stu-id="88a16-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="88a16-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-127">&nbsp; &nbsp; **Registrierung**</span><span class="sxs-lookup"><span data-stu-id="88a16-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="88a16-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-129">&nbsp;&nbsp; **Zauns**</span><span class="sxs-lookup"><span data-stu-id="88a16-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="88a16-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-131">&nbsp;&nbsp; **Benachrichtigung**</span><span class="sxs-lookup"><span data-stu-id="88a16-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="88a16-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-133">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="88a16-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="88a16-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-135">&nbsp;&nbsp; **Role-based Access Control (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="88a16-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="88a16-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-137">&nbsp;&nbsp; **Remotezugriff**</span><span class="sxs-lookup"><span data-stu-id="88a16-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="88a16-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88a16-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88a16-139">&nbsp;&nbsp; **Remoteunterstützung**</span><span class="sxs-lookup"><span data-stu-id="88a16-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="88a16-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-141">&nbsp;&nbsp; **Telekommunikation Ausgaben Management**</span><span class="sxs-lookup"><span data-stu-id="88a16-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="88a16-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-143">&nbsp;&nbsp; **Erleichterung**</span><span class="sxs-lookup"><span data-stu-id="88a16-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="88a16-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-145">&nbsp;&nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="88a16-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="88a16-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a16-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="88a16-147">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="88a16-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88a16-148">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88a16-148">Not supported.</span></span>|
| <span data-ttu-id="88a16-149">Anwendung</span><span class="sxs-lookup"><span data-stu-id="88a16-149">Application</span></span> | <span data-ttu-id="88a16-150">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88a16-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88a16-151">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="88a16-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="88a16-152">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="88a16-152">Request headers</span></span>

|<span data-ttu-id="88a16-153">Header</span><span class="sxs-lookup"><span data-stu-id="88a16-153">Header</span></span>|<span data-ttu-id="88a16-154">Wert</span><span class="sxs-lookup"><span data-stu-id="88a16-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88a16-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="88a16-155">Authorization</span></span>|<span data-ttu-id="88a16-156">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="88a16-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88a16-157">Annehmen</span><span class="sxs-lookup"><span data-stu-id="88a16-157">Accept</span></span>|<span data-ttu-id="88a16-158">application/json</span><span class="sxs-lookup"><span data-stu-id="88a16-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88a16-159">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="88a16-159">Request body</span></span>

<span data-ttu-id="88a16-160">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="88a16-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="88a16-161">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="88a16-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="88a16-162">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88a16-162">Property</span></span>|<span data-ttu-id="88a16-163">Typ</span><span class="sxs-lookup"><span data-stu-id="88a16-163">Type</span></span>|<span data-ttu-id="88a16-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88a16-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88a16-165">id</span><span class="sxs-lookup"><span data-stu-id="88a16-165">id</span></span>|<span data-ttu-id="88a16-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88a16-166">String</span></span>|<span data-ttu-id="88a16-167">Eindeutiger Bezeichner für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="88a16-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="88a16-168">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="88a16-168">**Device configuration**</span></span>|
|<span data-ttu-id="88a16-169">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="88a16-169">intuneAccountId</span></span>|<span data-ttu-id="88a16-170">GUID</span><span class="sxs-lookup"><span data-stu-id="88a16-170">GUID</span></span>|<span data-ttu-id="88a16-171">Intune Konto-ID für die angegebenen Mandanten</span><span class="sxs-lookup"><span data-stu-id="88a16-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="88a16-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="88a16-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="88a16-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="88a16-173">Boolean</span></span>|<span data-ttu-id="88a16-174">Die Eigenschaft zum Aktivieren von nicht-MDM verwaltet legacy PC-Verwaltung für dieses Konto.</span><span class="sxs-lookup"><span data-stu-id="88a16-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="88a16-175">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="88a16-175">This property is read-only.</span></span>|
|<span data-ttu-id="88a16-176">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="88a16-176">maximumDepTokens</span></span>|<span data-ttu-id="88a16-177">Int32</span><span class="sxs-lookup"><span data-stu-id="88a16-177">Int32</span></span>|<span data-ttu-id="88a16-178">Maximal zulässige Anzahl von DEP Token pro Mandant.</span><span class="sxs-lookup"><span data-stu-id="88a16-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="88a16-179">settings</span><span class="sxs-lookup"><span data-stu-id="88a16-179">settings</span></span>|[<span data-ttu-id="88a16-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="88a16-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="88a16-181">Einstellungen auf Kontoebene</span><span class="sxs-lookup"><span data-stu-id="88a16-181">Account level settings.</span></span>|
|<span data-ttu-id="88a16-182">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="88a16-182">**Device management**</span></span>|
|<span data-ttu-id="88a16-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="88a16-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="88a16-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88a16-184">DateTimeOffset</span></span>|<span data-ttu-id="88a16-185">Das Datum & Uhrzeit wann Mandantendaten zwischen Scaleunits verschoben.</span><span class="sxs-lookup"><span data-stu-id="88a16-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="88a16-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="88a16-186">adminConsent</span></span>|[<span data-ttu-id="88a16-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="88a16-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="88a16-188">Informationen zum Unternehmensadministrator Zustimmung.</span><span class="sxs-lookup"><span data-stu-id="88a16-188">Admin consent information.</span></span>|
|<span data-ttu-id="88a16-189">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="88a16-189">deviceProtectionOverview</span></span>|[<span data-ttu-id="88a16-190">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="88a16-190">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="88a16-191">Gerät Protection Overview.</span><span class="sxs-lookup"><span data-stu-id="88a16-191">Device protection overview.</span></span>|
|<span data-ttu-id="88a16-192">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="88a16-192">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="88a16-193">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="88a16-193">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="88a16-194">Cleanup-Regel</span><span class="sxs-lookup"><span data-stu-id="88a16-194">Device cleanup rule</span></span>|
|<span data-ttu-id="88a16-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="88a16-195">subscriptionState</span></span>|[<span data-ttu-id="88a16-196">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="88a16-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="88a16-197">Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="88a16-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="88a16-198">Mögliche Werte sind: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked` und `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="88a16-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="88a16-199">Abonnements</span><span class="sxs-lookup"><span data-stu-id="88a16-199">subscriptions</span></span>|[<span data-ttu-id="88a16-200">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="88a16-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="88a16-201">Mandanten-Abonnement.</span><span class="sxs-lookup"><span data-stu-id="88a16-201">Tenant's Subscription.</span></span> <span data-ttu-id="88a16-202">Mögliche Werte sind: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU` und `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="88a16-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="88a16-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="88a16-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="88a16-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="88a16-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="88a16-205">Übersicht über die Malware für Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="88a16-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="88a16-206">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="88a16-206">**Onboarding**</span></span>|
|<span data-ttu-id="88a16-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="88a16-207">intuneBrand</span></span>|[<span data-ttu-id="88a16-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="88a16-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="88a16-209">„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.</span><span class="sxs-lookup"><span data-stu-id="88a16-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="88a16-210">Anforderung Body-Eigenschaft Unterstützung variiert je nach Workflow.</span><span class="sxs-lookup"><span data-stu-id="88a16-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="88a16-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="88a16-211">Response</span></span>
<span data-ttu-id="88a16-212">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="88a16-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88a16-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="88a16-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="88a16-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="88a16-214">Request</span></span>

<span data-ttu-id="88a16-215">Es folgt ein Beispiel für eine Anforderung nach des Geräts-Workflows:</span><span class="sxs-lookup"><span data-stu-id="88a16-215">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="88a16-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="88a16-216">Response</span></span>

<span data-ttu-id="88a16-217">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="88a16-217">Here is an example of the response.</span></span> 

<span data-ttu-id="88a16-218">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="88a16-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="88a16-219">Zurückgegebene Eigenschaften variieren je nach Workflow und Kontext.</span><span class="sxs-lookup"><span data-stu-id="88a16-219">Returned properties vary according to workflow and context.</span></span>

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



