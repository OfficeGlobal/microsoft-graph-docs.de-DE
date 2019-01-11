---
title: Erstellen von „windowsPhone81GeneralConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7e406d043d063434d5accb4b89748ab612717ae3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815246"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="83ce0-103">Erstellen von „windowsPhone81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="83ce0-103">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="83ce0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="83ce0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83ce0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83ce0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83ce0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="83ce0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83ce0-107">Diese Methode erstellt ein neues Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83ce0-107">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83ce0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="83ce0-108">Prerequisites</span></span>
<span data-ttu-id="83ce0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83ce0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83ce0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="83ce0-111">Permission type</span></span>|<span data-ttu-id="83ce0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="83ce0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83ce0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="83ce0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83ce0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83ce0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83ce0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="83ce0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83ce0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83ce0-116">Not supported.</span></span>|
|<span data-ttu-id="83ce0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="83ce0-117">Application</span></span>|<span data-ttu-id="83ce0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83ce0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83ce0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="83ce0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="83ce0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="83ce0-120">Request headers</span></span>
|<span data-ttu-id="83ce0-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="83ce0-121">Header</span></span>|<span data-ttu-id="83ce0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="83ce0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83ce0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83ce0-123">Authorization</span></span>|<span data-ttu-id="83ce0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="83ce0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83ce0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="83ce0-125">Accept</span></span>|<span data-ttu-id="83ce0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83ce0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83ce0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="83ce0-127">Request body</span></span>
<span data-ttu-id="83ce0-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsPhone81GeneralConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="83ce0-128">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="83ce0-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsPhone81GeneralConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="83ce0-129">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="83ce0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83ce0-130">Property</span></span>|<span data-ttu-id="83ce0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="83ce0-131">Type</span></span>|<span data-ttu-id="83ce0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83ce0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83ce0-133">id</span><span class="sxs-lookup"><span data-stu-id="83ce0-133">id</span></span>|<span data-ttu-id="83ce0-134">String</span><span class="sxs-lookup"><span data-stu-id="83ce0-134">String</span></span>|<span data-ttu-id="83ce0-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="83ce0-135">Key of the entity.</span></span> <span data-ttu-id="83ce0-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83ce0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ce0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83ce0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="83ce0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83ce0-138">DateTimeOffset</span></span>|<span data-ttu-id="83ce0-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="83ce0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="83ce0-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83ce0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ce0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83ce0-141">roleScopeTagIds</span></span>|<span data-ttu-id="83ce0-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="83ce0-142">String collection</span></span>|<span data-ttu-id="83ce0-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="83ce0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83ce0-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83ce0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ce0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="83ce0-145">supportsScopeTags</span></span>|<span data-ttu-id="83ce0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-146">Boolean</span></span>|<span data-ttu-id="83ce0-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83ce0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="83ce0-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="83ce0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="83ce0-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="83ce0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="83ce0-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="83ce0-150">This property is read-only.</span></span> <span data-ttu-id="83ce0-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83ce0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ce0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83ce0-152">createdDateTime</span></span>|<span data-ttu-id="83ce0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83ce0-153">DateTimeOffset</span></span>|<span data-ttu-id="83ce0-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="83ce0-154">DateTime the object was created.</span></span> <span data-ttu-id="83ce0-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83ce0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ce0-156">description</span><span class="sxs-lookup"><span data-stu-id="83ce0-156">description</span></span>|<span data-ttu-id="83ce0-157">String</span><span class="sxs-lookup"><span data-stu-id="83ce0-157">String</span></span>|<span data-ttu-id="83ce0-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="83ce0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83ce0-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83ce0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ce0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="83ce0-160">displayName</span></span>|<span data-ttu-id="83ce0-161">String</span><span class="sxs-lookup"><span data-stu-id="83ce0-161">String</span></span>|<span data-ttu-id="83ce0-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="83ce0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83ce0-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83ce0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ce0-164">Version</span><span class="sxs-lookup"><span data-stu-id="83ce0-164">version</span></span>|<span data-ttu-id="83ce0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="83ce0-165">Int32</span></span>|<span data-ttu-id="83ce0-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="83ce0-166">Version of the device configuration.</span></span> <span data-ttu-id="83ce0-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83ce0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ce0-168">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="83ce0-168">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="83ce0-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-169">Boolean</span></span>|<span data-ttu-id="83ce0-170">Wert, der angibt, ob die Richtlinie nur für Windows Phone 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="83ce0-170">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="83ce0-171">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="83ce0-171">This property is read-only.</span></span>|
|<span data-ttu-id="83ce0-172">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="83ce0-172">appsBlockCopyPaste</span></span>|<span data-ttu-id="83ce0-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-173">Boolean</span></span>|<span data-ttu-id="83ce0-174">Gibt an, ob Kopieren/Einfügen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-174">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="83ce0-175">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="83ce0-175">bluetoothBlocked</span></span>|<span data-ttu-id="83ce0-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-176">Boolean</span></span>|<span data-ttu-id="83ce0-177">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-177">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="83ce0-178">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="83ce0-178">cameraBlocked</span></span>|<span data-ttu-id="83ce0-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-179">Boolean</span></span>|<span data-ttu-id="83ce0-180">Gibt an, ob die Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-180">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="83ce0-181">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="83ce0-181">cellularBlockWifiTethering</span></span>|<span data-ttu-id="83ce0-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-182">Boolean</span></span>|<span data-ttu-id="83ce0-183">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-183">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="83ce0-184">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="83ce0-184">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="83ce0-185">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="83ce0-185">compliantAppsList</span></span>|<span data-ttu-id="83ce0-186">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="83ce0-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="83ce0-187">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="83ce0-187">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="83ce0-188">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="83ce0-188">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="83ce0-189">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="83ce0-189">compliantAppListType</span></span>|[<span data-ttu-id="83ce0-190">appListType</span><span class="sxs-lookup"><span data-stu-id="83ce0-190">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="83ce0-191">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="83ce0-191">List that is in the AppComplianceList.</span></span> <span data-ttu-id="83ce0-192">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="83ce0-192">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="83ce0-193">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="83ce0-193">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="83ce0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-194">Boolean</span></span>|<span data-ttu-id="83ce0-195">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-195">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="83ce0-196">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="83ce0-196">emailBlockAddingAccounts</span></span>|<span data-ttu-id="83ce0-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-197">Boolean</span></span>|<span data-ttu-id="83ce0-198">Gibt an, ob benutzerdefinierte E-Mail-Konten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="83ce0-198">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="83ce0-199">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="83ce0-199">locationServicesBlocked</span></span>|<span data-ttu-id="83ce0-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-200">Boolean</span></span>|<span data-ttu-id="83ce0-201">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="83ce0-201">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="83ce0-202">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="83ce0-202">microsoftAccountBlocked</span></span>|<span data-ttu-id="83ce0-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-203">Boolean</span></span>|<span data-ttu-id="83ce0-204">Gibt an, ob die Verwendung eines Microsoft-Kontos erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="83ce0-204">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="83ce0-205">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="83ce0-205">nfcBlocked</span></span>|<span data-ttu-id="83ce0-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-206">Boolean</span></span>|<span data-ttu-id="83ce0-207">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-207">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="83ce0-208">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="83ce0-208">passwordBlockSimple</span></span>|<span data-ttu-id="83ce0-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-209">Boolean</span></span>|<span data-ttu-id="83ce0-210">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-210">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="83ce0-211">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="83ce0-211">passwordExpirationDays</span></span>|<span data-ttu-id="83ce0-212">Int32</span><span class="sxs-lookup"><span data-stu-id="83ce0-212">Int32</span></span>|<span data-ttu-id="83ce0-213">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="83ce0-213">Number of days before the password expires.</span></span>|
|<span data-ttu-id="83ce0-214">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="83ce0-214">passwordMinimumLength</span></span>|<span data-ttu-id="83ce0-215">Int32</span><span class="sxs-lookup"><span data-stu-id="83ce0-215">Int32</span></span>|<span data-ttu-id="83ce0-216">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="83ce0-216">Minimum length of passwords.</span></span>|
|<span data-ttu-id="83ce0-217">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="83ce0-217">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="83ce0-218">Int32</span><span class="sxs-lookup"><span data-stu-id="83ce0-218">Int32</span></span>|<span data-ttu-id="83ce0-219">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="83ce0-219">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="83ce0-220">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="83ce0-220">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="83ce0-221">Int32</span><span class="sxs-lookup"><span data-stu-id="83ce0-221">Int32</span></span>|<span data-ttu-id="83ce0-222">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss</span><span class="sxs-lookup"><span data-stu-id="83ce0-222">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="83ce0-223">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="83ce0-223">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="83ce0-224">Int32</span><span class="sxs-lookup"><span data-stu-id="83ce0-224">Int32</span></span>|<span data-ttu-id="83ce0-225">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="83ce0-225">Number of previous passwords to block.</span></span> <span data-ttu-id="83ce0-226">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="83ce0-226">Valid values 0 to 24</span></span>|
|<span data-ttu-id="83ce0-227">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="83ce0-227">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="83ce0-228">Int32</span><span class="sxs-lookup"><span data-stu-id="83ce0-228">Int32</span></span>|<span data-ttu-id="83ce0-229">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="83ce0-229">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="83ce0-230">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="83ce0-230">passwordRequiredType</span></span>|[<span data-ttu-id="83ce0-231">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="83ce0-231">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="83ce0-232">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="83ce0-232">Password type that is required.</span></span> <span data-ttu-id="83ce0-233">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="83ce0-233">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="83ce0-234">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="83ce0-234">passwordRequired</span></span>|<span data-ttu-id="83ce0-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-235">Boolean</span></span>|<span data-ttu-id="83ce0-236">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="83ce0-236">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="83ce0-237">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="83ce0-237">screenCaptureBlocked</span></span>|<span data-ttu-id="83ce0-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-238">Boolean</span></span>|<span data-ttu-id="83ce0-239">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="83ce0-239">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="83ce0-240">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="83ce0-240">storageBlockRemovableStorage</span></span>|<span data-ttu-id="83ce0-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-241">Boolean</span></span>|<span data-ttu-id="83ce0-242">Gibt an, ob Wechselmedien blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="83ce0-242">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="83ce0-243">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="83ce0-243">storageRequireEncryption</span></span>|<span data-ttu-id="83ce0-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-244">Boolean</span></span>|<span data-ttu-id="83ce0-245">Gibt an, ob Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="83ce0-245">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="83ce0-246">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="83ce0-246">webBrowserBlocked</span></span>|<span data-ttu-id="83ce0-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-247">Boolean</span></span>|<span data-ttu-id="83ce0-248">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-248">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="83ce0-249">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="83ce0-249">wifiBlocked</span></span>|<span data-ttu-id="83ce0-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-250">Boolean</span></span>|<span data-ttu-id="83ce0-251">Gibt an, ob die WLAN-Funktion blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-251">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="83ce0-252">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="83ce0-252">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="83ce0-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-253">Boolean</span></span>|<span data-ttu-id="83ce0-254">Gibt an, ob die automatische Herstellung einer Verbindung zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-254">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="83ce0-255">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="83ce0-255">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="83ce0-256">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="83ce0-256">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="83ce0-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-257">Boolean</span></span>|<span data-ttu-id="83ce0-258">Gibt an, ob die Erstellung von Berichten zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-258">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="83ce0-259">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="83ce0-259">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="83ce0-260">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="83ce0-260">windowsStoreBlocked</span></span>|<span data-ttu-id="83ce0-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ce0-261">Boolean</span></span>|<span data-ttu-id="83ce0-262">Gibt an, ob der Windows Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="83ce0-262">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="83ce0-263">Antwort</span><span class="sxs-lookup"><span data-stu-id="83ce0-263">Response</span></span>
<span data-ttu-id="83ce0-264">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="83ce0-264">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83ce0-265">Beispiel</span><span class="sxs-lookup"><span data-stu-id="83ce0-265">Example</span></span>
### <a name="request"></a><span data-ttu-id="83ce0-266">Anforderung</span><span class="sxs-lookup"><span data-stu-id="83ce0-266">Request</span></span>
<span data-ttu-id="83ce0-267">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83ce0-267">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1617

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="83ce0-268">Antwort</span><span class="sxs-lookup"><span data-stu-id="83ce0-268">Response</span></span>
<span data-ttu-id="83ce0-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="83ce0-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





