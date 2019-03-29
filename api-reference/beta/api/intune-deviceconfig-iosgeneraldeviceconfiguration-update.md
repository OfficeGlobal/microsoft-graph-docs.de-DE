---
title: iosGeneralDeviceConfiguration aktualisieren
description: Aktualisiert die Eigenschaften eines iosDeviceFeaturesConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f72ae25934e08c228375dbfefc6a243e87792b82
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974363"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="65ed3-103">iosGeneralDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="65ed3-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="65ed3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65ed3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65ed3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="65ed3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65ed3-106">Aktualisiert die Eigenschaften eines [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="65ed3-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65ed3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="65ed3-107">Prerequisites</span></span>
<span data-ttu-id="65ed3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65ed3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65ed3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65ed3-110">Permission type</span></span>|<span data-ttu-id="65ed3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65ed3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65ed3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65ed3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65ed3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65ed3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65ed3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65ed3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65ed3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65ed3-115">Not supported.</span></span>|
|<span data-ttu-id="65ed3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65ed3-116">Application</span></span>|<span data-ttu-id="65ed3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65ed3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65ed3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65ed3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="65ed3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65ed3-119">Request headers</span></span>
|<span data-ttu-id="65ed3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="65ed3-120">Header</span></span>|<span data-ttu-id="65ed3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65ed3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65ed3-122">Authorization</span></span>|<span data-ttu-id="65ed3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="65ed3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65ed3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="65ed3-124">Accept</span></span>|<span data-ttu-id="65ed3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65ed3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65ed3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65ed3-126">Request body</span></span>
<span data-ttu-id="65ed3-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="65ed3-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="65ed3-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="65ed3-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="65ed3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65ed3-129">Property</span></span>|<span data-ttu-id="65ed3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="65ed3-130">Type</span></span>|<span data-ttu-id="65ed3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65ed3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65ed3-132">id</span><span class="sxs-lookup"><span data-stu-id="65ed3-132">id</span></span>|<span data-ttu-id="65ed3-133">String</span><span class="sxs-lookup"><span data-stu-id="65ed3-133">String</span></span>|<span data-ttu-id="65ed3-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="65ed3-134">Key of the entity.</span></span> <span data-ttu-id="65ed3-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65ed3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65ed3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65ed3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="65ed3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65ed3-137">DateTimeOffset</span></span>|<span data-ttu-id="65ed3-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="65ed3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="65ed3-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65ed3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65ed3-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="65ed3-140">roleScopeTagIds</span></span>|<span data-ttu-id="65ed3-141">String collection</span><span class="sxs-lookup"><span data-stu-id="65ed3-141">String collection</span></span>|<span data-ttu-id="65ed3-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="65ed3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="65ed3-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65ed3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65ed3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="65ed3-144">supportsScopeTags</span></span>|<span data-ttu-id="65ed3-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-145">Boolean</span></span>|<span data-ttu-id="65ed3-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65ed3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="65ed3-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="65ed3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="65ed3-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="65ed3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="65ed3-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="65ed3-149">This property is read-only.</span></span> <span data-ttu-id="65ed3-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65ed3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65ed3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65ed3-151">createdDateTime</span></span>|<span data-ttu-id="65ed3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65ed3-152">DateTimeOffset</span></span>|<span data-ttu-id="65ed3-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="65ed3-153">DateTime the object was created.</span></span> <span data-ttu-id="65ed3-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65ed3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65ed3-155">description</span><span class="sxs-lookup"><span data-stu-id="65ed3-155">description</span></span>|<span data-ttu-id="65ed3-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65ed3-156">String</span></span>|<span data-ttu-id="65ed3-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="65ed3-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="65ed3-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65ed3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65ed3-159">displayName</span><span class="sxs-lookup"><span data-stu-id="65ed3-159">displayName</span></span>|<span data-ttu-id="65ed3-160">String</span><span class="sxs-lookup"><span data-stu-id="65ed3-160">String</span></span>|<span data-ttu-id="65ed3-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="65ed3-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="65ed3-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65ed3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65ed3-163">Version</span><span class="sxs-lookup"><span data-stu-id="65ed3-163">version</span></span>|<span data-ttu-id="65ed3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="65ed3-164">Int32</span></span>|<span data-ttu-id="65ed3-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="65ed3-165">Version of the device configuration.</span></span> <span data-ttu-id="65ed3-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65ed3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65ed3-167">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-167">accountBlockModification</span></span>|<span data-ttu-id="65ed3-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-168">Boolean</span></span>|<span data-ttu-id="65ed3-169">Gibt an, ob die Kontoänderung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-169">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-170">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="65ed3-170">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="65ed3-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-171">Boolean</span></span>|<span data-ttu-id="65ed3-172">Gibt an, ob die Aktivierungssperre zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-172">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="65ed3-173">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-173">airDropBlocked</span></span>|<span data-ttu-id="65ed3-174">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-174">Boolean</span></span>|<span data-ttu-id="65ed3-175">Gibt an, ob AirDrop zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-175">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-176">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="65ed3-176">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="65ed3-177">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-177">Boolean</span></span>|<span data-ttu-id="65ed3-178">Gibt an, ob AirDrop als nicht verwaltetes Drop-Ziel (iOS 9.0 oder höher) betrachtet werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-178">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="65ed3-179">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="65ed3-179">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="65ed3-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-180">Boolean</span></span>|<span data-ttu-id="65ed3-181">Gibt an, ob erzwungen werden soll, dass alle Geräte, die AirPlay-Anforderungen von diesem Gerät erhalten, ein Kopplungskennwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="65ed3-181">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="65ed3-182">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="65ed3-182">appleWatchBlockPairing</span></span>|<span data-ttu-id="65ed3-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-183">Boolean</span></span>|<span data-ttu-id="65ed3-184">Gibt an, ob eine Apple Watch-Kopplung zulässig ist, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-184">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="65ed3-185">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="65ed3-185">appleWatchForceWristDetection</span></span>|<span data-ttu-id="65ed3-186">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-186">Boolean</span></span>|<span data-ttu-id="65ed3-187">Gibt an, ob erzwungen werden soll, dass eine gekoppelte Apple Watch die Handgelenkerkennung (iOS 8.2 und höher) verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-187">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="65ed3-188">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-188">appleNewsBlocked</span></span>|<span data-ttu-id="65ed3-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-189">Boolean</span></span>|<span data-ttu-id="65ed3-190">Gibt an, ob verhindert werden soll, dass der Benutzer News verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-190">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="65ed3-191">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="65ed3-191">appsSingleAppModeList</span></span>|<span data-ttu-id="65ed3-192">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="65ed3-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="65ed3-193">Ruft die Liste von iOS-Apps ab, die autonom in den Einzelanwendungsmodus wechseln können, ab oder legt diese fest.</span><span class="sxs-lookup"><span data-stu-id="65ed3-193">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="65ed3-194">Nur überwacht.</span><span class="sxs-lookup"><span data-stu-id="65ed3-194">Supervised only.</span></span> <span data-ttu-id="65ed3-195">iOS 7.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="65ed3-195">iOS 7.0 and later.</span></span> <span data-ttu-id="65ed3-196">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="65ed3-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="65ed3-197">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="65ed3-197">appsVisibilityList</span></span>|<span data-ttu-id="65ed3-198">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="65ed3-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="65ed3-199">Liste von Apps in der Sichtbarkeitsliste (entweder eine Liste sichtbarer/startbarer Apps oder eine Liste ausgeblendeter/nicht startbarer Apps, gesteuert von AppsVisibilityListType) (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-199">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="65ed3-200">Diese Sammlung darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="65ed3-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="65ed3-201">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="65ed3-201">appsVisibilityListType</span></span>|[<span data-ttu-id="65ed3-202">appListType</span><span class="sxs-lookup"><span data-stu-id="65ed3-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="65ed3-203">Typ der in „AppsVisibilityList“ enthaltenen Liste.</span><span class="sxs-lookup"><span data-stu-id="65ed3-203">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="65ed3-204">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="65ed3-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="65ed3-205">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="65ed3-205">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="65ed3-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-206">Boolean</span></span>|<span data-ttu-id="65ed3-207">Gibt an, ob das automatische Herunterladen von Apps blockiert werden soll, die auf anderen Geräten gekauft wurden, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-207">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="65ed3-208">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-208">appStoreBlocked</span></span>|<span data-ttu-id="65ed3-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-209">Boolean</span></span>|<span data-ttu-id="65ed3-210">Gibt an, ob verhindert werden soll, dass der Benutzer den App Store verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-210">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="65ed3-211">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="65ed3-211">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="65ed3-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-212">Boolean</span></span>|<span data-ttu-id="65ed3-213">Gibt an, ob verhindert werden soll, dass der Benutzer In-App-Käufe tätigt.</span><span class="sxs-lookup"><span data-stu-id="65ed3-213">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="65ed3-214">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="65ed3-214">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="65ed3-215">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-215">Boolean</span></span>|<span data-ttu-id="65ed3-216">Gibt an, ob die App Store-App blockiert werden soll, ohne die Installation über Host-Apps einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="65ed3-216">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="65ed3-217">Gilt nur für den überwachten Modus (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-217">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="65ed3-218">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="65ed3-218">appStoreRequirePassword</span></span>|<span data-ttu-id="65ed3-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="65ed3-219">Boolean</span></span>|<span data-ttu-id="65ed3-220">Gibt an, ob bei Verwendung des App Stores ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-220">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="65ed3-221">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="65ed3-221">autoFillForceAuthentication</span></span>|<span data-ttu-id="65ed3-222">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-222">Boolean</span></span>|<span data-ttu-id="65ed3-223">Gibt an, ob die Benutzerauthentifizierung erzwungen werden soll, bevor Kennwörter und Kreditkarteninformationen in Safari und anderen apps auf überwachten Geräten automatisch gefüllt werden.</span><span class="sxs-lookup"><span data-stu-id="65ed3-223">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="65ed3-224">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-224">bluetoothBlockModification</span></span>|<span data-ttu-id="65ed3-225">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-225">Boolean</span></span>|<span data-ttu-id="65ed3-226">Gibt an, ob das Ändern von Bluetooth-Einstellungen zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 10.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-226">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="65ed3-227">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-227">cameraBlocked</span></span>|<span data-ttu-id="65ed3-228">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-228">Boolean</span></span>|<span data-ttu-id="65ed3-229">Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.</span><span class="sxs-lookup"><span data-stu-id="65ed3-229">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="65ed3-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="65ed3-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="65ed3-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-231">Boolean</span></span>|<span data-ttu-id="65ed3-232">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="65ed3-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="65ed3-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="65ed3-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-234">Boolean</span></span>|<span data-ttu-id="65ed3-235">Gibt an, ob das globales Abrufen im Hintergrund beim Roaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-235">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="65ed3-236">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-236">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="65ed3-237">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-237">Boolean</span></span>|<span data-ttu-id="65ed3-238">Gibt an, ob Änderungen an den Mobil-App-Daten zulässig sind, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-238">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-239">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="65ed3-239">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="65ed3-240">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-240">Boolean</span></span>|<span data-ttu-id="65ed3-241">Gibt an, ob der privater Hotspot blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-241">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="65ed3-242">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-242">cellularBlockPlanModification</span></span>|<span data-ttu-id="65ed3-243">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-243">Boolean</span></span>|<span data-ttu-id="65ed3-244">Gibt an, ob Benutzer die Einstellungen des Mobil Funk Plans auf einem überwachten Gerät ändern dürfen.</span><span class="sxs-lookup"><span data-stu-id="65ed3-244">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="65ed3-245">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="65ed3-245">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="65ed3-246">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-246">Boolean</span></span>|<span data-ttu-id="65ed3-247">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-247">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="65ed3-248">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="65ed3-248">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="65ed3-249">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-249">Boolean</span></span>|<span data-ttu-id="65ed3-250">Gibt an, ob nicht vertrauenswürdige TLS-Zertifikate blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="65ed3-250">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="65ed3-251">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="65ed3-251">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="65ed3-252">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-252">Boolean</span></span>|<span data-ttu-id="65ed3-253">Gibt an, ob die Remotebildschirmüberwachung über die Classroom-App zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-253">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="65ed3-254">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="65ed3-254">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="65ed3-255">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-255">Boolean</span></span>|<span data-ttu-id="65ed3-256">Gibt an, ob dem Lehrer eines verwalteten Kurses in der Classroom-App automatisch die Berechtigung erteilt werden soll, den Bildschirm eines Kursteilnehmers ohne Aufforderung anzuzeigen, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-256">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-257">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="65ed3-257">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="65ed3-258">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-258">Boolean</span></span>|<span data-ttu-id="65ed3-259">Gibt an, ob die Berechtigung für die Anforderungen des Lehrers automatisch erteilt werden soll, ohne dass der Kursteilnehmer dazu aufgefordert wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-259">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-260">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="65ed3-260">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="65ed3-261">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-261">Boolean</span></span>|<span data-ttu-id="65ed3-262">Gibt an, ob die Lehrerin Apps oder das Gerät Sperren soll, ohne dass der Kursteilnehmer dazu aufgefordert wird.</span><span class="sxs-lookup"><span data-stu-id="65ed3-262">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="65ed3-263">Nur überwacht.</span><span class="sxs-lookup"><span data-stu-id="65ed3-263">Supervised only.</span></span>|
|<span data-ttu-id="65ed3-264">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="65ed3-264">compliantAppsList</span></span>|<span data-ttu-id="65ed3-265">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="65ed3-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="65ed3-266">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="65ed3-266">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="65ed3-267">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="65ed3-267">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="65ed3-268">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="65ed3-268">compliantAppListType</span></span>|[<span data-ttu-id="65ed3-269">appListType</span><span class="sxs-lookup"><span data-stu-id="65ed3-269">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="65ed3-270">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="65ed3-270">List that is in the AppComplianceList.</span></span> <span data-ttu-id="65ed3-271">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="65ed3-271">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="65ed3-272">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="65ed3-272">configurationProfileBlockChanges</span></span>|<span data-ttu-id="65ed3-273">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-273">Boolean</span></span>|<span data-ttu-id="65ed3-274">Gibt an, ob verhindert werden soll, dass der Benutzer Konfigurationsprofile und Zertifikate interaktiv installiert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-274">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-275">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-275">definitionLookupBlocked</span></span>|<span data-ttu-id="65ed3-276">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-276">Boolean</span></span>|<span data-ttu-id="65ed3-277">Gibt an, ob die Definitionssuche zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-277">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="65ed3-278">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="65ed3-278">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="65ed3-279">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-279">Boolean</span></span>|<span data-ttu-id="65ed3-280">Gibt an, ob erlaubt werden soll, dass der Benutzer Einschränkungen in den Geräteeinstellungen aktiviert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-280">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-281">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="65ed3-281">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="65ed3-282">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-282">Boolean</span></span>|<span data-ttu-id="65ed3-283">Gibt an, ob die Verwendung der Option zum Löschen aller Inhalte und Einstellungen auf dem Gerät zugelassen werden soll, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-283">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-284">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-284">deviceBlockNameModification</span></span>|<span data-ttu-id="65ed3-285">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-285">Boolean</span></span>|<span data-ttu-id="65ed3-286">Gibt an, ob das Ändern des Gerätenamens zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-286">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="65ed3-287">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="65ed3-287">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="65ed3-288">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-288">Boolean</span></span>|<span data-ttu-id="65ed3-289">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-289">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="65ed3-290">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-290">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="65ed3-291">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-291">Boolean</span></span>|<span data-ttu-id="65ed3-292">Gibt an, ob das Ändern der Einstellungen für die Diagnoseübermittlung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3.2 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-292">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="65ed3-293">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="65ed3-293">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="65ed3-294">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-294">Boolean</span></span>|<span data-ttu-id="65ed3-295">Gibt an, ob verhindert werden soll, dass der Benutzer verwaltete Dokumente in nicht verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="65ed3-295">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="65ed3-296">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="65ed3-296">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="65ed3-297">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-297">Boolean</span></span>|<span data-ttu-id="65ed3-298">Gibt an, ob verhindert werden soll, dass der Benutzer nicht verwaltete Dokumente in verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="65ed3-298">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="65ed3-299">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="65ed3-299">emailInDomainSuffixes</span></span>|<span data-ttu-id="65ed3-300">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="65ed3-300">String collection</span></span>|<span data-ttu-id="65ed3-301">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="65ed3-301">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="65ed3-302">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="65ed3-302">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="65ed3-303">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-303">Boolean</span></span>|<span data-ttu-id="65ed3-304">Gibt an, ob verhindert werden soll, dass der Benutzer einer Unternehmens-App vertraut.</span><span class="sxs-lookup"><span data-stu-id="65ed3-304">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="65ed3-305">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-305">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="65ed3-306">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-306">Boolean</span></span>|<span data-ttu-id="65ed3-307">Gibt an, ob verhindert werden soll, dass der Benutzer die Vertrauensstellungseinstellungen der Unternehmens-App ändert.</span><span class="sxs-lookup"><span data-stu-id="65ed3-307">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="65ed3-308">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-308">esimBlockModification</span></span>|<span data-ttu-id="65ed3-309">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-309">Boolean</span></span>|<span data-ttu-id="65ed3-310">Gibt an, ob das Hinzufügen oder Entfernen von Zellen Plänen auf dem eSIM eines überwachten Geräts zugelassen werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-310">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="65ed3-311">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-311">faceTimeBlocked</span></span>|<span data-ttu-id="65ed3-312">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-312">Boolean</span></span>|<span data-ttu-id="65ed3-313">Gibt an, ob verhindert werden soll, dass der Benutzer FaceTime verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-313">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="65ed3-314">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-314">findMyFriendsBlocked</span></span>|<span data-ttu-id="65ed3-315">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-315">Boolean</span></span>|<span data-ttu-id="65ed3-316">Gibt an, ob „Freunde suchen“ blockiert wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-316">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-317">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="65ed3-317">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="65ed3-318">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-318">Boolean</span></span>|<span data-ttu-id="65ed3-319">Gibt an, ob verhindert werden soll, dass der Benutzer Freunde im Game Center hat.</span><span class="sxs-lookup"><span data-stu-id="65ed3-319">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="65ed3-320">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="65ed3-320">gamingBlockMultiplayer</span></span>|<span data-ttu-id="65ed3-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="65ed3-321">Boolean</span></span>|<span data-ttu-id="65ed3-322">Gibt an, ob verhindert werden soll, dass der Benutzer Multiplayerspiele verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-322">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="65ed3-323">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-323">gameCenterBlocked</span></span>|<span data-ttu-id="65ed3-324">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-324">Boolean</span></span>|<span data-ttu-id="65ed3-325">Gibt an, ob verhindert werden soll, dass der Benutzer Game Center verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-325">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-326">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-326">hostPairingBlocked</span></span>|<span data-ttu-id="65ed3-327">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-327">Boolean</span></span>|<span data-ttu-id="65ed3-328">Gibt an, ob die Hostkopplung blockiert werden soll, um zu steuern, mit welchen Geräten ein iOS-Gerät gekoppelt werden kann,wenn sich das iOS-Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-328">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-329">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-329">iBooksStoreBlocked</span></span>|<span data-ttu-id="65ed3-330">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-330">Boolean</span></span>|<span data-ttu-id="65ed3-331">Gibt an, ob verhindert werden soll, dass der Benutzer den iBooks Store verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-331">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-332">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="65ed3-332">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="65ed3-333">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-333">Boolean</span></span>|<span data-ttu-id="65ed3-334">Gibt an, ob verhindert werden soll, dass der Benutzer Medien aus dem iBook Store herunterlädt, die als Erotik gekennzeichnet sind.</span><span class="sxs-lookup"><span data-stu-id="65ed3-334">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="65ed3-335">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="65ed3-335">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="65ed3-336">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-336">Boolean</span></span>|<span data-ttu-id="65ed3-337">Gibt an, ob der Benutzer von der Fortsetzung der Arbeit, die er auf dem iOS-Gerät gestartet hat, zu einem anderen iOS-oder macOS-Gerät blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-337">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="65ed3-338">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="65ed3-338">iCloudBlockBackup</span></span>|<span data-ttu-id="65ed3-339">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-339">Boolean</span></span>|<span data-ttu-id="65ed3-340">Gibt an, ob die iCloud-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-340">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="65ed3-341">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="65ed3-341">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="65ed3-342">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-342">Boolean</span></span>|<span data-ttu-id="65ed3-343">Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-343">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="65ed3-344">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="65ed3-344">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="65ed3-345">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-345">Boolean</span></span>|<span data-ttu-id="65ed3-346">Gibt an, ob die Cloudsynchronisierung für verwaltete Apps blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-346">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="65ed3-347">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="65ed3-347">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="65ed3-348">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-348">Boolean</span></span>|<span data-ttu-id="65ed3-349">Gibt an, ob die iCloud-Fotomediathek blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-349">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="65ed3-350">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="65ed3-350">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="65ed3-351">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-351">Boolean</span></span>|<span data-ttu-id="65ed3-352">Gibt an, ob die Fotostream-Synchronisierung in iCloud blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-352">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="65ed3-353">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="65ed3-353">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="65ed3-354">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-354">Boolean</span></span>|<span data-ttu-id="65ed3-355">Gibt an, ob die Fotofreigabe blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-355">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="65ed3-356">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="65ed3-356">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="65ed3-357">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-357">Boolean</span></span>|<span data-ttu-id="65ed3-358">Gibt an, ob Sicherungen in iCloud verschlüsselt sein müssen.</span><span class="sxs-lookup"><span data-stu-id="65ed3-358">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="65ed3-359">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="65ed3-359">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="65ed3-360">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-360">Boolean</span></span>|<span data-ttu-id="65ed3-361">Gibt an, ob verhindert werden soll, dass der Benutzer auf anstößige Inhalte in iTunes und im App Store zugreift. </span><span class="sxs-lookup"><span data-stu-id="65ed3-361">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="65ed3-362">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="65ed3-362">iTunesBlockMusicService</span></span>|<span data-ttu-id="65ed3-363">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-363">Boolean</span></span>|<span data-ttu-id="65ed3-364">Gibt an, ob der Music-Dienst blockiert und die Music-App in den klassischen Modus zurückgesetzt werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher und Mac OS 10.12 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-364">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="65ed3-365">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="65ed3-365">iTunesBlockRadio</span></span>|<span data-ttu-id="65ed3-366">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-366">Boolean</span></span>|<span data-ttu-id="65ed3-367">Gibt an, ob verhindert werden soll, dass der Benutzer iTunes Radio verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-367">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="65ed3-368">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="65ed3-368">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="65ed3-369">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-369">Boolean</span></span>|<span data-ttu-id="65ed3-370">Gibt an, ob die Autokorrektur der Tastatur blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-370">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="65ed3-371">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="65ed3-371">keyboardBlockDictation</span></span>|<span data-ttu-id="65ed3-372">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-372">Boolean</span></span>|<span data-ttu-id="65ed3-373">Gibt an, ob verhindert werden soll, dass der Benutzer die Diktatfunktion verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-373">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-374">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="65ed3-374">keyboardBlockPredictive</span></span>|<span data-ttu-id="65ed3-375">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-375">Boolean</span></span>|<span data-ttu-id="65ed3-376">Gibt an, ob Tastaturwortvorschläge blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-376">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="65ed3-377">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="65ed3-377">keyboardBlockShortcuts</span></span>|<span data-ttu-id="65ed3-378">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-378">Boolean</span></span>|<span data-ttu-id="65ed3-379">Gibt an, ob Tastenkombinationen blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-379">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="65ed3-380">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="65ed3-380">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="65ed3-381">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-381">Boolean</span></span>|<span data-ttu-id="65ed3-382">Gibt an, ob die Rechtschreibprüfung blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-382">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="65ed3-383">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="65ed3-383">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="65ed3-384">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-384">Boolean</span></span>|<span data-ttu-id="65ed3-385">Gibt an, ob Sprachunterstützung im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-385">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-386">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="65ed3-386">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="65ed3-387">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-387">Boolean</span></span>|<span data-ttu-id="65ed3-388">Gibt an, ob Zugriff auf die Einstellungen der Touch-Unterstützung im Kiosk-Modus gewährt werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-388">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-389">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="65ed3-389">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="65ed3-390">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-390">Boolean</span></span>|<span data-ttu-id="65ed3-391">Gibt an, ob die automatische Gerätesperre im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-391">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-392">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="65ed3-392">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="65ed3-393">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-393">Boolean</span></span>|<span data-ttu-id="65ed3-394">Gibt ab, ob der Zugriff auf die Farbinversionseinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-394">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-395">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="65ed3-395">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="65ed3-396">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-396">Boolean</span></span>|<span data-ttu-id="65ed3-397">Gibt ab, ob die Verwendung des Ruftonschalters im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-397">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-398">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="65ed3-398">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="65ed3-399">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-399">Boolean</span></span>|<span data-ttu-id="65ed3-400">Gibt ab, ob die Bildschirmdrehung im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-400">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-401">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="65ed3-401">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="65ed3-402">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-402">Boolean</span></span>|<span data-ttu-id="65ed3-403">Gibt ab, ob die Verwendung der Energiespartaste im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-403">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-404">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="65ed3-404">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="65ed3-405">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-405">Boolean</span></span>|<span data-ttu-id="65ed3-406">Gibt ab, ob die Verwendung des Touchscreens im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-406">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-407">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="65ed3-407">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="65ed3-408">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-408">Boolean</span></span>|<span data-ttu-id="65ed3-409">Gibt ab, ob der Zugriff auf die Einstellungen für Hintergrundkommentare im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-409">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-410">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="65ed3-410">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="65ed3-411">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-411">Boolean</span></span>|<span data-ttu-id="65ed3-412">Gibt ab, ob die Verwendung der Lautstärketasten im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-412">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-413">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="65ed3-413">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="65ed3-414">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-414">Boolean</span></span>|<span data-ttu-id="65ed3-415">Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="65ed3-415">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="65ed3-416">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="65ed3-416">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="65ed3-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="65ed3-417">Boolean</span></span>|<span data-ttu-id="65ed3-418">Gibt ab, ob der Zugriff auf die Zoomeinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-418">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-419">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="65ed3-419">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="65ed3-420">String</span><span class="sxs-lookup"><span data-stu-id="65ed3-420">String</span></span>|<span data-ttu-id="65ed3-421">URL im App Store zu der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-421">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="65ed3-422">Verwenden Sie diese, wenn „KioskModeManagedAppId“ nicht bekannt ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-422">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="65ed3-423">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="65ed3-423">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="65ed3-424">String</span><span class="sxs-lookup"><span data-stu-id="65ed3-424">String</span></span>|<span data-ttu-id="65ed3-425">ID für integrierte apps, die für den Kiosk-Modus verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="65ed3-425">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="65ed3-426">Wird verwendet, wenn "Kioskmodemanagedappid" und KioskModeAppStoreUrl nicht festgelegt sind.</span><span class="sxs-lookup"><span data-stu-id="65ed3-426">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="65ed3-427">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="65ed3-427">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="65ed3-428">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-428">Boolean</span></span>|<span data-ttu-id="65ed3-429">Gibt an, ob Touch-Unterstützung im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-429">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-430">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="65ed3-430">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="65ed3-431">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-431">Boolean</span></span>|<span data-ttu-id="65ed3-432">Gibt ab, ob die Farbinversion im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-432">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-433">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="65ed3-433">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="65ed3-434">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-434">Boolean</span></span>|<span data-ttu-id="65ed3-435">Gibt ab, ob Mono-Audio im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-435">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-436">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="65ed3-436">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="65ed3-437">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-437">Boolean</span></span>|<span data-ttu-id="65ed3-438">Gibt ab, ob Hintergrundkommentare im Kiosk-Modus erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="65ed3-438">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-439">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="65ed3-439">kioskModeRequireZoom</span></span>|<span data-ttu-id="65ed3-440">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-440">Boolean</span></span>|<span data-ttu-id="65ed3-441">Gibt ab, ob Zoom im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-441">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="65ed3-442">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="65ed3-442">kioskModeManagedAppId</span></span>|<span data-ttu-id="65ed3-443">String</span><span class="sxs-lookup"><span data-stu-id="65ed3-443">String</span></span>|<span data-ttu-id="65ed3-444">Verwaltete App-ID der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-444">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="65ed3-445">Wenn „KioskModeManagedAppId“ angegeben ist, wird „KioskModeAppStoreUrl“ ignoriert.</span><span class="sxs-lookup"><span data-stu-id="65ed3-445">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="65ed3-446">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="65ed3-446">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="65ed3-447">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-447">Boolean</span></span>|<span data-ttu-id="65ed3-448">Gibt an, ob verhindert werden soll, dass der Benutzer das Kontrollzentrum für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-448">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="65ed3-449">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="65ed3-449">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="65ed3-450">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-450">Boolean</span></span>|<span data-ttu-id="65ed3-451">Gibt an, ob verhindert werden soll, dass der Benutzer die Benachrichtigungsansicht auf dem Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-451">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="65ed3-452">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="65ed3-452">lockScreenBlockPassbook</span></span>|<span data-ttu-id="65ed3-453">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-453">Boolean</span></span>|<span data-ttu-id="65ed3-454">Gibt an, ob verhindert werden soll, dass der Benutzer Passbook verwendet, wenn das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-454">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="65ed3-455">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="65ed3-455">lockScreenBlockTodayView</span></span>|<span data-ttu-id="65ed3-456">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-456">Boolean</span></span>|<span data-ttu-id="65ed3-457">Gibt an, ob verhindert werden soll, dass der Benutzer die Ansicht „Heute“ für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-457">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="65ed3-458">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="65ed3-458">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="65ed3-459">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="65ed3-459">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="65ed3-460">Einstellungen für Medieninhalte für Australien</span><span class="sxs-lookup"><span data-stu-id="65ed3-460">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="65ed3-461">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="65ed3-461">mediaContentRatingCanada</span></span>|[<span data-ttu-id="65ed3-462">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="65ed3-462">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="65ed3-463">Einstellungen für Medieninhalte für Kanada</span><span class="sxs-lookup"><span data-stu-id="65ed3-463">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="65ed3-464">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="65ed3-464">mediaContentRatingFrance</span></span>|[<span data-ttu-id="65ed3-465">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="65ed3-465">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="65ed3-466">Einstellungen für Medieninhalte für Frankreich</span><span class="sxs-lookup"><span data-stu-id="65ed3-466">Media content rating settings for France</span></span>|
|<span data-ttu-id="65ed3-467">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="65ed3-467">mediaContentRatingGermany</span></span>|[<span data-ttu-id="65ed3-468">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="65ed3-468">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="65ed3-469">Einstellungen für Medieninhalte für Deutschland</span><span class="sxs-lookup"><span data-stu-id="65ed3-469">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="65ed3-470">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="65ed3-470">mediaContentRatingIreland</span></span>|[<span data-ttu-id="65ed3-471">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="65ed3-471">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="65ed3-472">Einstellungen für Medieninhalte für Irland</span><span class="sxs-lookup"><span data-stu-id="65ed3-472">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="65ed3-473">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="65ed3-473">mediaContentRatingJapan</span></span>|[<span data-ttu-id="65ed3-474">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="65ed3-474">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="65ed3-475">Einstellungen für Medieninhalte für Japan</span><span class="sxs-lookup"><span data-stu-id="65ed3-475">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="65ed3-476">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="65ed3-476">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="65ed3-477">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="65ed3-477">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="65ed3-478">Einstellungen für Medieninhalte für Neuseeland</span><span class="sxs-lookup"><span data-stu-id="65ed3-478">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="65ed3-479">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="65ed3-479">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="65ed3-480">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="65ed3-480">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="65ed3-481">Einstellungen für Medieninhalte für das Vereinigte Königreich</span><span class="sxs-lookup"><span data-stu-id="65ed3-481">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="65ed3-482">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="65ed3-482">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="65ed3-483">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="65ed3-483">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="65ed3-484">Einstellungen für Medieninhalte für die USA</span><span class="sxs-lookup"><span data-stu-id="65ed3-484">Media content rating settings for United States</span></span>|
|<span data-ttu-id="65ed3-485">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="65ed3-485">networkUsageRules</span></span>|<span data-ttu-id="65ed3-486">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="65ed3-486">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="65ed3-487">Liste verwalteter Apps und die Netzwerkregeln, die darauf angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="65ed3-487">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="65ed3-488">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="65ed3-488">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="65ed3-489">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="65ed3-489">mediaContentRatingApps</span></span>|[<span data-ttu-id="65ed3-490">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="65ed3-490">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="65ed3-491">Einstellungen für die Medieninhalts Bewertung für apps.</span><span class="sxs-lookup"><span data-stu-id="65ed3-491">Media content rating settings for Apps.</span></span> <span data-ttu-id="65ed3-492">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12` und `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="65ed3-492">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="65ed3-493">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-493">messagesBlocked</span></span>|<span data-ttu-id="65ed3-494">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-494">Boolean</span></span>|<span data-ttu-id="65ed3-495">Gibt an, ob verhindert werden soll, dass der Benutzer die Nachrichten-App auf dem überwachten Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-495">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="65ed3-496">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-496">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="65ed3-497">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-497">Boolean</span></span>|<span data-ttu-id="65ed3-498">Gibt an, ob die Änderung von Benachrichtigungseinstellungen zugelassen wird (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-498">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="65ed3-499">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="65ed3-499">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="65ed3-500">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-500">Boolean</span></span>|<span data-ttu-id="65ed3-501">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-501">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="65ed3-502">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-502">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="65ed3-503">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-503">Boolean</span></span>|<span data-ttu-id="65ed3-504">Blockiert das Ändern registrierter Touch ID-Fingerabdrücke im überwachten Modus.</span><span class="sxs-lookup"><span data-stu-id="65ed3-504">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-505">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-505">passcodeBlockModification</span></span>|<span data-ttu-id="65ed3-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="65ed3-506">Boolean</span></span>|<span data-ttu-id="65ed3-507">Gibt an, ob das Ändern der Kennung auf dem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-507">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="65ed3-508">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="65ed3-508">passcodeBlockSimple</span></span>|<span data-ttu-id="65ed3-509">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-509">Boolean</span></span>|<span data-ttu-id="65ed3-510">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="65ed3-510">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="65ed3-511">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="65ed3-511">passcodeExpirationDays</span></span>|<span data-ttu-id="65ed3-512">Int32</span><span class="sxs-lookup"><span data-stu-id="65ed3-512">Int32</span></span>|<span data-ttu-id="65ed3-513">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="65ed3-513">Number of days before the passcode expires.</span></span> <span data-ttu-id="65ed3-514">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="65ed3-514">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="65ed3-515">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="65ed3-515">passcodeMinimumLength</span></span>|<span data-ttu-id="65ed3-516">Int32</span><span class="sxs-lookup"><span data-stu-id="65ed3-516">Int32</span></span>|<span data-ttu-id="65ed3-517">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="65ed3-517">Minimum length of passcode.</span></span> <span data-ttu-id="65ed3-518">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="65ed3-518">Valid values 4 to 14</span></span>|
|<span data-ttu-id="65ed3-519">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="65ed3-519">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="65ed3-520">Int32</span><span class="sxs-lookup"><span data-stu-id="65ed3-520">Int32</span></span>|<span data-ttu-id="65ed3-521">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-521">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="65ed3-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="65ed3-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="65ed3-523">Int32</span><span class="sxs-lookup"><span data-stu-id="65ed3-523">Int32</span></span>|<span data-ttu-id="65ed3-524">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="65ed3-524">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="65ed3-525">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="65ed3-525">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="65ed3-526">Int32</span><span class="sxs-lookup"><span data-stu-id="65ed3-526">Int32</span></span>|<span data-ttu-id="65ed3-527">Anzahl von Zeichensätzen, die eine Kennung enthalten muss</span><span class="sxs-lookup"><span data-stu-id="65ed3-527">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="65ed3-528">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="65ed3-528">Valid values 0 to 4</span></span>|
|<span data-ttu-id="65ed3-529">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="65ed3-529">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="65ed3-530">Int32</span><span class="sxs-lookup"><span data-stu-id="65ed3-530">Int32</span></span>|<span data-ttu-id="65ed3-531">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="65ed3-531">Number of previous passcodes to block.</span></span> <span data-ttu-id="65ed3-532">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="65ed3-532">Valid values 1 to 24</span></span>|
|<span data-ttu-id="65ed3-533">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="65ed3-533">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="65ed3-534">Int32</span><span class="sxs-lookup"><span data-stu-id="65ed3-534">Int32</span></span>|<span data-ttu-id="65ed3-535">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung des Geräts durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="65ed3-535">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="65ed3-536">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="65ed3-536">Valid values 4 to 11</span></span>|
|<span data-ttu-id="65ed3-537">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="65ed3-537">passcodeRequiredType</span></span>|[<span data-ttu-id="65ed3-538">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="65ed3-538">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="65ed3-539">Geforderter Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="65ed3-539">Type of passcode that is required.</span></span> <span data-ttu-id="65ed3-540">Mögliche Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="65ed3-540">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="65ed3-541">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="65ed3-541">passcodeRequired</span></span>|<span data-ttu-id="65ed3-542">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-542">Boolean</span></span>|<span data-ttu-id="65ed3-543">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-543">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="65ed3-544">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-544">podcastsBlocked</span></span>|<span data-ttu-id="65ed3-545">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-545">Boolean</span></span>|<span data-ttu-id="65ed3-546">Gibt an, ob verhindert werden soll, dass der Benutzer Podcasts auf dem überwachten Gerät verwendet (iOS 8.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-546">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="65ed3-547">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="65ed3-547">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="65ed3-548">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-548">Boolean</span></span>|<span data-ttu-id="65ed3-549">Gibt an, ob die Ansage zum Einrichten von benachbarten Geräten mit einem überwachten Gerät aktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-549">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="65ed3-550">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="65ed3-550">safariBlockAutofill</span></span>|<span data-ttu-id="65ed3-551">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-551">Boolean</span></span>|<span data-ttu-id="65ed3-552">Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-552">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="65ed3-553">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="65ed3-553">safariBlockJavaScript</span></span>|<span data-ttu-id="65ed3-554">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-554">Boolean</span></span>|<span data-ttu-id="65ed3-555">Gibt an, ob JavaScript in Safari blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-555">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="65ed3-556">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="65ed3-556">safariBlockPopups</span></span>|<span data-ttu-id="65ed3-557">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-557">Boolean</span></span>|<span data-ttu-id="65ed3-558">Gibt an, ob Popups in Safari blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="65ed3-558">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="65ed3-559">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-559">safariBlocked</span></span>|<span data-ttu-id="65ed3-560">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-560">Boolean</span></span>|<span data-ttu-id="65ed3-561">Gibt an, ob verhindert werden soll, dass der Benutzer Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-561">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="65ed3-562">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="65ed3-562">safariCookieSettings</span></span>|[<span data-ttu-id="65ed3-563">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="65ed3-563">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="65ed3-564">Cokkieeinstellungen für Safari.</span><span class="sxs-lookup"><span data-stu-id="65ed3-564">Cookie settings for Safari.</span></span> <span data-ttu-id="65ed3-565">Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="65ed3-565">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="65ed3-566">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="65ed3-566">safariManagedDomains</span></span>|<span data-ttu-id="65ed3-567">String collection</span><span class="sxs-lookup"><span data-stu-id="65ed3-567">String collection</span></span>|<span data-ttu-id="65ed3-568">URLs, die mit den hier aufgeführten Mustern übereinstimmen, werden als verwaltet betrachtet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-568">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="65ed3-569">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="65ed3-569">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="65ed3-570">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="65ed3-570">String collection</span></span>|<span data-ttu-id="65ed3-571">Benutzer können Kennwörter in Safari nur von URLs speichern, die mit den hier aufgeführten Mustern übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="65ed3-571">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="65ed3-572">Gilt für Geräte im überwachten Modus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-572">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="65ed3-573">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="65ed3-573">safariRequireFraudWarning</span></span>|<span data-ttu-id="65ed3-574">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-574">Boolean</span></span>|<span data-ttu-id="65ed3-575">Gibt an, ob eine Betrugswarnung in Safari erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-575">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="65ed3-576">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-576">screenCaptureBlocked</span></span>|<span data-ttu-id="65ed3-577">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-577">Boolean</span></span>|<span data-ttu-id="65ed3-578">Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.</span><span class="sxs-lookup"><span data-stu-id="65ed3-578">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="65ed3-579">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-579">siriBlocked</span></span>|<span data-ttu-id="65ed3-580">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-580">Boolean</span></span>|<span data-ttu-id="65ed3-581">Gibt an, ob verhindert werden soll, dass der Benutzer Siri verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-581">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="65ed3-582">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-582">siriBlockedWhenLocked</span></span>|<span data-ttu-id="65ed3-583">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-583">Boolean</span></span>|<span data-ttu-id="65ed3-584">Gibt an, ob verhindert werden soll, dass der Benutzer Siri bei Sperrung verwendet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-584">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="65ed3-585">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="65ed3-585">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="65ed3-586">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-586">Boolean</span></span>|<span data-ttu-id="65ed3-587">Gibt an, ob Siri bei Verwendung auf einem überwachten Gerät davon abgehalten werden soll, benutzergenerierte Inhalte abzufragen.</span><span class="sxs-lookup"><span data-stu-id="65ed3-587">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="65ed3-588">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="65ed3-588">siriRequireProfanityFilter</span></span>|<span data-ttu-id="65ed3-589">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-589">Boolean</span></span>|<span data-ttu-id="65ed3-590">Gibt an, ob verhindert werden soll, dass Siri anstößige Ausdrücke auf dem überwachten Gerät diktiert oder spricht.</span><span class="sxs-lookup"><span data-stu-id="65ed3-590">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="65ed3-591">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="65ed3-591">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="65ed3-592">Int32</span><span class="sxs-lookup"><span data-stu-id="65ed3-592">Int32</span></span>|<span data-ttu-id="65ed3-593">Legt fest, wie viele Tage ein Software Update für ein überwachte Gerät delyed wird.</span><span class="sxs-lookup"><span data-stu-id="65ed3-593">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="65ed3-594">Gültige Werte: 0 bis 90.</span><span class="sxs-lookup"><span data-stu-id="65ed3-594">Valid values 0 to 90</span></span>|
|<span data-ttu-id="65ed3-595">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="65ed3-595">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="65ed3-596">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-596">Boolean</span></span>|<span data-ttu-id="65ed3-597">Gibt an, ob die Benutzersicht barkeit von Softwareupdates verzögert werden soll, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-597">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-598">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="65ed3-598">spotlightBlockInternetResults</span></span>|<span data-ttu-id="65ed3-599">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-599">Boolean</span></span>|<span data-ttu-id="65ed3-600">Gibt an, ob verhindert werden soll, dass die Spotlight-Suche Internetergebnisse auf dem überwachten Gerät zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="65ed3-600">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="65ed3-601">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-601">voiceDialingBlocked</span></span>|<span data-ttu-id="65ed3-602">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-602">Boolean</span></span>|<span data-ttu-id="65ed3-603">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-603">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="65ed3-604">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="65ed3-604">wallpaperBlockModification</span></span>|<span data-ttu-id="65ed3-605">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-605">Boolean</span></span>|<span data-ttu-id="65ed3-606">Gibt an, ob das Ändern des Hintergrunds auf einem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-606">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="65ed3-607">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="65ed3-607">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="65ed3-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="65ed3-608">Boolean</span></span>|<span data-ttu-id="65ed3-609">Gibt an, ob erzwungen werden soll, dass das Gerät nur WLAN-Netzwerke aus Konfigurationsprofilen verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="65ed3-609">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="65ed3-610">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="65ed3-610">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="65ed3-611">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-611">Boolean</span></span>|<span data-ttu-id="65ed3-612">Gibt an, ob ein Teilnehmer, der über das Klassenzimmer in einem nicht verwalteten Kurs angemeldet ist, beim Versuch, den Kurs zu verlassen (iOS 11,3 und höher) die Berechtigung des Lehrers anfordert.</span><span class="sxs-lookup"><span data-stu-id="65ed3-612">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="65ed3-613">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="65ed3-613">keychainBlockCloudSync</span></span>|<span data-ttu-id="65ed3-614">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-614">Boolean</span></span>|<span data-ttu-id="65ed3-615">Gibt an, ob die iCloud-Schlüsselbund Synchronisierung blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-615">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="65ed3-616">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="65ed3-616">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="65ed3-617">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-617">Boolean</span></span>|<span data-ttu-id="65ed3-618">Gibt an, ob over-the-Air-PKI-Updates blockiert sind.</span><span class="sxs-lookup"><span data-stu-id="65ed3-618">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="65ed3-619">Wenn Sie diese Einschränkung auf false festlegen, werden CRL-und OCSP-Prüfungen nicht deaktiviert (iOS 7,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-619">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="65ed3-620">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="65ed3-620">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="65ed3-621">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-621">Boolean</span></span>|<span data-ttu-id="65ed3-622">Gibt an, ob die AD-Verfolgung begrenzt ist. (iOS 7,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-622">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="65ed3-623">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="65ed3-623">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="65ed3-624">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-624">Boolean</span></span>|<span data-ttu-id="65ed3-625">Gibt an, ob Enterprise Book Back up gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-625">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="65ed3-626">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="65ed3-626">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="65ed3-627">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-627">Boolean</span></span>|<span data-ttu-id="65ed3-628">Gibt an, ob die Synchronisierung von Enterprise Book Notes und Highlights blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-628">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="65ed3-629">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-629">airPrintBlocked</span></span>|<span data-ttu-id="65ed3-630">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-630">Boolean</span></span>|<span data-ttu-id="65ed3-631">Gibt an, ob der druckDruck blockiert ist (iOS 11,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-631">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="65ed3-632">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="65ed3-632">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="65ed3-633">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-633">Boolean</span></span>|<span data-ttu-id="65ed3-634">Gibt an, ob die Schlüsselbund Speicherung von Benutzername und Kennwort für druckdruck blockiert ist (iOS 11,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-634">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="65ed3-635">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="65ed3-635">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="65ed3-636">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-636">Boolean</span></span>|<span data-ttu-id="65ed3-637">Gibt an, ob vertrauenswürdige Zertifikate für die TLS-Druckkommunikation erforderlich sind (iOS 11,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-637">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="65ed3-638">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="65ed3-638">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="65ed3-639">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-639">Boolean</span></span>|<span data-ttu-id="65ed3-640">Gibt an, ob die iBeacon-Erkennung von Druckern blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="65ed3-640">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="65ed3-641">Dadurch wird verhindert, dass gefälschte Bluetooth-Baken für den Netzwerkdatenverkehr aus dem Phishing entfernt werden (iOS 11,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-641">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="65ed3-642">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="65ed3-642">blockSystemAppRemoval</span></span>|<span data-ttu-id="65ed3-643">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-643">Boolean</span></span>|<span data-ttu-id="65ed3-644">Gibt an, ob das Entfernen von System-apps vom Gerät auf einem überwachten Gerät (iOS 11,0 und höher) blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-644">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="65ed3-645">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="65ed3-645">vpnBlockCreation</span></span>|<span data-ttu-id="65ed3-646">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-646">Boolean</span></span>|<span data-ttu-id="65ed3-647">Gibt an, ob die Erstellung von VPN-Konfigurationen blockiert ist (iOS 11,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-647">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="65ed3-648">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-648">appRemovalBlocked</span></span>|<span data-ttu-id="65ed3-649">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-649">Boolean</span></span>|<span data-ttu-id="65ed3-650">Gibt an, ob das Entfernen von apps zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-650">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="65ed3-651">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="65ed3-651">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="65ed3-652">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-652">Boolean</span></span>|<span data-ttu-id="65ed3-653">Gibt an, ob das Herstellen einer Verbindung mit USB-Zubehör während der Sperrung des Geräts zulässig ist (iOS 11.4.1 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-653">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="65ed3-654">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="65ed3-654">passwordBlockAutoFill</span></span>|<span data-ttu-id="65ed3-655">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-655">Boolean</span></span>|<span data-ttu-id="65ed3-656">Gibt an, ob das Feature AutoFill passwords (iOS 12,0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="65ed3-656">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="65ed3-657">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="65ed3-657">passwordBlockProximityRequests</span></span>|<span data-ttu-id="65ed3-658">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-658">Boolean</span></span>|<span data-ttu-id="65ed3-659">Gibt an, ob das Anfordern von Kennwörtern von benachbarten Geräten (iOS 12,0 und höher) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-659">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="65ed3-660">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="65ed3-660">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="65ed3-661">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-661">Boolean</span></span>|<span data-ttu-id="65ed3-662">Gibt an, ob das Freigeben von Kennwörtern für die Kennwörter von iOS 12,0 und höher blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="65ed3-662">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="65ed3-663">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="65ed3-663">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="65ed3-664">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-664">Boolean</span></span>|<span data-ttu-id="65ed3-665">Gibt an, ob die Funktion für Datum und Uhrzeit "automatisch festlegen" aktiviert ist und nicht vom Benutzer deaktiviert werden kann (iOS 12,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-665">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="65ed3-666">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="65ed3-666">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="65ed3-667">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-667">Boolean</span></span>|<span data-ttu-id="65ed3-668">Gibt an, ob verwaltete Apps Kontakte in nicht verwaltete Kontakte-Konten schreiben können (iOS 12,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-668">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="65ed3-669">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="65ed3-669">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="65ed3-670">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="65ed3-670">Boolean</span></span>|<span data-ttu-id="65ed3-671">Gibt an, ob nicht verwaltete Apps aus Konten für verwaltete Kontakte lesen können (iOS 12,0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="65ed3-671">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="65ed3-672">Antwort</span><span class="sxs-lookup"><span data-stu-id="65ed3-672">Response</span></span>
<span data-ttu-id="65ed3-673">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="65ed3-673">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65ed3-674">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65ed3-674">Example</span></span>

### <a name="request"></a><span data-ttu-id="65ed3-675">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65ed3-675">Request</span></span>
<span data-ttu-id="65ed3-676">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65ed3-676">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 9105

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true
}
```

### <a name="response"></a><span data-ttu-id="65ed3-677">Antwort</span><span class="sxs-lookup"><span data-stu-id="65ed3-677">Response</span></span>
<span data-ttu-id="65ed3-p133">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65ed3-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9277

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true
}
```




