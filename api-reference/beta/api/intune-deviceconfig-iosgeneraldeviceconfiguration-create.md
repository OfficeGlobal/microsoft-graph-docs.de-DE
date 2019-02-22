---
title: iosGeneralDeviceConfiguration erstellen
description: Erstellen Sie ein neues iosGeneralDeviceConfiguration-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5690a63548020f73e0328468f0f37340d00bbf1b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148146"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="d61fe-103">iosGeneralDeviceConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="d61fe-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="d61fe-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d61fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d61fe-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d61fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d61fe-106">Erstellen Sie ein neues [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d61fe-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d61fe-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d61fe-107">Prerequisites</span></span>
<span data-ttu-id="d61fe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d61fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d61fe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d61fe-110">Permission type</span></span>|<span data-ttu-id="d61fe-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d61fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d61fe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d61fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d61fe-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d61fe-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d61fe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d61fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d61fe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d61fe-115">Not supported.</span></span>|
|<span data-ttu-id="d61fe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d61fe-116">Application</span></span>|<span data-ttu-id="d61fe-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d61fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d61fe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d61fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d61fe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d61fe-119">Request headers</span></span>
|<span data-ttu-id="d61fe-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d61fe-120">Header</span></span>|<span data-ttu-id="d61fe-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d61fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d61fe-122">Authorization</span></span>|<span data-ttu-id="d61fe-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d61fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d61fe-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d61fe-124">Accept</span></span>|<span data-ttu-id="d61fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d61fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d61fe-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d61fe-126">Request body</span></span>
<span data-ttu-id="d61fe-127">Geben Sie im Anforderungstext eine JSON-Darstellung des iosGeneralDeviceConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d61fe-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="d61fe-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs iosGeneralDeviceConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="d61fe-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="d61fe-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d61fe-129">Property</span></span>|<span data-ttu-id="d61fe-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d61fe-130">Type</span></span>|<span data-ttu-id="d61fe-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d61fe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d61fe-132">id</span><span class="sxs-lookup"><span data-stu-id="d61fe-132">id</span></span>|<span data-ttu-id="d61fe-133">string</span><span class="sxs-lookup"><span data-stu-id="d61fe-133">String</span></span>|<span data-ttu-id="d61fe-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d61fe-134">Key of the entity.</span></span> <span data-ttu-id="d61fe-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d61fe-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d61fe-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d61fe-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d61fe-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d61fe-137">DateTimeOffset</span></span>|<span data-ttu-id="d61fe-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d61fe-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d61fe-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d61fe-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d61fe-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="d61fe-140">roleScopeTagIds</span></span>|<span data-ttu-id="d61fe-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d61fe-141">String collection</span></span>|<span data-ttu-id="d61fe-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="d61fe-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d61fe-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d61fe-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d61fe-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d61fe-144">supportsScopeTags</span></span>|<span data-ttu-id="d61fe-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-145">Boolean</span></span>|<span data-ttu-id="d61fe-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d61fe-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d61fe-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="d61fe-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d61fe-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d61fe-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d61fe-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d61fe-149">This property is read-only.</span></span> <span data-ttu-id="d61fe-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d61fe-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d61fe-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d61fe-151">createdDateTime</span></span>|<span data-ttu-id="d61fe-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d61fe-152">DateTimeOffset</span></span>|<span data-ttu-id="d61fe-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d61fe-153">DateTime the object was created.</span></span> <span data-ttu-id="d61fe-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d61fe-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d61fe-155">description</span><span class="sxs-lookup"><span data-stu-id="d61fe-155">description</span></span>|<span data-ttu-id="d61fe-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d61fe-156">String</span></span>|<span data-ttu-id="d61fe-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d61fe-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d61fe-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d61fe-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d61fe-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d61fe-159">displayName</span></span>|<span data-ttu-id="d61fe-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d61fe-160">String</span></span>|<span data-ttu-id="d61fe-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d61fe-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d61fe-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d61fe-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d61fe-163">Version</span><span class="sxs-lookup"><span data-stu-id="d61fe-163">version</span></span>|<span data-ttu-id="d61fe-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d61fe-164">Int32</span></span>|<span data-ttu-id="d61fe-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d61fe-165">Version of the device configuration.</span></span> <span data-ttu-id="d61fe-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d61fe-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d61fe-167">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-167">accountBlockModification</span></span>|<span data-ttu-id="d61fe-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-168">Boolean</span></span>|<span data-ttu-id="d61fe-169">Gibt an, ob die Kontoänderung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-169">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-170">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="d61fe-170">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="d61fe-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-171">Boolean</span></span>|<span data-ttu-id="d61fe-172">Gibt an, ob die Aktivierungssperre zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-172">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="d61fe-173">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-173">airDropBlocked</span></span>|<span data-ttu-id="d61fe-174">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-174">Boolean</span></span>|<span data-ttu-id="d61fe-175">Gibt an, ob AirDrop zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-175">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-176">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="d61fe-176">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="d61fe-177">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-177">Boolean</span></span>|<span data-ttu-id="d61fe-178">Gibt an, ob AirDrop als nicht verwaltetes Drop-Ziel (iOS 9.0 oder höher) betrachtet werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-178">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d61fe-179">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="d61fe-179">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="d61fe-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-180">Boolean</span></span>|<span data-ttu-id="d61fe-181">Gibt an, ob erzwungen werden soll, dass alle Geräte, die AirPlay-Anforderungen von diesem Gerät erhalten, ein Kopplungskennwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="d61fe-181">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="d61fe-182">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="d61fe-182">appleWatchBlockPairing</span></span>|<span data-ttu-id="d61fe-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-183">Boolean</span></span>|<span data-ttu-id="d61fe-184">Gibt an, ob eine Apple Watch-Kopplung zulässig ist, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-184">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d61fe-185">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="d61fe-185">appleWatchForceWristDetection</span></span>|<span data-ttu-id="d61fe-186">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-186">Boolean</span></span>|<span data-ttu-id="d61fe-187">Gibt an, ob erzwungen werden soll, dass eine gekoppelte Apple Watch die Handgelenkerkennung (iOS 8.2 und höher) verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-187">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="d61fe-188">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-188">appleNewsBlocked</span></span>|<span data-ttu-id="d61fe-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-189">Boolean</span></span>|<span data-ttu-id="d61fe-190">Gibt an, ob verhindert werden soll, dass der Benutzer News verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-190">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d61fe-191">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="d61fe-191">appsSingleAppModeList</span></span>|<span data-ttu-id="d61fe-192">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d61fe-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d61fe-193">Ruft die Liste von iOS-Apps ab, die autonom in den Einzelanwendungsmodus wechseln können, ab oder legt diese fest.</span><span class="sxs-lookup"><span data-stu-id="d61fe-193">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="d61fe-194">Nur überwacht.</span><span class="sxs-lookup"><span data-stu-id="d61fe-194">Supervised only.</span></span> <span data-ttu-id="d61fe-195">iOS 7.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="d61fe-195">iOS 7.0 and later.</span></span> <span data-ttu-id="d61fe-196">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d61fe-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d61fe-197">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="d61fe-197">appsVisibilityList</span></span>|<span data-ttu-id="d61fe-198">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d61fe-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d61fe-199">Liste von Apps in der Sichtbarkeitsliste (entweder eine Liste sichtbarer/startbarer Apps oder eine Liste ausgeblendeter/nicht startbarer Apps, gesteuert von AppsVisibilityListType) (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-199">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="d61fe-200">Diese Sammlung darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d61fe-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d61fe-201">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="d61fe-201">appsVisibilityListType</span></span>|[<span data-ttu-id="d61fe-202">appListType</span><span class="sxs-lookup"><span data-stu-id="d61fe-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d61fe-203">Typ der in „AppsVisibilityList“ enthaltenen Liste.</span><span class="sxs-lookup"><span data-stu-id="d61fe-203">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="d61fe-204">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d61fe-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d61fe-205">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="d61fe-205">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="d61fe-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-206">Boolean</span></span>|<span data-ttu-id="d61fe-207">Gibt an, ob das automatische Herunterladen von Apps blockiert werden soll, die auf anderen Geräten gekauft wurden, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-207">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d61fe-208">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-208">appStoreBlocked</span></span>|<span data-ttu-id="d61fe-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-209">Boolean</span></span>|<span data-ttu-id="d61fe-210">Gibt an, ob verhindert werden soll, dass der Benutzer den App Store verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-210">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="d61fe-211">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="d61fe-211">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="d61fe-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-212">Boolean</span></span>|<span data-ttu-id="d61fe-213">Gibt an, ob verhindert werden soll, dass der Benutzer In-App-Käufe tätigt.</span><span class="sxs-lookup"><span data-stu-id="d61fe-213">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="d61fe-214">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d61fe-214">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="d61fe-215">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-215">Boolean</span></span>|<span data-ttu-id="d61fe-216">Gibt an, ob die App Store-App blockiert werden soll, ohne die Installation über Host-Apps einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="d61fe-216">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="d61fe-217">Gilt nur für den überwachten Modus (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-217">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d61fe-218">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="d61fe-218">appStoreRequirePassword</span></span>|<span data-ttu-id="d61fe-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-219">Boolean</span></span>|<span data-ttu-id="d61fe-220">Gibt an, ob bei Verwendung des App Stores ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-220">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="d61fe-221">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="d61fe-221">autoFillForceAuthentication</span></span>|<span data-ttu-id="d61fe-222">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-222">Boolean</span></span>|<span data-ttu-id="d61fe-223">Gibt an, ob die Benutzerauthentifizierung erzwungen werden soll, bevor Kennwörter und Kreditkarteninformationen in Safari und anderen apps auf überwachten Geräten automatisch gefüllt werden.</span><span class="sxs-lookup"><span data-stu-id="d61fe-223">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="d61fe-224">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-224">bluetoothBlockModification</span></span>|<span data-ttu-id="d61fe-225">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-225">Boolean</span></span>|<span data-ttu-id="d61fe-226">Gibt an, ob das Ändern von Bluetooth-Einstellungen zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 10.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-226">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="d61fe-227">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-227">cameraBlocked</span></span>|<span data-ttu-id="d61fe-228">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-228">Boolean</span></span>|<span data-ttu-id="d61fe-229">Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.</span><span class="sxs-lookup"><span data-stu-id="d61fe-229">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="d61fe-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="d61fe-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="d61fe-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-231">Boolean</span></span>|<span data-ttu-id="d61fe-232">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="d61fe-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="d61fe-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="d61fe-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-234">Boolean</span></span>|<span data-ttu-id="d61fe-235">Gibt an, ob das globales Abrufen im Hintergrund beim Roaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-235">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="d61fe-236">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-236">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="d61fe-237">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-237">Boolean</span></span>|<span data-ttu-id="d61fe-238">Gibt an, ob Änderungen an den Mobil-App-Daten zulässig sind, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-238">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-239">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="d61fe-239">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="d61fe-240">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-240">Boolean</span></span>|<span data-ttu-id="d61fe-241">Gibt an, ob der privater Hotspot blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-241">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="d61fe-242">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-242">cellularBlockPlanModification</span></span>|<span data-ttu-id="d61fe-243">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-243">Boolean</span></span>|<span data-ttu-id="d61fe-244">Gibt an, ob Benutzer die Einstellungen des Mobil Funk Plans auf einem überwachten Gerät ändern dürfen.</span><span class="sxs-lookup"><span data-stu-id="d61fe-244">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="d61fe-245">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="d61fe-245">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="d61fe-246">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-246">Boolean</span></span>|<span data-ttu-id="d61fe-247">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-247">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="d61fe-248">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="d61fe-248">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="d61fe-249">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-249">Boolean</span></span>|<span data-ttu-id="d61fe-250">Gibt an, ob nicht vertrauenswürdige TLS-Zertifikate blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d61fe-250">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="d61fe-251">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d61fe-251">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="d61fe-252">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-252">Boolean</span></span>|<span data-ttu-id="d61fe-253">Gibt an, ob die Remotebildschirmüberwachung über die Classroom-App zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-253">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d61fe-254">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d61fe-254">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="d61fe-255">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-255">Boolean</span></span>|<span data-ttu-id="d61fe-256">Gibt an, ob dem Lehrer eines verwalteten Kurses in der Classroom-App automatisch die Berechtigung erteilt werden soll, den Bildschirm eines Kursteilnehmers ohne Aufforderung anzuzeigen, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-256">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-257">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="d61fe-257">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="d61fe-258">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-258">Boolean</span></span>|<span data-ttu-id="d61fe-259">Gibt an, ob die Berechtigung für die Anforderungen des Lehrers automatisch erteilt werden soll, ohne dass der Kursteilnehmer dazu aufgefordert wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-259">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-260">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="d61fe-260">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="d61fe-261">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-261">Boolean</span></span>|<span data-ttu-id="d61fe-262">Gibt an, ob die Lehrerin Apps oder das Gerät Sperren soll, ohne dass der Kursteilnehmer dazu aufgefordert wird.</span><span class="sxs-lookup"><span data-stu-id="d61fe-262">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="d61fe-263">Nur überwacht.</span><span class="sxs-lookup"><span data-stu-id="d61fe-263">Supervised only.</span></span>|
|<span data-ttu-id="d61fe-264">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="d61fe-264">compliantAppsList</span></span>|<span data-ttu-id="d61fe-265">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d61fe-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d61fe-266">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="d61fe-266">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="d61fe-267">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d61fe-267">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d61fe-268">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="d61fe-268">compliantAppListType</span></span>|[<span data-ttu-id="d61fe-269">appListType</span><span class="sxs-lookup"><span data-stu-id="d61fe-269">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d61fe-270">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="d61fe-270">List that is in the AppComplianceList.</span></span> <span data-ttu-id="d61fe-271">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d61fe-271">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d61fe-272">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="d61fe-272">configurationProfileBlockChanges</span></span>|<span data-ttu-id="d61fe-273">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-273">Boolean</span></span>|<span data-ttu-id="d61fe-274">Gibt an, ob verhindert werden soll, dass der Benutzer Konfigurationsprofile und Zertifikate interaktiv installiert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-274">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-275">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-275">definitionLookupBlocked</span></span>|<span data-ttu-id="d61fe-276">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-276">Boolean</span></span>|<span data-ttu-id="d61fe-277">Gibt an, ob die Definitionssuche zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-277">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="d61fe-278">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="d61fe-278">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="d61fe-279">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-279">Boolean</span></span>|<span data-ttu-id="d61fe-280">Gibt an, ob erlaubt werden soll, dass der Benutzer Einschränkungen in den Geräteeinstellungen aktiviert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-280">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-281">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="d61fe-281">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="d61fe-282">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-282">Boolean</span></span>|<span data-ttu-id="d61fe-283">Gibt an, ob die Verwendung der Option zum Löschen aller Inhalte und Einstellungen auf dem Gerät zugelassen werden soll, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-283">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-284">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-284">deviceBlockNameModification</span></span>|<span data-ttu-id="d61fe-285">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-285">Boolean</span></span>|<span data-ttu-id="d61fe-286">Gibt an, ob das Ändern des Gerätenamens zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-286">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d61fe-287">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="d61fe-287">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="d61fe-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61fe-288">Boolean</span></span>|<span data-ttu-id="d61fe-289">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-289">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="d61fe-290">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-290">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="d61fe-291">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-291">Boolean</span></span>|<span data-ttu-id="d61fe-292">Gibt an, ob das Ändern der Einstellungen für die Diagnoseübermittlung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3.2 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-292">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="d61fe-293">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="d61fe-293">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="d61fe-294">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-294">Boolean</span></span>|<span data-ttu-id="d61fe-295">Gibt an, ob verhindert werden soll, dass der Benutzer verwaltete Dokumente in nicht verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="d61fe-295">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="d61fe-296">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="d61fe-296">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="d61fe-297">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-297">Boolean</span></span>|<span data-ttu-id="d61fe-298">Gibt an, ob verhindert werden soll, dass der Benutzer nicht verwaltete Dokumente in verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="d61fe-298">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="d61fe-299">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="d61fe-299">emailInDomainSuffixes</span></span>|<span data-ttu-id="d61fe-300">String collection</span><span class="sxs-lookup"><span data-stu-id="d61fe-300">String collection</span></span>|<span data-ttu-id="d61fe-301">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="d61fe-301">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="d61fe-302">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="d61fe-302">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="d61fe-303">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-303">Boolean</span></span>|<span data-ttu-id="d61fe-304">Gibt an, ob verhindert werden soll, dass der Benutzer einer Unternehmens-App vertraut.</span><span class="sxs-lookup"><span data-stu-id="d61fe-304">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="d61fe-305">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-305">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="d61fe-306">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-306">Boolean</span></span>|<span data-ttu-id="d61fe-307">Gibt an, ob verhindert werden soll, dass der Benutzer die Vertrauensstellungseinstellungen der Unternehmens-App ändert.</span><span class="sxs-lookup"><span data-stu-id="d61fe-307">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="d61fe-308">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-308">esimBlockModification</span></span>|<span data-ttu-id="d61fe-309">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-309">Boolean</span></span>|<span data-ttu-id="d61fe-310">Gibt an, ob das Hinzufügen oder Entfernen von Zellen Plänen auf dem eSIM eines überwachten Geräts zugelassen werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-310">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="d61fe-311">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-311">faceTimeBlocked</span></span>|<span data-ttu-id="d61fe-312">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-312">Boolean</span></span>|<span data-ttu-id="d61fe-313">Gibt an, ob verhindert werden soll, dass der Benutzer FaceTime verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-313">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="d61fe-314">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-314">findMyFriendsBlocked</span></span>|<span data-ttu-id="d61fe-315">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-315">Boolean</span></span>|<span data-ttu-id="d61fe-316">Gibt an, ob „Freunde suchen“ blockiert wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-316">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-317">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="d61fe-317">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="d61fe-318">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-318">Boolean</span></span>|<span data-ttu-id="d61fe-319">Gibt an, ob verhindert werden soll, dass der Benutzer Freunde im Game Center hat.</span><span class="sxs-lookup"><span data-stu-id="d61fe-319">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="d61fe-320">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="d61fe-320">gamingBlockMultiplayer</span></span>|<span data-ttu-id="d61fe-321">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-321">Boolean</span></span>|<span data-ttu-id="d61fe-322">Gibt an, ob verhindert werden soll, dass der Benutzer Multiplayerspiele verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-322">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="d61fe-323">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-323">gameCenterBlocked</span></span>|<span data-ttu-id="d61fe-324">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-324">Boolean</span></span>|<span data-ttu-id="d61fe-325">Gibt an, ob verhindert werden soll, dass der Benutzer Game Center verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-325">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-326">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-326">hostPairingBlocked</span></span>|<span data-ttu-id="d61fe-327">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-327">Boolean</span></span>|<span data-ttu-id="d61fe-328">Gibt an, ob die Hostkopplung blockiert werden soll, um zu steuern, mit welchen Geräten ein iOS-Gerät gekoppelt werden kann,wenn sich das iOS-Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-328">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-329">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-329">iBooksStoreBlocked</span></span>|<span data-ttu-id="d61fe-330">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-330">Boolean</span></span>|<span data-ttu-id="d61fe-331">Gibt an, ob verhindert werden soll, dass der Benutzer den iBooks Store verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-331">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-332">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="d61fe-332">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="d61fe-333">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-333">Boolean</span></span>|<span data-ttu-id="d61fe-334">Gibt an, ob verhindert werden soll, dass der Benutzer Medien aus dem iBook Store herunterlädt, die als Erotik gekennzeichnet sind.</span><span class="sxs-lookup"><span data-stu-id="d61fe-334">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="d61fe-335">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="d61fe-335">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="d61fe-336">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-336">Boolean</span></span>|<span data-ttu-id="d61fe-337">Gibt an, ob verhindert werden soll, dass der Benutzer eine Aufgabe, die er auf dem iOS-Gerät begonnen hat, auf einem anderen iOS- oder macOS-Gerät fortsetzt.</span><span class="sxs-lookup"><span data-stu-id="d61fe-337">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="d61fe-338">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="d61fe-338">iCloudBlockBackup</span></span>|<span data-ttu-id="d61fe-339">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-339">Boolean</span></span>|<span data-ttu-id="d61fe-340">Gibt an, ob die iCloud-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-340">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="d61fe-341">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="d61fe-341">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="d61fe-342">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-342">Boolean</span></span>|<span data-ttu-id="d61fe-343">Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-343">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="d61fe-344">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="d61fe-344">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="d61fe-345">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-345">Boolean</span></span>|<span data-ttu-id="d61fe-346">Gibt an, ob die Cloudsynchronisierung für verwaltete Apps blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-346">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="d61fe-347">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="d61fe-347">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="d61fe-348">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-348">Boolean</span></span>|<span data-ttu-id="d61fe-349">Gibt an, ob die iCloud-Fotomediathek blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-349">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="d61fe-350">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="d61fe-350">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="d61fe-351">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-351">Boolean</span></span>|<span data-ttu-id="d61fe-352">Gibt an, ob die Fotostream-Synchronisierung in iCloud blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-352">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="d61fe-353">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="d61fe-353">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="d61fe-354">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-354">Boolean</span></span>|<span data-ttu-id="d61fe-355">Gibt an, ob die Fotofreigabe blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-355">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="d61fe-356">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="d61fe-356">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="d61fe-357">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-357">Boolean</span></span>|<span data-ttu-id="d61fe-358">Gibt an, ob Sicherungen in iCloud verschlüsselt sein müssen.</span><span class="sxs-lookup"><span data-stu-id="d61fe-358">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="d61fe-359">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="d61fe-359">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="d61fe-360">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-360">Boolean</span></span>|<span data-ttu-id="d61fe-361">Gibt an, ob verhindert werden soll, dass der Benutzer auf anstößige Inhalte in iTunes und im App Store zugreift. </span><span class="sxs-lookup"><span data-stu-id="d61fe-361">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="d61fe-362">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="d61fe-362">iTunesBlockMusicService</span></span>|<span data-ttu-id="d61fe-363">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-363">Boolean</span></span>|<span data-ttu-id="d61fe-364">Gibt an, ob der Music-Dienst blockiert und die Music-App in den klassischen Modus zurückgesetzt werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher und Mac OS 10.12 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-364">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="d61fe-365">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="d61fe-365">iTunesBlockRadio</span></span>|<span data-ttu-id="d61fe-366">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-366">Boolean</span></span>|<span data-ttu-id="d61fe-367">Gibt an, ob verhindert werden soll, dass der Benutzer iTunes Radio verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-367">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d61fe-368">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="d61fe-368">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="d61fe-369">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-369">Boolean</span></span>|<span data-ttu-id="d61fe-370">Gibt an, ob die Autokorrektur der Tastatur blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-370">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d61fe-371">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="d61fe-371">keyboardBlockDictation</span></span>|<span data-ttu-id="d61fe-372">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-372">Boolean</span></span>|<span data-ttu-id="d61fe-373">Gibt an, ob verhindert werden soll, dass der Benutzer die Diktatfunktion verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-373">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-374">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="d61fe-374">keyboardBlockPredictive</span></span>|<span data-ttu-id="d61fe-375">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-375">Boolean</span></span>|<span data-ttu-id="d61fe-376">Gibt an, ob Tastaturwortvorschläge blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-376">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d61fe-377">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="d61fe-377">keyboardBlockShortcuts</span></span>|<span data-ttu-id="d61fe-378">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-378">Boolean</span></span>|<span data-ttu-id="d61fe-379">Gibt an, ob Tastenkombinationen blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-379">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d61fe-380">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="d61fe-380">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="d61fe-381">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-381">Boolean</span></span>|<span data-ttu-id="d61fe-382">Gibt an, ob die Rechtschreibprüfung blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-382">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d61fe-383">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="d61fe-383">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="d61fe-384">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-384">Boolean</span></span>|<span data-ttu-id="d61fe-385">Gibt an, ob Sprachunterstützung im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-385">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-386">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="d61fe-386">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="d61fe-387">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-387">Boolean</span></span>|<span data-ttu-id="d61fe-388">Gibt an, ob Zugriff auf die Einstellungen der Touch-Unterstützung im Kiosk-Modus gewährt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-388">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-389">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="d61fe-389">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="d61fe-390">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-390">Boolean</span></span>|<span data-ttu-id="d61fe-391">Gibt an, ob die automatische Gerätesperre im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-391">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-392">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="d61fe-392">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="d61fe-393">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-393">Boolean</span></span>|<span data-ttu-id="d61fe-394">Gibt ab, ob der Zugriff auf die Farbinversionseinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-394">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-395">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="d61fe-395">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="d61fe-396">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-396">Boolean</span></span>|<span data-ttu-id="d61fe-397">Gibt ab, ob die Verwendung des Ruftonschalters im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-397">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-398">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="d61fe-398">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="d61fe-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61fe-399">Boolean</span></span>|<span data-ttu-id="d61fe-400">Gibt ab, ob die Bildschirmdrehung im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-400">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-401">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="d61fe-401">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="d61fe-402">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-402">Boolean</span></span>|<span data-ttu-id="d61fe-403">Gibt ab, ob die Verwendung der Energiespartaste im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-403">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-404">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="d61fe-404">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="d61fe-405">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-405">Boolean</span></span>|<span data-ttu-id="d61fe-406">Gibt ab, ob die Verwendung des Touchscreens im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-406">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-407">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="d61fe-407">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="d61fe-408">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-408">Boolean</span></span>|<span data-ttu-id="d61fe-409">Gibt ab, ob der Zugriff auf die Einstellungen für Hintergrundkommentare im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-409">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-410">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="d61fe-410">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="d61fe-411">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-411">Boolean</span></span>|<span data-ttu-id="d61fe-412">Gibt ab, ob die Verwendung der Lautstärketasten im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-412">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-413">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="d61fe-413">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="d61fe-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61fe-414">Boolean</span></span>|<span data-ttu-id="d61fe-415">Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d61fe-415">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="d61fe-416">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="d61fe-416">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="d61fe-417">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-417">Boolean</span></span>|<span data-ttu-id="d61fe-418">Gibt ab, ob der Zugriff auf die Zoomeinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-418">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-419">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d61fe-419">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="d61fe-420">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d61fe-420">String</span></span>|<span data-ttu-id="d61fe-421">URL im App Store zu der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-421">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="d61fe-422">Verwenden Sie diese, wenn „KioskModeManagedAppId“ nicht bekannt ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-422">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="d61fe-423">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="d61fe-423">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="d61fe-424">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d61fe-424">String</span></span>|<span data-ttu-id="d61fe-425">ID für integrierte apps, die für den Kiosk-Modus verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d61fe-425">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="d61fe-426">Wird verwendet, wenn "Kioskmodemanagedappid" und KioskModeAppStoreUrl nicht festgelegt sind.</span><span class="sxs-lookup"><span data-stu-id="d61fe-426">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="d61fe-427">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="d61fe-427">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="d61fe-428">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-428">Boolean</span></span>|<span data-ttu-id="d61fe-429">Gibt an, ob Touch-Unterstützung im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-429">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-430">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="d61fe-430">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="d61fe-431">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-431">Boolean</span></span>|<span data-ttu-id="d61fe-432">Gibt ab, ob die Farbinversion im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-432">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-433">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="d61fe-433">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="d61fe-434">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-434">Boolean</span></span>|<span data-ttu-id="d61fe-435">Gibt ab, ob Mono-Audio im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-435">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-436">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="d61fe-436">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="d61fe-437">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-437">Boolean</span></span>|<span data-ttu-id="d61fe-438">Gibt ab, ob Hintergrundkommentare im Kiosk-Modus erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d61fe-438">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-439">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="d61fe-439">kioskModeRequireZoom</span></span>|<span data-ttu-id="d61fe-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61fe-440">Boolean</span></span>|<span data-ttu-id="d61fe-441">Gibt ab, ob Zoom im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-441">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="d61fe-442">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="d61fe-442">kioskModeManagedAppId</span></span>|<span data-ttu-id="d61fe-443">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d61fe-443">String</span></span>|<span data-ttu-id="d61fe-444">Verwaltete App-ID der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-444">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="d61fe-445">Wenn „KioskModeManagedAppId“ angegeben ist, wird „KioskModeAppStoreUrl“ ignoriert.</span><span class="sxs-lookup"><span data-stu-id="d61fe-445">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="d61fe-446">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="d61fe-446">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="d61fe-447">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-447">Boolean</span></span>|<span data-ttu-id="d61fe-448">Gibt an, ob verhindert werden soll, dass der Benutzer das Kontrollzentrum für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-448">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="d61fe-449">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="d61fe-449">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="d61fe-450">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-450">Boolean</span></span>|<span data-ttu-id="d61fe-451">Gibt an, ob verhindert werden soll, dass der Benutzer die Benachrichtigungsansicht auf dem Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-451">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="d61fe-452">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="d61fe-452">lockScreenBlockPassbook</span></span>|<span data-ttu-id="d61fe-453">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-453">Boolean</span></span>|<span data-ttu-id="d61fe-454">Gibt an, ob verhindert werden soll, dass der Benutzer Passbook verwendet, wenn das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-454">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="d61fe-455">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="d61fe-455">lockScreenBlockTodayView</span></span>|<span data-ttu-id="d61fe-456">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-456">Boolean</span></span>|<span data-ttu-id="d61fe-457">Gibt an, ob verhindert werden soll, dass der Benutzer die Ansicht „Heute“ für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-457">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="d61fe-458">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d61fe-458">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="d61fe-459">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d61fe-459">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="d61fe-460">Einstellungen für Medieninhalte für Australien</span><span class="sxs-lookup"><span data-stu-id="d61fe-460">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="d61fe-461">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d61fe-461">mediaContentRatingCanada</span></span>|[<span data-ttu-id="d61fe-462">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d61fe-462">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="d61fe-463">Einstellungen für Medieninhalte für Kanada</span><span class="sxs-lookup"><span data-stu-id="d61fe-463">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="d61fe-464">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d61fe-464">mediaContentRatingFrance</span></span>|[<span data-ttu-id="d61fe-465">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d61fe-465">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="d61fe-466">Einstellungen für Medieninhalte für Frankreich</span><span class="sxs-lookup"><span data-stu-id="d61fe-466">Media content rating settings for France</span></span>|
|<span data-ttu-id="d61fe-467">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d61fe-467">mediaContentRatingGermany</span></span>|[<span data-ttu-id="d61fe-468">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d61fe-468">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="d61fe-469">Einstellungen für Medieninhalte für Deutschland</span><span class="sxs-lookup"><span data-stu-id="d61fe-469">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="d61fe-470">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d61fe-470">mediaContentRatingIreland</span></span>|[<span data-ttu-id="d61fe-471">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d61fe-471">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="d61fe-472">Einstellungen für Medieninhalte für Irland</span><span class="sxs-lookup"><span data-stu-id="d61fe-472">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="d61fe-473">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d61fe-473">mediaContentRatingJapan</span></span>|[<span data-ttu-id="d61fe-474">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d61fe-474">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="d61fe-475">Einstellungen für Medieninhalte für Japan</span><span class="sxs-lookup"><span data-stu-id="d61fe-475">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="d61fe-476">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d61fe-476">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="d61fe-477">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d61fe-477">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="d61fe-478">Einstellungen für Medieninhalte für Neuseeland</span><span class="sxs-lookup"><span data-stu-id="d61fe-478">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="d61fe-479">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d61fe-479">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="d61fe-480">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d61fe-480">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="d61fe-481">Einstellungen für Medieninhalte für das Vereinigte Königreich</span><span class="sxs-lookup"><span data-stu-id="d61fe-481">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="d61fe-482">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d61fe-482">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="d61fe-483">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d61fe-483">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="d61fe-484">Einstellungen für Medieninhalte für die USA</span><span class="sxs-lookup"><span data-stu-id="d61fe-484">Media content rating settings for United States</span></span>|
|<span data-ttu-id="d61fe-485">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="d61fe-485">networkUsageRules</span></span>|<span data-ttu-id="d61fe-486">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d61fe-486">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="d61fe-487">Liste verwalteter Apps und die Netzwerkregeln, die darauf angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="d61fe-487">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="d61fe-488">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d61fe-488">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d61fe-489">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="d61fe-489">mediaContentRatingApps</span></span>|[<span data-ttu-id="d61fe-490">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="d61fe-490">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="d61fe-491">Einstellungen für die Medieninhalts Bewertung für apps.</span><span class="sxs-lookup"><span data-stu-id="d61fe-491">Media content rating settings for Apps.</span></span> <span data-ttu-id="d61fe-492">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12` und `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="d61fe-492">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="d61fe-493">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-493">messagesBlocked</span></span>|<span data-ttu-id="d61fe-494">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-494">Boolean</span></span>|<span data-ttu-id="d61fe-495">Gibt an, ob verhindert werden soll, dass der Benutzer die Nachrichten-App auf dem überwachten Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-495">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="d61fe-496">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-496">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="d61fe-497">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-497">Boolean</span></span>|<span data-ttu-id="d61fe-498">Gibt an, ob die Änderung von Benachrichtigungseinstellungen zugelassen wird (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-498">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d61fe-499">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d61fe-499">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="d61fe-500">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-500">Boolean</span></span>|<span data-ttu-id="d61fe-501">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-501">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d61fe-502">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-502">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="d61fe-503">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-503">Boolean</span></span>|<span data-ttu-id="d61fe-504">Blockiert das Ändern registrierter Touch ID-Fingerabdrücke im überwachten Modus.</span><span class="sxs-lookup"><span data-stu-id="d61fe-504">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-505">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-505">passcodeBlockModification</span></span>|<span data-ttu-id="d61fe-506">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-506">Boolean</span></span>|<span data-ttu-id="d61fe-507">Gibt an, ob das Ändern der Kennung auf dem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-507">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d61fe-508">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d61fe-508">passcodeBlockSimple</span></span>|<span data-ttu-id="d61fe-509">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-509">Boolean</span></span>|<span data-ttu-id="d61fe-510">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="d61fe-510">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="d61fe-511">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d61fe-511">passcodeExpirationDays</span></span>|<span data-ttu-id="d61fe-512">Int32</span><span class="sxs-lookup"><span data-stu-id="d61fe-512">Int32</span></span>|<span data-ttu-id="d61fe-513">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="d61fe-513">Number of days before the passcode expires.</span></span> <span data-ttu-id="d61fe-514">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="d61fe-514">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="d61fe-515">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d61fe-515">passcodeMinimumLength</span></span>|<span data-ttu-id="d61fe-516">Int32</span><span class="sxs-lookup"><span data-stu-id="d61fe-516">Int32</span></span>|<span data-ttu-id="d61fe-517">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="d61fe-517">Minimum length of passcode.</span></span> <span data-ttu-id="d61fe-518">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="d61fe-518">Valid values 4 to 14</span></span>|
|<span data-ttu-id="d61fe-519">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d61fe-519">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d61fe-520">Int32</span><span class="sxs-lookup"><span data-stu-id="d61fe-520">Int32</span></span>|<span data-ttu-id="d61fe-521">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-521">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="d61fe-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d61fe-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d61fe-523">Int32</span><span class="sxs-lookup"><span data-stu-id="d61fe-523">Int32</span></span>|<span data-ttu-id="d61fe-524">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="d61fe-524">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d61fe-525">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d61fe-525">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="d61fe-526">Int32</span><span class="sxs-lookup"><span data-stu-id="d61fe-526">Int32</span></span>|<span data-ttu-id="d61fe-527">Anzahl von Zeichensätzen, die eine Kennung enthalten muss</span><span class="sxs-lookup"><span data-stu-id="d61fe-527">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="d61fe-528">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="d61fe-528">Valid values 0 to 4</span></span>|
|<span data-ttu-id="d61fe-529">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="d61fe-529">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="d61fe-530">Int32</span><span class="sxs-lookup"><span data-stu-id="d61fe-530">Int32</span></span>|<span data-ttu-id="d61fe-531">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d61fe-531">Number of previous passcodes to block.</span></span> <span data-ttu-id="d61fe-532">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="d61fe-532">Valid values 1 to 24</span></span>|
|<span data-ttu-id="d61fe-533">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="d61fe-533">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="d61fe-534">Int32</span><span class="sxs-lookup"><span data-stu-id="d61fe-534">Int32</span></span>|<span data-ttu-id="d61fe-535">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung des Geräts durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d61fe-535">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="d61fe-536">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="d61fe-536">Valid values 4 to 11</span></span>|
|<span data-ttu-id="d61fe-537">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="d61fe-537">passcodeRequiredType</span></span>|[<span data-ttu-id="d61fe-538">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d61fe-538">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d61fe-539">Geforderter Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="d61fe-539">Type of passcode that is required.</span></span> <span data-ttu-id="d61fe-540">Mögliche Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d61fe-540">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d61fe-541">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="d61fe-541">passcodeRequired</span></span>|<span data-ttu-id="d61fe-542">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-542">Boolean</span></span>|<span data-ttu-id="d61fe-543">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-543">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="d61fe-544">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-544">podcastsBlocked</span></span>|<span data-ttu-id="d61fe-545">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-545">Boolean</span></span>|<span data-ttu-id="d61fe-546">Gibt an, ob verhindert werden soll, dass der Benutzer Podcasts auf dem überwachten Gerät verwendet (iOS 8.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-546">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="d61fe-547">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="d61fe-547">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="d61fe-548">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-548">Boolean</span></span>|<span data-ttu-id="d61fe-549">Gibt an, ob die Ansage zum Einrichten von benachbarten Geräten mit einem überwachten Gerät aktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-549">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="d61fe-550">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="d61fe-550">safariBlockAutofill</span></span>|<span data-ttu-id="d61fe-551">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-551">Boolean</span></span>|<span data-ttu-id="d61fe-552">Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-552">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="d61fe-553">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="d61fe-553">safariBlockJavaScript</span></span>|<span data-ttu-id="d61fe-554">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-554">Boolean</span></span>|<span data-ttu-id="d61fe-555">Gibt an, ob JavaScript in Safari blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-555">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="d61fe-556">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="d61fe-556">safariBlockPopups</span></span>|<span data-ttu-id="d61fe-557">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-557">Boolean</span></span>|<span data-ttu-id="d61fe-558">Gibt an, ob Popups in Safari blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d61fe-558">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="d61fe-559">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-559">safariBlocked</span></span>|<span data-ttu-id="d61fe-560">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-560">Boolean</span></span>|<span data-ttu-id="d61fe-561">Gibt an, ob verhindert werden soll, dass der Benutzer Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-561">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="d61fe-562">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d61fe-562">safariCookieSettings</span></span>|[<span data-ttu-id="d61fe-563">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d61fe-563">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="d61fe-564">Cokkieeinstellungen für Safari.</span><span class="sxs-lookup"><span data-stu-id="d61fe-564">Cookie settings for Safari.</span></span> <span data-ttu-id="d61fe-565">Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="d61fe-565">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="d61fe-566">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="d61fe-566">safariManagedDomains</span></span>|<span data-ttu-id="d61fe-567">String collection</span><span class="sxs-lookup"><span data-stu-id="d61fe-567">String collection</span></span>|<span data-ttu-id="d61fe-568">URLs, die mit den hier aufgeführten Mustern übereinstimmen, werden als verwaltet betrachtet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-568">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="d61fe-569">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="d61fe-569">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="d61fe-570">String collection</span><span class="sxs-lookup"><span data-stu-id="d61fe-570">String collection</span></span>|<span data-ttu-id="d61fe-571">Benutzer können Kennwörter in Safari nur von URLs speichern, die mit den hier aufgeführten Mustern übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="d61fe-571">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="d61fe-572">Gilt für Geräte im überwachten Modus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-572">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d61fe-573">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="d61fe-573">safariRequireFraudWarning</span></span>|<span data-ttu-id="d61fe-574">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-574">Boolean</span></span>|<span data-ttu-id="d61fe-575">Gibt an, ob eine Betrugswarnung in Safari erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-575">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="d61fe-576">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-576">screenCaptureBlocked</span></span>|<span data-ttu-id="d61fe-577">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-577">Boolean</span></span>|<span data-ttu-id="d61fe-578">Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.</span><span class="sxs-lookup"><span data-stu-id="d61fe-578">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="d61fe-579">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-579">siriBlocked</span></span>|<span data-ttu-id="d61fe-580">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-580">Boolean</span></span>|<span data-ttu-id="d61fe-581">Gibt an, ob verhindert werden soll, dass der Benutzer Siri verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-581">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="d61fe-582">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-582">siriBlockedWhenLocked</span></span>|<span data-ttu-id="d61fe-583">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-583">Boolean</span></span>|<span data-ttu-id="d61fe-584">Gibt an, ob verhindert werden soll, dass der Benutzer Siri bei Sperrung verwendet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-584">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="d61fe-585">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="d61fe-585">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="d61fe-586">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-586">Boolean</span></span>|<span data-ttu-id="d61fe-587">Gibt an, ob Siri bei Verwendung auf einem überwachten Gerät davon abgehalten werden soll, benutzergenerierte Inhalte abzufragen.</span><span class="sxs-lookup"><span data-stu-id="d61fe-587">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="d61fe-588">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="d61fe-588">siriRequireProfanityFilter</span></span>|<span data-ttu-id="d61fe-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61fe-589">Boolean</span></span>|<span data-ttu-id="d61fe-590">Gibt an, ob verhindert werden soll, dass Siri anstößige Ausdrücke auf dem überwachten Gerät diktiert oder spricht.</span><span class="sxs-lookup"><span data-stu-id="d61fe-590">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="d61fe-591">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="d61fe-591">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="d61fe-592">Int32</span><span class="sxs-lookup"><span data-stu-id="d61fe-592">Int32</span></span>|<span data-ttu-id="d61fe-593">Legt fest, wie viele Tage ein Software Update für ein überwachte Gerät delyed wird.</span><span class="sxs-lookup"><span data-stu-id="d61fe-593">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="d61fe-594">Gültige Werte: 0 bis 90.</span><span class="sxs-lookup"><span data-stu-id="d61fe-594">Valid values 0 to 90</span></span>|
|<span data-ttu-id="d61fe-595">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="d61fe-595">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="d61fe-596">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-596">Boolean</span></span>|<span data-ttu-id="d61fe-597">Gibt an, ob die Benutzersicht barkeit von Softwareupdates verzögert werden soll, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-597">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-598">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="d61fe-598">spotlightBlockInternetResults</span></span>|<span data-ttu-id="d61fe-599">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-599">Boolean</span></span>|<span data-ttu-id="d61fe-600">Gibt an, ob verhindert werden soll, dass die Spotlight-Suche Internetergebnisse auf dem überwachten Gerät zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="d61fe-600">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="d61fe-601">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-601">voiceDialingBlocked</span></span>|<span data-ttu-id="d61fe-602">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61fe-602">Boolean</span></span>|<span data-ttu-id="d61fe-603">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-603">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="d61fe-604">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="d61fe-604">wallpaperBlockModification</span></span>|<span data-ttu-id="d61fe-605">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-605">Boolean</span></span>|<span data-ttu-id="d61fe-606">Gibt an, ob das Ändern des Hintergrunds auf einem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-606">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="d61fe-607">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="d61fe-607">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="d61fe-608">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-608">Boolean</span></span>|<span data-ttu-id="d61fe-609">Gibt an, ob erzwungen werden soll, dass das Gerät nur WLAN-Netzwerke aus Konfigurationsprofilen verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="d61fe-609">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d61fe-610">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="d61fe-610">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="d61fe-611">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-611">Boolean</span></span>|<span data-ttu-id="d61fe-612">Gibt an, ob ein Teilnehmer, der über das Klassenzimmer in einem nicht verwalteten Kurs angemeldet ist, beim Versuch, den Kurs zu verlassen (iOS 11,3 und höher) die Berechtigung des Lehrers anfordert.</span><span class="sxs-lookup"><span data-stu-id="d61fe-612">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="d61fe-613">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="d61fe-613">keychainBlockCloudSync</span></span>|<span data-ttu-id="d61fe-614">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-614">Boolean</span></span>|<span data-ttu-id="d61fe-615">Gibt an, ob die iCloud-Schlüsselbund Synchronisierung blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-615">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="d61fe-616">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="d61fe-616">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="d61fe-617">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-617">Boolean</span></span>|<span data-ttu-id="d61fe-618">Gibt an, ob over-the-Air-PKI-Updates blockiert sind.</span><span class="sxs-lookup"><span data-stu-id="d61fe-618">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="d61fe-619">Wenn Sie diese Einschränkung auf false festlegen, werden CRL-und OCSP-Prüfungen nicht deaktiviert (iOS 7,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-619">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="d61fe-620">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="d61fe-620">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="d61fe-621">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-621">Boolean</span></span>|<span data-ttu-id="d61fe-622">Gibt an, ob die AD-Verfolgung begrenzt ist. (iOS 7,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-622">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="d61fe-623">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="d61fe-623">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="d61fe-624">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-624">Boolean</span></span>|<span data-ttu-id="d61fe-625">Gibt an, ob Enterprise Book Back up gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-625">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="d61fe-626">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="d61fe-626">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="d61fe-627">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-627">Boolean</span></span>|<span data-ttu-id="d61fe-628">Gibt an, ob die Synchronisierung von Enterprise Book Notes und Highlights blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-628">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="d61fe-629">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-629">airPrintBlocked</span></span>|<span data-ttu-id="d61fe-630">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-630">Boolean</span></span>|<span data-ttu-id="d61fe-631">Gibt an, ob der druckDruck blockiert ist (iOS 11,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-631">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d61fe-632">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="d61fe-632">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="d61fe-633">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-633">Boolean</span></span>|<span data-ttu-id="d61fe-634">Gibt an, ob die Schlüsselbund Speicherung von Benutzername und Kennwort für druckdruck blockiert ist (iOS 11,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-634">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d61fe-635">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="d61fe-635">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="d61fe-636">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-636">Boolean</span></span>|<span data-ttu-id="d61fe-637">Gibt an, ob vertrauenswürdige Zertifikate für die TLS-Druckkommunikation erforderlich sind (iOS 11,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-637">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d61fe-638">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="d61fe-638">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="d61fe-639">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-639">Boolean</span></span>|<span data-ttu-id="d61fe-640">Gibt an, ob die iBeacon-Erkennung von Druckern blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="d61fe-640">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="d61fe-641">Dadurch wird verhindert, dass gefälschte Bluetooth-Baken für den Netzwerkdatenverkehr aus dem Phishing entfernt werden (iOS 11,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-641">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d61fe-642">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="d61fe-642">blockSystemAppRemoval</span></span>|<span data-ttu-id="d61fe-643">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-643">Boolean</span></span>|<span data-ttu-id="d61fe-644">Gibt an, ob das Entfernen von System-apps vom Gerät auf einem überwachten Gerät (iOS 11,0 und höher) blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-644">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d61fe-645">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="d61fe-645">vpnBlockCreation</span></span>|<span data-ttu-id="d61fe-646">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-646">Boolean</span></span>|<span data-ttu-id="d61fe-647">Gibt an, ob die Erstellung von VPN-Konfigurationen blockiert ist (iOS 11,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-647">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d61fe-648">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-648">appRemovalBlocked</span></span>|<span data-ttu-id="d61fe-649">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-649">Boolean</span></span>|<span data-ttu-id="d61fe-650">Gibt an, ob das Entfernen von apps zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-650">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="d61fe-651">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="d61fe-651">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="d61fe-652">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-652">Boolean</span></span>|<span data-ttu-id="d61fe-653">Gibt an, ob das Herstellen einer Verbindung mit USB-Zubehör während der Sperrung des Geräts zulässig ist (iOS 11.4.1 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-653">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="d61fe-654">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="d61fe-654">passwordBlockAutoFill</span></span>|<span data-ttu-id="d61fe-655">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-655">Boolean</span></span>|<span data-ttu-id="d61fe-656">Gibt an, ob das Feature AutoFill passwords (iOS 12,0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="d61fe-656">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d61fe-657">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="d61fe-657">passwordBlockProximityRequests</span></span>|<span data-ttu-id="d61fe-658">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-658">Boolean</span></span>|<span data-ttu-id="d61fe-659">Gibt an, ob das Anfordern von Kennwörtern von benachbarten Geräten (iOS 12,0 und höher) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-659">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d61fe-660">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="d61fe-660">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="d61fe-661">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-661">Boolean</span></span>|<span data-ttu-id="d61fe-662">Gibt an, ob das Freigeben von Kennwörtern für die Kennwörter von iOS 12,0 und höher blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d61fe-662">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d61fe-663">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="d61fe-663">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="d61fe-664">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-664">Boolean</span></span>|<span data-ttu-id="d61fe-665">Gibt an, ob die Funktion für Datum und Uhrzeit "automatisch festlegen" aktiviert ist und nicht vom Benutzer deaktiviert werden kann (iOS 12,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-665">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d61fe-666">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="d61fe-666">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="d61fe-667">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-667">Boolean</span></span>|<span data-ttu-id="d61fe-668">Gibt an, ob verwaltete Apps Kontakte in nicht verwaltete Kontakte-Konten schreiben können (iOS 12,0 und höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-668">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d61fe-669">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="d61fe-669">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="d61fe-670">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d61fe-670">Boolean</span></span>|<span data-ttu-id="d61fe-671">Gibt an, ob nicht verwaltete Apps aus Konten für verwaltete Kontakte lesen können (iOS 12,0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="d61fe-671">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="d61fe-672">Antwort</span><span class="sxs-lookup"><span data-stu-id="d61fe-672">Response</span></span>
<span data-ttu-id="d61fe-673">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d61fe-673">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d61fe-674">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d61fe-674">Example</span></span>

### <a name="request"></a><span data-ttu-id="d61fe-675">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d61fe-675">Request</span></span>
<span data-ttu-id="d61fe-676">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d61fe-676">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d61fe-677">Antwort</span><span class="sxs-lookup"><span data-stu-id="d61fe-677">Response</span></span>
<span data-ttu-id="d61fe-p133">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d61fe-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




