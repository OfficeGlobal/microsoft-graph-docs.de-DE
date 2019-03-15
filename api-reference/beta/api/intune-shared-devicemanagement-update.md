---
title: deviceManagement aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a71212652d789b08a8cb496b6b98c18b12d3e9c7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571053"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="bc7b3-103">deviceManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bc7b3-103">Update deviceManagement</span></span>

> <span data-ttu-id="bc7b3-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc7b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc7b3-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc7b3-107">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc7b3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bc7b3-108">Prerequisites</span></span>

<span data-ttu-id="bc7b3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc7b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

<span data-ttu-id="bc7b3-111">Beachten Sie, dass die Berechtigung je nach Workflow variiert.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="bc7b3-112">&nbsp;Berechtigungstyp&nbsp;(nach&nbsp;Workflow)</span><span class="sxs-lookup"><span data-stu-id="bc7b3-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="bc7b3-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc7b3-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="bc7b3-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc7b3-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="bc7b3-115">&nbsp;&nbsp; **Android for Work**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="bc7b3-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="bc7b3-117">&nbsp; &nbsp; **Überwachung**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="bc7b3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-119">&nbsp; &nbsp; **Geschäftsbedingungen des Unternehmens**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="bc7b3-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-121">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="bc7b3-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-123">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="bc7b3-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-125">&nbsp;&nbsp; **Elektronische SIM-Karte**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="bc7b3-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-127">&nbsp;&nbsp; **Registrierung**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="bc7b3-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-129">&nbsp;&nbsp; **Fechten**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="bc7b3-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-131">&nbsp; &nbsp; **Benachrichtigung**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="bc7b3-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-133">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="bc7b3-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-135">&nbsp; &nbsp; **Rollenbasierte Zugriffssteuerung**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="bc7b3-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-137">&nbsp; &nbsp; **Remotezugriff**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="bc7b3-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="bc7b3-139">&nbsp;&nbsp; **Remote Unterstützung**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="bc7b3-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-141">&nbsp;&nbsp; **Telekom-Spesenverwaltung**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="bc7b3-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-143">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="bc7b3-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-145">&nbsp;&nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="bc7b3-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7b3-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="bc7b3-147">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc7b3-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc7b3-148">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc7b3-148">Not supported.</span></span>|
| <span data-ttu-id="bc7b3-149">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc7b3-149">Application</span></span> | <span data-ttu-id="bc7b3-150">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc7b3-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc7b3-151">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc7b3-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="bc7b3-152">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc7b3-152">Request headers</span></span>

|<span data-ttu-id="bc7b3-153">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bc7b3-153">Header</span></span>|<span data-ttu-id="bc7b3-154">Wert</span><span class="sxs-lookup"><span data-stu-id="bc7b3-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc7b3-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc7b3-155">Authorization</span></span>|<span data-ttu-id="bc7b3-156">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc7b3-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc7b3-157">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bc7b3-157">Accept</span></span>|<span data-ttu-id="bc7b3-158">application/json</span><span class="sxs-lookup"><span data-stu-id="bc7b3-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc7b3-159">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc7b3-159">Request body</span></span>

<span data-ttu-id="bc7b3-160">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="bc7b3-161">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="bc7b3-162">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc7b3-162">Property</span></span>|<span data-ttu-id="bc7b3-163">Typ</span><span class="sxs-lookup"><span data-stu-id="bc7b3-163">Type</span></span>|<span data-ttu-id="bc7b3-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc7b3-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc7b3-165">id</span><span class="sxs-lookup"><span data-stu-id="bc7b3-165">id</span></span>|<span data-ttu-id="bc7b3-166">String</span><span class="sxs-lookup"><span data-stu-id="bc7b3-166">String</span></span>|<span data-ttu-id="bc7b3-167">Eindeutiger Bezeichner für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="bc7b3-168">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-168">**Device configuration**</span></span>|
|<span data-ttu-id="bc7b3-169">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="bc7b3-169">intuneAccountId</span></span>|<span data-ttu-id="bc7b3-170">GUID</span><span class="sxs-lookup"><span data-stu-id="bc7b3-170">GUID</span></span>|<span data-ttu-id="bc7b3-171">InTune-Konto-ID für angegebenen Mandanten</span><span class="sxs-lookup"><span data-stu-id="bc7b3-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="bc7b3-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="bc7b3-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="bc7b3-173">Boolesch</span><span class="sxs-lookup"><span data-stu-id="bc7b3-173">Boolean</span></span>|<span data-ttu-id="bc7b3-174">Die Eigenschaft zum Aktivieren der nicht-MDM-verwalteten Legacy-PC-Verwaltung für dieses Konto.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="bc7b3-175">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-175">This property is read-only.</span></span>|
|<span data-ttu-id="bc7b3-176">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="bc7b3-176">maximumDepTokens</span></span>|<span data-ttu-id="bc7b3-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bc7b3-177">Int32</span></span>|<span data-ttu-id="bc7b3-178">Maximale Anzahl der pro-Mandanten zulässigen DEP-Token.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="bc7b3-179">settings</span><span class="sxs-lookup"><span data-stu-id="bc7b3-179">settings</span></span>|[<span data-ttu-id="bc7b3-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="bc7b3-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="bc7b3-181">Einstellungen auf Kontoebene</span><span class="sxs-lookup"><span data-stu-id="bc7b3-181">Account level settings.</span></span>|
|<span data-ttu-id="bc7b3-182">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-182">**Device management**</span></span>|
|<span data-ttu-id="bc7b3-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="bc7b3-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="bc7b3-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc7b3-184">DateTimeOffset</span></span>|<span data-ttu-id="bc7b3-185">Das Datum & Zeitpunkt, zu dem die Mandantendaten zwischen scaleunits verschoben wurden.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="bc7b3-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="bc7b3-186">adminConsent</span></span>|[<span data-ttu-id="bc7b3-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="bc7b3-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="bc7b3-188">Informationen zur Administrator Einwilligung.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-188">Admin consent information.</span></span>|
|<span data-ttu-id="bc7b3-189">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="bc7b3-189">deviceProtectionOverview</span></span>|[<span data-ttu-id="bc7b3-190">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="bc7b3-190">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="bc7b3-191">Übersicht über Geräteschutz.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-191">Device protection overview.</span></span>|
|<span data-ttu-id="bc7b3-192">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="bc7b3-192">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="bc7b3-193">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="bc7b3-193">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="bc7b3-194">Regel zur Gerätebereinigung</span><span class="sxs-lookup"><span data-stu-id="bc7b3-194">Device cleanup rule</span></span>|
|<span data-ttu-id="bc7b3-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="bc7b3-195">subscriptionState</span></span>|[<span data-ttu-id="bc7b3-196">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="bc7b3-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="bc7b3-197">Abonnementstatus für Verwaltung mobiler Geräte des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="bc7b3-198">Mögliche Werte: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="bc7b3-199">Abonnements</span><span class="sxs-lookup"><span data-stu-id="bc7b3-199">subscriptions</span></span>|[<span data-ttu-id="bc7b3-200">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="bc7b3-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="bc7b3-201">Abonnement des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-201">Tenant's Subscription.</span></span> <span data-ttu-id="bc7b3-202">Mögliche Werte sind: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU` und `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="bc7b3-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="bc7b3-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="bc7b3-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="bc7b3-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="bc7b3-205">Übersicht über Malware für Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="bc7b3-206">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="bc7b3-206">**Onboarding**</span></span>|
|<span data-ttu-id="bc7b3-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="bc7b3-207">intuneBrand</span></span>|[<span data-ttu-id="bc7b3-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="bc7b3-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="bc7b3-209">„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="bc7b3-210">Die Unterstützung von Request Body-Eigenschaften variiert je nach Workflow.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="bc7b3-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc7b3-211">Response</span></span>
<span data-ttu-id="bc7b3-212">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc7b3-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc7b3-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc7b3-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc7b3-214">Request</span></span>

<span data-ttu-id="bc7b3-215">Nachfolgend finden Sie ein Beispiel für eine Anforderung nach dem Geräte Verwaltungs Workflow:</span><span class="sxs-lookup"><span data-stu-id="bc7b3-215">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="bc7b3-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc7b3-216">Response</span></span>

<span data-ttu-id="bc7b3-217">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-217">Here is an example of the response.</span></span> 

<span data-ttu-id="bc7b3-218">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bc7b3-219">ZurückgeGebene Eigenschaften unterscheiden sich je nach Workflow und Kontext.</span><span class="sxs-lookup"><span data-stu-id="bc7b3-219">Returned properties vary according to workflow and context.</span></span>

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



