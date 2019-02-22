---
title: Aktualisieren von „windowsPhone81GeneralConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3fdec86f5989c5ab215d651c65106c1d7f891a26
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159339"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="eb2a4-103">Aktualisieren von „windowsPhone81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="eb2a4-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="eb2a4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb2a4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb2a4-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-106">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb2a4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb2a4-107">Prerequisites</span></span>
<span data-ttu-id="eb2a4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eb2a4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb2a4-110">Permission type</span></span>|<span data-ttu-id="eb2a4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb2a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb2a4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb2a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb2a4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb2a4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb2a4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb2a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb2a4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb2a4-115">Not supported.</span></span>|
|<span data-ttu-id="eb2a4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb2a4-116">Application</span></span>|<span data-ttu-id="eb2a4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb2a4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb2a4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb2a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="eb2a4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb2a4-119">Request headers</span></span>
|<span data-ttu-id="eb2a4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eb2a4-120">Header</span></span>|<span data-ttu-id="eb2a4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb2a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb2a4-122">Authorization</span></span>|<span data-ttu-id="eb2a4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb2a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb2a4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eb2a4-124">Accept</span></span>|<span data-ttu-id="eb2a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb2a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb2a4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb2a4-126">Request body</span></span>
<span data-ttu-id="eb2a4-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-127">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="eb2a4-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-128">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="eb2a4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb2a4-129">Property</span></span>|<span data-ttu-id="eb2a4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="eb2a4-130">Type</span></span>|<span data-ttu-id="eb2a4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb2a4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb2a4-132">id</span><span class="sxs-lookup"><span data-stu-id="eb2a4-132">id</span></span>|<span data-ttu-id="eb2a4-133">string</span><span class="sxs-lookup"><span data-stu-id="eb2a4-133">String</span></span>|<span data-ttu-id="eb2a4-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="eb2a4-134">Key of the entity.</span></span> <span data-ttu-id="eb2a4-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb2a4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb2a4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="eb2a4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb2a4-137">DateTimeOffset</span></span>|<span data-ttu-id="eb2a4-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="eb2a4-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb2a4-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="eb2a4-140">roleScopeTagIds</span></span>|<span data-ttu-id="eb2a4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="eb2a4-141">String collection</span></span>|<span data-ttu-id="eb2a4-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="eb2a4-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb2a4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="eb2a4-144">supportsScopeTags</span></span>|<span data-ttu-id="eb2a4-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-145">Boolean</span></span>|<span data-ttu-id="eb2a4-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="eb2a4-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="eb2a4-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="eb2a4-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-149">This property is read-only.</span></span> <span data-ttu-id="eb2a4-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb2a4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb2a4-151">createdDateTime</span></span>|<span data-ttu-id="eb2a4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb2a4-152">DateTimeOffset</span></span>|<span data-ttu-id="eb2a4-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-153">DateTime the object was created.</span></span> <span data-ttu-id="eb2a4-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb2a4-155">description</span><span class="sxs-lookup"><span data-stu-id="eb2a4-155">description</span></span>|<span data-ttu-id="eb2a4-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb2a4-156">String</span></span>|<span data-ttu-id="eb2a4-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eb2a4-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb2a4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="eb2a4-159">displayName</span></span>|<span data-ttu-id="eb2a4-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb2a4-160">String</span></span>|<span data-ttu-id="eb2a4-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eb2a4-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb2a4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb2a4-163">Version</span><span class="sxs-lookup"><span data-stu-id="eb2a4-163">version</span></span>|<span data-ttu-id="eb2a4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="eb2a4-164">Int32</span></span>|<span data-ttu-id="eb2a4-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-165">Version of the device configuration.</span></span> <span data-ttu-id="eb2a4-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb2a4-167">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="eb2a4-167">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="eb2a4-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-168">Boolean</span></span>|<span data-ttu-id="eb2a4-169">Wert, der angibt, ob die Richtlinie nur für Windows Phone 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-169">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="eb2a4-170">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-170">This property is read-only.</span></span>|
|<span data-ttu-id="eb2a4-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="eb2a4-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="eb2a4-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-172">Boolean</span></span>|<span data-ttu-id="eb2a4-173">Gibt an, ob Kopieren/Einfügen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-173">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="eb2a4-174">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="eb2a4-174">bluetoothBlocked</span></span>|<span data-ttu-id="eb2a4-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-175">Boolean</span></span>|<span data-ttu-id="eb2a4-176">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-176">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="eb2a4-177">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="eb2a4-177">cameraBlocked</span></span>|<span data-ttu-id="eb2a4-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-178">Boolean</span></span>|<span data-ttu-id="eb2a4-179">Gibt an, ob die Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-179">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="eb2a4-180">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="eb2a4-180">cellularBlockWifiTethering</span></span>|<span data-ttu-id="eb2a4-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-181">Boolean</span></span>|<span data-ttu-id="eb2a4-182">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-182">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="eb2a4-183">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-183">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="eb2a4-184">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="eb2a4-184">compliantAppsList</span></span>|<span data-ttu-id="eb2a4-185">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="eb2a4-185">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="eb2a4-186">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="eb2a4-186">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="eb2a4-187">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-187">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="eb2a4-188">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="eb2a4-188">compliantAppListType</span></span>|[<span data-ttu-id="eb2a4-189">appListType</span><span class="sxs-lookup"><span data-stu-id="eb2a4-189">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="eb2a4-190">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-190">List that is in the AppComplianceList.</span></span> <span data-ttu-id="eb2a4-191">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-191">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="eb2a4-192">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="eb2a4-192">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="eb2a4-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-193">Boolean</span></span>|<span data-ttu-id="eb2a4-194">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-194">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="eb2a4-195">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="eb2a4-195">emailBlockAddingAccounts</span></span>|<span data-ttu-id="eb2a4-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-196">Boolean</span></span>|<span data-ttu-id="eb2a4-197">Gibt an, ob benutzerdefinierte E-Mail-Konten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-197">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="eb2a4-198">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="eb2a4-198">locationServicesBlocked</span></span>|<span data-ttu-id="eb2a4-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb2a4-199">Boolean</span></span>|<span data-ttu-id="eb2a4-200">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-200">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="eb2a4-201">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="eb2a4-201">microsoftAccountBlocked</span></span>|<span data-ttu-id="eb2a4-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb2a4-202">Boolean</span></span>|<span data-ttu-id="eb2a4-203">Gibt an, ob die Verwendung eines Microsoft-Kontos erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-203">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="eb2a4-204">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="eb2a4-204">nfcBlocked</span></span>|<span data-ttu-id="eb2a4-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-205">Boolean</span></span>|<span data-ttu-id="eb2a4-206">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-206">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="eb2a4-207">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="eb2a4-207">passwordBlockSimple</span></span>|<span data-ttu-id="eb2a4-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-208">Boolean</span></span>|<span data-ttu-id="eb2a4-209">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-209">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="eb2a4-210">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="eb2a4-210">passwordExpirationDays</span></span>|<span data-ttu-id="eb2a4-211">Int32</span><span class="sxs-lookup"><span data-stu-id="eb2a4-211">Int32</span></span>|<span data-ttu-id="eb2a4-212">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-212">Number of days before the password expires.</span></span>|
|<span data-ttu-id="eb2a4-213">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="eb2a4-213">passwordMinimumLength</span></span>|<span data-ttu-id="eb2a4-214">Int32</span><span class="sxs-lookup"><span data-stu-id="eb2a4-214">Int32</span></span>|<span data-ttu-id="eb2a4-215">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-215">Minimum length of passwords.</span></span>|
|<span data-ttu-id="eb2a4-216">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="eb2a4-216">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="eb2a4-217">Int32</span><span class="sxs-lookup"><span data-stu-id="eb2a4-217">Int32</span></span>|<span data-ttu-id="eb2a4-218">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="eb2a4-218">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="eb2a4-219">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="eb2a4-219">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="eb2a4-220">Int32</span><span class="sxs-lookup"><span data-stu-id="eb2a4-220">Int32</span></span>|<span data-ttu-id="eb2a4-221">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss</span><span class="sxs-lookup"><span data-stu-id="eb2a4-221">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="eb2a4-222">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="eb2a4-222">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="eb2a4-223">Int32</span><span class="sxs-lookup"><span data-stu-id="eb2a4-223">Int32</span></span>|<span data-ttu-id="eb2a4-224">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-224">Number of previous passwords to block.</span></span> <span data-ttu-id="eb2a4-225">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-225">Valid values 0 to 24</span></span>|
|<span data-ttu-id="eb2a4-226">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="eb2a4-226">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="eb2a4-227">Int32</span><span class="sxs-lookup"><span data-stu-id="eb2a4-227">Int32</span></span>|<span data-ttu-id="eb2a4-228">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-228">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="eb2a4-229">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="eb2a4-229">passwordRequiredType</span></span>|[<span data-ttu-id="eb2a4-230">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="eb2a4-230">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="eb2a4-231">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-231">Password type that is required.</span></span> <span data-ttu-id="eb2a4-232">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-232">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="eb2a4-233">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="eb2a4-233">passwordRequired</span></span>|<span data-ttu-id="eb2a4-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-234">Boolean</span></span>|<span data-ttu-id="eb2a4-235">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-235">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="eb2a4-236">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="eb2a4-236">screenCaptureBlocked</span></span>|<span data-ttu-id="eb2a4-237">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-237">Boolean</span></span>|<span data-ttu-id="eb2a4-238">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-238">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="eb2a4-239">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="eb2a4-239">storageBlockRemovableStorage</span></span>|<span data-ttu-id="eb2a4-240">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-240">Boolean</span></span>|<span data-ttu-id="eb2a4-241">Gibt an, ob Wechselmedien blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-241">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="eb2a4-242">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="eb2a4-242">storageRequireEncryption</span></span>|<span data-ttu-id="eb2a4-243">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-243">Boolean</span></span>|<span data-ttu-id="eb2a4-244">Gibt an, ob Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-244">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="eb2a4-245">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="eb2a4-245">webBrowserBlocked</span></span>|<span data-ttu-id="eb2a4-246">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-246">Boolean</span></span>|<span data-ttu-id="eb2a4-247">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-247">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="eb2a4-248">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="eb2a4-248">wifiBlocked</span></span>|<span data-ttu-id="eb2a4-249">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-249">Boolean</span></span>|<span data-ttu-id="eb2a4-250">Gibt an, ob die WLAN-Funktion blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-250">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="eb2a4-251">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="eb2a4-251">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="eb2a4-252">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-252">Boolean</span></span>|<span data-ttu-id="eb2a4-253">Gibt an, ob die automatische Herstellung einer Verbindung zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-253">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="eb2a4-254">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-254">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="eb2a4-255">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="eb2a4-255">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="eb2a4-256">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eb2a4-256">Boolean</span></span>|<span data-ttu-id="eb2a4-257">Gibt an, ob die Erstellung von Berichten zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-257">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="eb2a4-258">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-258">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="eb2a4-259">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="eb2a4-259">windowsStoreBlocked</span></span>|<span data-ttu-id="eb2a4-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb2a4-260">Boolean</span></span>|<span data-ttu-id="eb2a4-261">Gibt an, ob der Windows Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-261">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="eb2a4-262">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb2a4-262">Response</span></span>
<span data-ttu-id="eb2a4-263">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-263">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb2a4-264">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb2a4-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb2a4-265">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb2a4-265">Request</span></span>
<span data-ttu-id="eb2a4-266">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1553

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="eb2a4-267">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb2a4-267">Response</span></span>
<span data-ttu-id="eb2a4-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb2a4-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1725

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```




