---
title: iosGeneralDeviceConfiguration erstellen
description: Erstellen Sie ein neues iosGeneralDeviceConfiguration-Objekt.
ms.openlocfilehash: cb3231d5da3e06039533167f42a1088bb931c956
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019035"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="c07cb-103">iosGeneralDeviceConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="c07cb-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c07cb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c07cb-105">Erstellen Sie ein neues [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="c07cb-105">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c07cb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c07cb-106">Prerequisites</span></span>
<span data-ttu-id="c07cb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c07cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c07cb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c07cb-109">Permission type</span></span>|<span data-ttu-id="c07cb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c07cb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c07cb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c07cb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c07cb-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c07cb-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c07cb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c07cb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c07cb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c07cb-114">Not supported.</span></span>|
|<span data-ttu-id="c07cb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c07cb-115">Application</span></span>|<span data-ttu-id="c07cb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c07cb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c07cb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c07cb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c07cb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c07cb-118">Request headers</span></span>
|<span data-ttu-id="c07cb-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c07cb-119">Header</span></span>|<span data-ttu-id="c07cb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c07cb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c07cb-121">Authorization</span></span>|<span data-ttu-id="c07cb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c07cb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c07cb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c07cb-123">Accept</span></span>|<span data-ttu-id="c07cb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c07cb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c07cb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c07cb-125">Request body</span></span>
<span data-ttu-id="c07cb-126">Geben Sie im Anforderungstext eine JSON-Darstellung des iosGeneralDeviceConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c07cb-126">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="c07cb-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs iosGeneralDeviceConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="c07cb-127">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="c07cb-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c07cb-128">Property</span></span>|<span data-ttu-id="c07cb-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c07cb-129">Type</span></span>|<span data-ttu-id="c07cb-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c07cb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c07cb-131">id</span><span class="sxs-lookup"><span data-stu-id="c07cb-131">id</span></span>|<span data-ttu-id="c07cb-132">String</span><span class="sxs-lookup"><span data-stu-id="c07cb-132">String</span></span>|<span data-ttu-id="c07cb-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c07cb-133">Key of the entity.</span></span> <span data-ttu-id="c07cb-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c07cb-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c07cb-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c07cb-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c07cb-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c07cb-136">DateTimeOffset</span></span>|<span data-ttu-id="c07cb-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c07cb-137">DateTime the object was last modified.</span></span> <span data-ttu-id="c07cb-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c07cb-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c07cb-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c07cb-139">createdDateTime</span></span>|<span data-ttu-id="c07cb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c07cb-140">DateTimeOffset</span></span>|<span data-ttu-id="c07cb-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c07cb-141">DateTime the object was created.</span></span> <span data-ttu-id="c07cb-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c07cb-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c07cb-143">description</span><span class="sxs-lookup"><span data-stu-id="c07cb-143">description</span></span>|<span data-ttu-id="c07cb-144">String</span><span class="sxs-lookup"><span data-stu-id="c07cb-144">String</span></span>|<span data-ttu-id="c07cb-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c07cb-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c07cb-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c07cb-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c07cb-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c07cb-147">displayName</span></span>|<span data-ttu-id="c07cb-148">String</span><span class="sxs-lookup"><span data-stu-id="c07cb-148">String</span></span>|<span data-ttu-id="c07cb-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c07cb-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c07cb-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c07cb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c07cb-151">Version</span><span class="sxs-lookup"><span data-stu-id="c07cb-151">version</span></span>|<span data-ttu-id="c07cb-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c07cb-152">Int32</span></span>|<span data-ttu-id="c07cb-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c07cb-153">Version of the device configuration.</span></span> <span data-ttu-id="c07cb-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c07cb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c07cb-155">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="c07cb-155">accountBlockModification</span></span>|<span data-ttu-id="c07cb-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-156">Boolean</span></span>|<span data-ttu-id="c07cb-157">Gibt an, ob die Kontoänderung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-157">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-158">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="c07cb-158">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="c07cb-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-159">Boolean</span></span>|<span data-ttu-id="c07cb-160">Gibt an, ob die Aktivierungssperre zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-160">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="c07cb-161">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-161">airDropBlocked</span></span>|<span data-ttu-id="c07cb-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-162">Boolean</span></span>|<span data-ttu-id="c07cb-163">Gibt an, ob AirDrop zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-163">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-164">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="c07cb-164">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="c07cb-165">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-165">Boolean</span></span>|<span data-ttu-id="c07cb-166">Gibt an, ob AirDrop als nicht verwaltetes Drop-Ziel (iOS 9.0 oder höher) betrachtet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-166">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c07cb-167">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="c07cb-167">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="c07cb-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-168">Boolean</span></span>|<span data-ttu-id="c07cb-169">Gibt an, ob erzwungen werden soll, dass alle Geräte, die AirPlay-Anforderungen von diesem Gerät erhalten, ein Kopplungskennwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="c07cb-169">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="c07cb-170">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="c07cb-170">appleWatchBlockPairing</span></span>|<span data-ttu-id="c07cb-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-171">Boolean</span></span>|<span data-ttu-id="c07cb-172">Gibt an, ob eine Apple Watch-Kopplung zulässig ist, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-172">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c07cb-173">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="c07cb-173">appleWatchForceWristDetection</span></span>|<span data-ttu-id="c07cb-174">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-174">Boolean</span></span>|<span data-ttu-id="c07cb-175">Gibt an, ob erzwungen werden soll, dass eine gekoppelte Apple Watch die Handgelenkerkennung (iOS 8.2 und höher) verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-175">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="c07cb-176">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-176">appleNewsBlocked</span></span>|<span data-ttu-id="c07cb-177">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-177">Boolean</span></span>|<span data-ttu-id="c07cb-178">Gibt an, ob verhindert werden soll, dass der Benutzer News verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-178">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c07cb-179">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="c07cb-179">appsSingleAppModeList</span></span>|<span data-ttu-id="c07cb-180">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c07cb-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c07cb-181">Ruft die Liste von iOS-Apps ab, die autonom in den Einzelanwendungsmodus wechseln können, ab oder legt diese fest.</span><span class="sxs-lookup"><span data-stu-id="c07cb-181">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="c07cb-182">Nur überwacht.</span><span class="sxs-lookup"><span data-stu-id="c07cb-182">Supervised only.</span></span> <span data-ttu-id="c07cb-183">iOS 7.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="c07cb-183">iOS 7.0 and later.</span></span> <span data-ttu-id="c07cb-184">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c07cb-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c07cb-185">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="c07cb-185">appsVisibilityList</span></span>|<span data-ttu-id="c07cb-186">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c07cb-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c07cb-187">Liste von Apps in der Sichtbarkeitsliste (entweder eine Liste sichtbarer/startbarer Apps oder eine Liste ausgeblendeter/nicht startbarer Apps, gesteuert von AppsVisibilityListType) (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-187">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="c07cb-188">Diese Sammlung darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c07cb-188">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c07cb-189">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="c07cb-189">appsVisibilityListType</span></span>|[<span data-ttu-id="c07cb-190">appListType</span><span class="sxs-lookup"><span data-stu-id="c07cb-190">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c07cb-191">Typ der in „AppsVisibilityList“ enthaltenen Liste.</span><span class="sxs-lookup"><span data-stu-id="c07cb-191">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="c07cb-192">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="c07cb-192">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c07cb-193">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="c07cb-193">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="c07cb-194">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-194">Boolean</span></span>|<span data-ttu-id="c07cb-195">Gibt an, ob das automatische Herunterladen von Apps blockiert werden soll, die auf anderen Geräten gekauft wurden, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-195">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c07cb-196">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-196">appStoreBlocked</span></span>|<span data-ttu-id="c07cb-197">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-197">Boolean</span></span>|<span data-ttu-id="c07cb-198">Gibt an, ob verhindert werden soll, dass der Benutzer den App Store verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-198">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="c07cb-199">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="c07cb-199">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="c07cb-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-200">Boolean</span></span>|<span data-ttu-id="c07cb-201">Gibt an, ob verhindert werden soll, dass der Benutzer In-App-Käufe tätigt.</span><span class="sxs-lookup"><span data-stu-id="c07cb-201">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="c07cb-202">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c07cb-202">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="c07cb-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-203">Boolean</span></span>|<span data-ttu-id="c07cb-204">Gibt an, ob die App Store-App blockiert werden soll, ohne die Installation über Host-Apps einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="c07cb-204">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="c07cb-205">Gilt nur für den überwachten Modus (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-205">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c07cb-206">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="c07cb-206">appStoreRequirePassword</span></span>|<span data-ttu-id="c07cb-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-207">Boolean</span></span>|<span data-ttu-id="c07cb-208">Gibt an, ob bei Verwendung des App Stores ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-208">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="c07cb-209">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="c07cb-209">bluetoothBlockModification</span></span>|<span data-ttu-id="c07cb-210">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-210">Boolean</span></span>|<span data-ttu-id="c07cb-211">Gibt an, ob das Ändern von Bluetooth-Einstellungen zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 10.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-211">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="c07cb-212">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-212">cameraBlocked</span></span>|<span data-ttu-id="c07cb-213">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-213">Boolean</span></span>|<span data-ttu-id="c07cb-214">Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.</span><span class="sxs-lookup"><span data-stu-id="c07cb-214">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="c07cb-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="c07cb-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="c07cb-216">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-216">Boolean</span></span>|<span data-ttu-id="c07cb-217">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="c07cb-218">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="c07cb-218">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="c07cb-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-219">Boolean</span></span>|<span data-ttu-id="c07cb-220">Gibt an, ob das globales Abrufen im Hintergrund beim Roaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-220">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="c07cb-221">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="c07cb-221">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="c07cb-222">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-222">Boolean</span></span>|<span data-ttu-id="c07cb-223">Gibt an, ob Änderungen an den Mobil-App-Daten zulässig sind, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-223">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-224">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="c07cb-224">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="c07cb-225">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-225">Boolean</span></span>|<span data-ttu-id="c07cb-226">Gibt an, ob der privater Hotspot blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-226">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="c07cb-227">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="c07cb-227">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="c07cb-228">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-228">Boolean</span></span>|<span data-ttu-id="c07cb-229">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-229">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="c07cb-230">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="c07cb-230">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="c07cb-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-231">Boolean</span></span>|<span data-ttu-id="c07cb-232">Gibt an, ob nicht vertrauenswürdige TLS-Zertifikate blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c07cb-232">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="c07cb-233">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="c07cb-233">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="c07cb-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-234">Boolean</span></span>|<span data-ttu-id="c07cb-235">Gibt an, ob die Remotebildschirmüberwachung über die Classroom-App zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-235">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="c07cb-236">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="c07cb-236">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="c07cb-237">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-237">Boolean</span></span>|<span data-ttu-id="c07cb-238">Gibt an, ob dem Lehrer eines verwalteten Kurses in der Classroom-App automatisch die Berechtigung erteilt werden soll, den Bildschirm eines Kursteilnehmers ohne Aufforderung anzuzeigen, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-238">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-239">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c07cb-239">compliantAppsList</span></span>|<span data-ttu-id="c07cb-240">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c07cb-240">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c07cb-241">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="c07cb-241">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c07cb-242">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c07cb-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c07cb-243">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c07cb-243">compliantAppListType</span></span>|[<span data-ttu-id="c07cb-244">appListType</span><span class="sxs-lookup"><span data-stu-id="c07cb-244">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c07cb-245">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="c07cb-245">List that is in the AppComplianceList.</span></span> <span data-ttu-id="c07cb-246">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="c07cb-246">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c07cb-247">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="c07cb-247">configurationProfileBlockChanges</span></span>|<span data-ttu-id="c07cb-248">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-248">Boolean</span></span>|<span data-ttu-id="c07cb-249">Gibt an, ob verhindert werden soll, dass der Benutzer Konfigurationsprofile und Zertifikate interaktiv installiert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-249">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-250">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-250">definitionLookupBlocked</span></span>|<span data-ttu-id="c07cb-251">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-251">Boolean</span></span>|<span data-ttu-id="c07cb-252">Gibt an, ob die Definitionssuche zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-252">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="c07cb-253">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="c07cb-253">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="c07cb-254">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-254">Boolean</span></span>|<span data-ttu-id="c07cb-255">Gibt an, ob erlaubt werden soll, dass der Benutzer Einschränkungen in den Geräteeinstellungen aktiviert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-255">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-256">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="c07cb-256">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="c07cb-257">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-257">Boolean</span></span>|<span data-ttu-id="c07cb-258">Gibt an, ob die Verwendung der Option zum Löschen aller Inhalte und Einstellungen auf dem Gerät zugelassen werden soll, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-258">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-259">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="c07cb-259">deviceBlockNameModification</span></span>|<span data-ttu-id="c07cb-260">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-260">Boolean</span></span>|<span data-ttu-id="c07cb-261">Gibt an, ob das Ändern des Gerätenamens zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-261">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c07cb-262">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="c07cb-262">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="c07cb-263">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-263">Boolean</span></span>|<span data-ttu-id="c07cb-264">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-264">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="c07cb-265">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="c07cb-265">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="c07cb-266">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-266">Boolean</span></span>|<span data-ttu-id="c07cb-267">Gibt an, ob das Ändern der Einstellungen für die Diagnoseübermittlung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3.2 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-267">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="c07cb-268">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="c07cb-268">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="c07cb-269">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-269">Boolean</span></span>|<span data-ttu-id="c07cb-270">Gibt an, ob verhindert werden soll, dass der Benutzer verwaltete Dokumente in nicht verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="c07cb-270">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="c07cb-271">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="c07cb-271">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="c07cb-272">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-272">Boolean</span></span>|<span data-ttu-id="c07cb-273">Gibt an, ob verhindert werden soll, dass der Benutzer nicht verwaltete Dokumente in verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="c07cb-273">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="c07cb-274">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="c07cb-274">emailInDomainSuffixes</span></span>|<span data-ttu-id="c07cb-275">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c07cb-275">String collection</span></span>|<span data-ttu-id="c07cb-276">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="c07cb-276">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="c07cb-277">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="c07cb-277">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="c07cb-278">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-278">Boolean</span></span>|<span data-ttu-id="c07cb-279">Gibt an, ob verhindert werden soll, dass der Benutzer einer Unternehmens-App vertraut.</span><span class="sxs-lookup"><span data-stu-id="c07cb-279">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="c07cb-280">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="c07cb-280">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="c07cb-281">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-281">Boolean</span></span>|<span data-ttu-id="c07cb-282">Gibt an, ob verhindert werden soll, dass der Benutzer die Vertrauensstellungseinstellungen der Unternehmens-App ändert.</span><span class="sxs-lookup"><span data-stu-id="c07cb-282">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="c07cb-283">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-283">faceTimeBlocked</span></span>|<span data-ttu-id="c07cb-284">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-284">Boolean</span></span>|<span data-ttu-id="c07cb-285">Gibt an, ob verhindert werden soll, dass der Benutzer FaceTime verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-285">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="c07cb-286">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-286">findMyFriendsBlocked</span></span>|<span data-ttu-id="c07cb-287">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-287">Boolean</span></span>|<span data-ttu-id="c07cb-288">Gibt an, ob „Freunde suchen“ blockiert wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-288">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-289">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="c07cb-289">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="c07cb-290">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-290">Boolean</span></span>|<span data-ttu-id="c07cb-291">Gibt an, ob verhindert werden soll, dass der Benutzer Freunde im Game Center hat.</span><span class="sxs-lookup"><span data-stu-id="c07cb-291">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="c07cb-292">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="c07cb-292">gamingBlockMultiplayer</span></span>|<span data-ttu-id="c07cb-293">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-293">Boolean</span></span>|<span data-ttu-id="c07cb-294">Gibt an, ob verhindert werden soll, dass der Benutzer Multiplayerspiele verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-294">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="c07cb-295">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-295">gameCenterBlocked</span></span>|<span data-ttu-id="c07cb-296">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-296">Boolean</span></span>|<span data-ttu-id="c07cb-297">Gibt an, ob verhindert werden soll, dass der Benutzer Game Center verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-297">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-298">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-298">hostPairingBlocked</span></span>|<span data-ttu-id="c07cb-299">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-299">Boolean</span></span>|<span data-ttu-id="c07cb-300">Gibt an, ob die Hostkopplung blockiert werden soll, um zu steuern, mit welchen Geräten ein iOS-Gerät gekoppelt werden kann,wenn sich das iOS-Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-300">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-301">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-301">iBooksStoreBlocked</span></span>|<span data-ttu-id="c07cb-302">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-302">Boolean</span></span>|<span data-ttu-id="c07cb-303">Gibt an, ob verhindert werden soll, dass der Benutzer den iBooks Store verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-303">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-304">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="c07cb-304">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="c07cb-305">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-305">Boolean</span></span>|<span data-ttu-id="c07cb-306">Gibt an, ob verhindert werden soll, dass der Benutzer Medien aus dem iBook Store herunterlädt, die als Erotik gekennzeichnet sind.</span><span class="sxs-lookup"><span data-stu-id="c07cb-306">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="c07cb-307">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="c07cb-307">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="c07cb-308">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-308">Boolean</span></span>|<span data-ttu-id="c07cb-309">Gibt an, ob verhindert werden soll, dass der Benutzer eine Aufgabe, die er auf dem iOS-Gerät begonnen hat, auf einem anderen iOS- oder macOS-Gerät fortsetzt.</span><span class="sxs-lookup"><span data-stu-id="c07cb-309">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="c07cb-310">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="c07cb-310">iCloudBlockBackup</span></span>|<span data-ttu-id="c07cb-311">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-311">Boolean</span></span>|<span data-ttu-id="c07cb-312">Gibt an, ob die iCloud-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-312">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="c07cb-313">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="c07cb-313">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="c07cb-314">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-314">Boolean</span></span>|<span data-ttu-id="c07cb-315">Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-315">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="c07cb-316">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="c07cb-316">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="c07cb-317">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-317">Boolean</span></span>|<span data-ttu-id="c07cb-318">Gibt an, ob die Cloudsynchronisierung für verwaltete Apps blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-318">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="c07cb-319">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="c07cb-319">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="c07cb-320">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-320">Boolean</span></span>|<span data-ttu-id="c07cb-321">Gibt an, ob die iCloud-Fotomediathek blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-321">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="c07cb-322">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="c07cb-322">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="c07cb-323">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-323">Boolean</span></span>|<span data-ttu-id="c07cb-324">Gibt an, ob die Fotostream-Synchronisierung in iCloud blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-324">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="c07cb-325">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="c07cb-325">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="c07cb-326">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-326">Boolean</span></span>|<span data-ttu-id="c07cb-327">Gibt an, ob die Fotofreigabe blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-327">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="c07cb-328">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="c07cb-328">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="c07cb-329">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-329">Boolean</span></span>|<span data-ttu-id="c07cb-330">Gibt an, ob Sicherungen in iCloud verschlüsselt sein müssen.</span><span class="sxs-lookup"><span data-stu-id="c07cb-330">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="c07cb-331">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="c07cb-331">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="c07cb-332">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-332">Boolean</span></span>|<span data-ttu-id="c07cb-333">Gibt an, ob verhindert werden soll, dass der Benutzer auf anstößige Inhalte in iTunes und im App Store zugreift. </span><span class="sxs-lookup"><span data-stu-id="c07cb-333">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="c07cb-334">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="c07cb-334">iTunesBlockMusicService</span></span>|<span data-ttu-id="c07cb-335">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-335">Boolean</span></span>|<span data-ttu-id="c07cb-336">Gibt an, ob der Music-Dienst blockiert und die Music-App in den klassischen Modus zurückgesetzt werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher und Mac OS 10.12 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-336">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="c07cb-337">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="c07cb-337">iTunesBlockRadio</span></span>|<span data-ttu-id="c07cb-338">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-338">Boolean</span></span>|<span data-ttu-id="c07cb-339">Gibt an, ob verhindert werden soll, dass der Benutzer iTunes Radio verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-339">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="c07cb-340">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="c07cb-340">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="c07cb-341">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-341">Boolean</span></span>|<span data-ttu-id="c07cb-342">Gibt an, ob die Autokorrektur der Tastatur blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-342">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="c07cb-343">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="c07cb-343">keyboardBlockDictation</span></span>|<span data-ttu-id="c07cb-344">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-344">Boolean</span></span>|<span data-ttu-id="c07cb-345">Gibt an, ob verhindert werden soll, dass der Benutzer die Diktatfunktion verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-345">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-346">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="c07cb-346">keyboardBlockPredictive</span></span>|<span data-ttu-id="c07cb-347">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-347">Boolean</span></span>|<span data-ttu-id="c07cb-348">Gibt an, ob Tastaturwortvorschläge blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-348">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="c07cb-349">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="c07cb-349">keyboardBlockShortcuts</span></span>|<span data-ttu-id="c07cb-350">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-350">Boolean</span></span>|<span data-ttu-id="c07cb-351">Gibt an, ob Tastenkombinationen blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-351">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c07cb-352">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="c07cb-352">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="c07cb-353">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-353">Boolean</span></span>|<span data-ttu-id="c07cb-354">Gibt an, ob die Rechtschreibprüfung blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-354">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="c07cb-355">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="c07cb-355">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="c07cb-356">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-356">Boolean</span></span>|<span data-ttu-id="c07cb-357">Gibt an, ob Sprachunterstützung im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-357">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-358">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="c07cb-358">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="c07cb-359">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-359">Boolean</span></span>|<span data-ttu-id="c07cb-360">Gibt an, ob Zugriff auf die Einstellungen der Touch-Unterstützung im Kiosk-Modus gewährt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-360">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-361">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="c07cb-361">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="c07cb-362">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-362">Boolean</span></span>|<span data-ttu-id="c07cb-363">Gibt an, ob die automatische Gerätesperre im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-363">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-364">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="c07cb-364">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="c07cb-365">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-365">Boolean</span></span>|<span data-ttu-id="c07cb-366">Gibt ab, ob der Zugriff auf die Farbinversionseinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-366">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-367">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="c07cb-367">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="c07cb-368">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-368">Boolean</span></span>|<span data-ttu-id="c07cb-369">Gibt ab, ob die Verwendung des Ruftonschalters im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-369">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-370">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="c07cb-370">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="c07cb-371">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-371">Boolean</span></span>|<span data-ttu-id="c07cb-372">Gibt ab, ob die Bildschirmdrehung im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-372">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-373">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="c07cb-373">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="c07cb-374">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-374">Boolean</span></span>|<span data-ttu-id="c07cb-375">Gibt ab, ob die Verwendung der Energiespartaste im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-375">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-376">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="c07cb-376">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="c07cb-377">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-377">Boolean</span></span>|<span data-ttu-id="c07cb-378">Gibt ab, ob die Verwendung des Touchscreens im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-378">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-379">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="c07cb-379">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="c07cb-380">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-380">Boolean</span></span>|<span data-ttu-id="c07cb-381">Gibt ab, ob der Zugriff auf die Einstellungen für Hintergrundkommentare im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-381">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-382">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="c07cb-382">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="c07cb-383">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-383">Boolean</span></span>|<span data-ttu-id="c07cb-384">Gibt ab, ob die Verwendung der Lautstärketasten im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-384">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-385">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="c07cb-385">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="c07cb-386">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-386">Boolean</span></span>|<span data-ttu-id="c07cb-387">Gibt ab, ob der Zugriff auf die Zoomeinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-387">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-388">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c07cb-388">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="c07cb-389">String</span><span class="sxs-lookup"><span data-stu-id="c07cb-389">String</span></span>|<span data-ttu-id="c07cb-390">URL im App Store zu der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-390">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="c07cb-391">Verwenden Sie diese, wenn „KioskModeManagedAppId“ nicht bekannt ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-391">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="c07cb-392">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="c07cb-392">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="c07cb-393">String</span><span class="sxs-lookup"><span data-stu-id="c07cb-393">String</span></span>|<span data-ttu-id="c07cb-394">ID für integrierte apps im Kioskmodus verwenden.</span><span class="sxs-lookup"><span data-stu-id="c07cb-394">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="c07cb-395">Verwendet, wenn KioskModeManagedAppId und KioskModeAppStoreUrl nicht festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="c07cb-395">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="c07cb-396">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="c07cb-396">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="c07cb-397">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-397">Boolean</span></span>|<span data-ttu-id="c07cb-398">Gibt an, ob Touch-Unterstützung im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-398">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-399">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="c07cb-399">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="c07cb-400">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-400">Boolean</span></span>|<span data-ttu-id="c07cb-401">Gibt ab, ob die Farbinversion im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-401">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-402">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="c07cb-402">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="c07cb-403">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-403">Boolean</span></span>|<span data-ttu-id="c07cb-404">Gibt ab, ob Mono-Audio im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-404">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-405">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="c07cb-405">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="c07cb-406">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-406">Boolean</span></span>|<span data-ttu-id="c07cb-407">Gibt ab, ob Hintergrundkommentare im Kiosk-Modus erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c07cb-407">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-408">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="c07cb-408">kioskModeRequireZoom</span></span>|<span data-ttu-id="c07cb-409">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-409">Boolean</span></span>|<span data-ttu-id="c07cb-410">Gibt ab, ob Zoom im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-410">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="c07cb-411">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="c07cb-411">kioskModeManagedAppId</span></span>|<span data-ttu-id="c07cb-412">String</span><span class="sxs-lookup"><span data-stu-id="c07cb-412">String</span></span>|<span data-ttu-id="c07cb-413">Verwaltete App-ID der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-413">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="c07cb-414">Wenn „KioskModeManagedAppId“ angegeben ist, wird „KioskModeAppStoreUrl“ ignoriert.</span><span class="sxs-lookup"><span data-stu-id="c07cb-414">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="c07cb-415">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="c07cb-415">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="c07cb-416">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-416">Boolean</span></span>|<span data-ttu-id="c07cb-417">Gibt an, ob verhindert werden soll, dass der Benutzer das Kontrollzentrum für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-417">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="c07cb-418">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="c07cb-418">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="c07cb-419">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-419">Boolean</span></span>|<span data-ttu-id="c07cb-420">Gibt an, ob verhindert werden soll, dass der Benutzer die Benachrichtigungsansicht auf dem Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-420">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="c07cb-421">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="c07cb-421">lockScreenBlockPassbook</span></span>|<span data-ttu-id="c07cb-422">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-422">Boolean</span></span>|<span data-ttu-id="c07cb-423">Gibt an, ob verhindert werden soll, dass der Benutzer Passbook verwendet, wenn das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-423">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="c07cb-424">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="c07cb-424">lockScreenBlockTodayView</span></span>|<span data-ttu-id="c07cb-425">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-425">Boolean</span></span>|<span data-ttu-id="c07cb-426">Gibt an, ob verhindert werden soll, dass der Benutzer die Ansicht „Heute“ für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-426">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="c07cb-427">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="c07cb-427">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="c07cb-428">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="c07cb-428">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="c07cb-429">Einstellungen für Medieninhalte für Australien</span><span class="sxs-lookup"><span data-stu-id="c07cb-429">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="c07cb-430">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="c07cb-430">mediaContentRatingCanada</span></span>|[<span data-ttu-id="c07cb-431">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="c07cb-431">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="c07cb-432">Einstellungen für Medieninhalte für Kanada</span><span class="sxs-lookup"><span data-stu-id="c07cb-432">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="c07cb-433">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="c07cb-433">mediaContentRatingFrance</span></span>|[<span data-ttu-id="c07cb-434">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="c07cb-434">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="c07cb-435">Einstellungen für Medieninhalte für Frankreich</span><span class="sxs-lookup"><span data-stu-id="c07cb-435">Media content rating settings for France</span></span>|
|<span data-ttu-id="c07cb-436">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="c07cb-436">mediaContentRatingGermany</span></span>|[<span data-ttu-id="c07cb-437">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="c07cb-437">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="c07cb-438">Einstellungen für Medieninhalte für Deutschland</span><span class="sxs-lookup"><span data-stu-id="c07cb-438">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="c07cb-439">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="c07cb-439">mediaContentRatingIreland</span></span>|[<span data-ttu-id="c07cb-440">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="c07cb-440">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="c07cb-441">Einstellungen für Medieninhalte für Irland</span><span class="sxs-lookup"><span data-stu-id="c07cb-441">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="c07cb-442">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="c07cb-442">mediaContentRatingJapan</span></span>|[<span data-ttu-id="c07cb-443">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="c07cb-443">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="c07cb-444">Einstellungen für Medieninhalte für Japan</span><span class="sxs-lookup"><span data-stu-id="c07cb-444">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="c07cb-445">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="c07cb-445">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="c07cb-446">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="c07cb-446">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="c07cb-447">Einstellungen für Medieninhalte für Neuseeland</span><span class="sxs-lookup"><span data-stu-id="c07cb-447">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="c07cb-448">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="c07cb-448">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="c07cb-449">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="c07cb-449">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="c07cb-450">Einstellungen für Medieninhalte für das Vereinigte Königreich</span><span class="sxs-lookup"><span data-stu-id="c07cb-450">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="c07cb-451">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="c07cb-451">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="c07cb-452">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="c07cb-452">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="c07cb-453">Einstellungen für Medieninhalte für die USA</span><span class="sxs-lookup"><span data-stu-id="c07cb-453">Media content rating settings for United States</span></span>|
|<span data-ttu-id="c07cb-454">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="c07cb-454">networkUsageRules</span></span>|<span data-ttu-id="c07cb-455">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c07cb-455">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="c07cb-456">Liste verwalteter Apps und die Netzwerkregeln, die darauf angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="c07cb-456">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="c07cb-457">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c07cb-457">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="c07cb-458">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="c07cb-458">mediaContentRatingApps</span></span>|[<span data-ttu-id="c07cb-459">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="c07cb-459">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="c07cb-460">Media content Bewertung Einstellungen für Apps.</span><span class="sxs-lookup"><span data-stu-id="c07cb-460">Media content rating settings for Apps.</span></span> <span data-ttu-id="c07cb-461">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12` und `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="c07cb-461">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="c07cb-462">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-462">messagesBlocked</span></span>|<span data-ttu-id="c07cb-463">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-463">Boolean</span></span>|<span data-ttu-id="c07cb-464">Gibt an, ob verhindert werden soll, dass der Benutzer die Nachrichten-App auf dem überwachten Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-464">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="c07cb-465">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="c07cb-465">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="c07cb-466">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-466">Boolean</span></span>|<span data-ttu-id="c07cb-467">Gibt an, ob die Änderung von Benachrichtigungseinstellungen zugelassen wird (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-467">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="c07cb-468">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c07cb-468">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="c07cb-469">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-469">Boolean</span></span>|<span data-ttu-id="c07cb-470">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-470">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c07cb-471">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="c07cb-471">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="c07cb-472">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-472">Boolean</span></span>|<span data-ttu-id="c07cb-473">Blockiert das Ändern registrierter Touch ID-Fingerabdrücke im überwachten Modus.</span><span class="sxs-lookup"><span data-stu-id="c07cb-473">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="c07cb-474">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="c07cb-474">passcodeBlockModification</span></span>|<span data-ttu-id="c07cb-475">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-475">Boolean</span></span>|<span data-ttu-id="c07cb-476">Gibt an, ob das Ändern der Kennung auf dem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-476">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c07cb-477">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c07cb-477">passcodeBlockSimple</span></span>|<span data-ttu-id="c07cb-478">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-478">Boolean</span></span>|<span data-ttu-id="c07cb-479">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="c07cb-479">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="c07cb-480">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c07cb-480">passcodeExpirationDays</span></span>|<span data-ttu-id="c07cb-481">Int32</span><span class="sxs-lookup"><span data-stu-id="c07cb-481">Int32</span></span>|<span data-ttu-id="c07cb-482">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="c07cb-482">Number of days before the passcode expires.</span></span> <span data-ttu-id="c07cb-483">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="c07cb-483">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="c07cb-484">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c07cb-484">passcodeMinimumLength</span></span>|<span data-ttu-id="c07cb-485">Int32</span><span class="sxs-lookup"><span data-stu-id="c07cb-485">Int32</span></span>|<span data-ttu-id="c07cb-486">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="c07cb-486">Minimum length of passcode.</span></span> <span data-ttu-id="c07cb-487">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="c07cb-487">Valid values 4 to 14</span></span>|
|<span data-ttu-id="c07cb-488">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c07cb-488">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c07cb-489">Int32</span><span class="sxs-lookup"><span data-stu-id="c07cb-489">Int32</span></span>|<span data-ttu-id="c07cb-490">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-490">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="c07cb-491">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c07cb-491">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c07cb-492">Int32</span><span class="sxs-lookup"><span data-stu-id="c07cb-492">Int32</span></span>|<span data-ttu-id="c07cb-493">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="c07cb-493">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c07cb-494">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c07cb-494">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="c07cb-495">Int32</span><span class="sxs-lookup"><span data-stu-id="c07cb-495">Int32</span></span>|<span data-ttu-id="c07cb-496">Anzahl von Zeichensätzen, die eine Kennung enthalten muss</span><span class="sxs-lookup"><span data-stu-id="c07cb-496">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="c07cb-497">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="c07cb-497">Valid values 0 to 4</span></span>|
|<span data-ttu-id="c07cb-498">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="c07cb-498">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="c07cb-499">Int32</span><span class="sxs-lookup"><span data-stu-id="c07cb-499">Int32</span></span>|<span data-ttu-id="c07cb-500">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="c07cb-500">Number of previous passcodes to block.</span></span> <span data-ttu-id="c07cb-501">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="c07cb-501">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c07cb-502">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="c07cb-502">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="c07cb-503">Int32</span><span class="sxs-lookup"><span data-stu-id="c07cb-503">Int32</span></span>|<span data-ttu-id="c07cb-504">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung des Geräts durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c07cb-504">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="c07cb-505">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="c07cb-505">Valid values 4 to 11</span></span>|
|<span data-ttu-id="c07cb-506">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="c07cb-506">passcodeRequiredType</span></span>|[<span data-ttu-id="c07cb-507">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c07cb-507">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c07cb-508">Geforderter Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="c07cb-508">Type of passcode that is required.</span></span> <span data-ttu-id="c07cb-509">Mögliche Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="c07cb-509">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c07cb-510">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="c07cb-510">passcodeRequired</span></span>|<span data-ttu-id="c07cb-511">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-511">Boolean</span></span>|<span data-ttu-id="c07cb-512">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-512">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="c07cb-513">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-513">podcastsBlocked</span></span>|<span data-ttu-id="c07cb-514">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-514">Boolean</span></span>|<span data-ttu-id="c07cb-515">Gibt an, ob verhindert werden soll, dass der Benutzer Podcasts auf dem überwachten Gerät verwendet (iOS 8.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-515">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="c07cb-516">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="c07cb-516">safariBlockAutofill</span></span>|<span data-ttu-id="c07cb-517">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-517">Boolean</span></span>|<span data-ttu-id="c07cb-518">Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-518">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="c07cb-519">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="c07cb-519">safariBlockJavaScript</span></span>|<span data-ttu-id="c07cb-520">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-520">Boolean</span></span>|<span data-ttu-id="c07cb-521">Gibt an, ob JavaScript in Safari blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-521">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="c07cb-522">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="c07cb-522">safariBlockPopups</span></span>|<span data-ttu-id="c07cb-523">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-523">Boolean</span></span>|<span data-ttu-id="c07cb-524">Gibt an, ob Popups in Safari blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c07cb-524">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="c07cb-525">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-525">safariBlocked</span></span>|<span data-ttu-id="c07cb-526">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-526">Boolean</span></span>|<span data-ttu-id="c07cb-527">Gibt an, ob verhindert werden soll, dass der Benutzer Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-527">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="c07cb-528">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="c07cb-528">safariCookieSettings</span></span>|[<span data-ttu-id="c07cb-529">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="c07cb-529">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="c07cb-530">Cokkieeinstellungen für Safari.</span><span class="sxs-lookup"><span data-stu-id="c07cb-530">Cookie settings for Safari.</span></span> <span data-ttu-id="c07cb-531">Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="c07cb-531">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="c07cb-532">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="c07cb-532">safariManagedDomains</span></span>|<span data-ttu-id="c07cb-533">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c07cb-533">String collection</span></span>|<span data-ttu-id="c07cb-534">URLs, die mit den hier aufgeführten Mustern übereinstimmen, werden als verwaltet betrachtet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-534">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="c07cb-535">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="c07cb-535">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="c07cb-536">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c07cb-536">String collection</span></span>|<span data-ttu-id="c07cb-537">Benutzer können Kennwörter in Safari nur von URLs speichern, die mit den hier aufgeführten Mustern übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="c07cb-537">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="c07cb-538">Gilt für Geräte im überwachten Modus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="c07cb-538">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="c07cb-539">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="c07cb-539">safariRequireFraudWarning</span></span>|<span data-ttu-id="c07cb-540">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-540">Boolean</span></span>|<span data-ttu-id="c07cb-541">Gibt an, ob eine Betrugswarnung in Safari erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-541">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="c07cb-542">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-542">screenCaptureBlocked</span></span>|<span data-ttu-id="c07cb-543">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-543">Boolean</span></span>|<span data-ttu-id="c07cb-544">Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.</span><span class="sxs-lookup"><span data-stu-id="c07cb-544">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="c07cb-545">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-545">siriBlocked</span></span>|<span data-ttu-id="c07cb-546">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-546">Boolean</span></span>|<span data-ttu-id="c07cb-547">Gibt an, ob verhindert werden soll, dass der Benutzer Siri verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-547">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="c07cb-548">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-548">siriBlockedWhenLocked</span></span>|<span data-ttu-id="c07cb-549">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-549">Boolean</span></span>|<span data-ttu-id="c07cb-550">Gibt an, ob verhindert werden soll, dass der Benutzer Siri bei Sperrung verwendet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-550">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="c07cb-551">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="c07cb-551">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="c07cb-552">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-552">Boolean</span></span>|<span data-ttu-id="c07cb-553">Gibt an, ob Siri bei Verwendung auf einem überwachten Gerät davon abgehalten werden soll, benutzergenerierte Inhalte abzufragen.</span><span class="sxs-lookup"><span data-stu-id="c07cb-553">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="c07cb-554">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="c07cb-554">siriRequireProfanityFilter</span></span>|<span data-ttu-id="c07cb-555">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-555">Boolean</span></span>|<span data-ttu-id="c07cb-556">Gibt an, ob verhindert werden soll, dass Siri anstößige Ausdrücke auf dem überwachten Gerät diktiert oder spricht.</span><span class="sxs-lookup"><span data-stu-id="c07cb-556">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="c07cb-557">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="c07cb-557">spotlightBlockInternetResults</span></span>|<span data-ttu-id="c07cb-558">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-558">Boolean</span></span>|<span data-ttu-id="c07cb-559">Gibt an, ob verhindert werden soll, dass die Spotlight-Suche Internetergebnisse auf dem überwachten Gerät zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="c07cb-559">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="c07cb-560">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="c07cb-560">voiceDialingBlocked</span></span>|<span data-ttu-id="c07cb-561">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-561">Boolean</span></span>|<span data-ttu-id="c07cb-562">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c07cb-562">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="c07cb-563">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="c07cb-563">wallpaperBlockModification</span></span>|<span data-ttu-id="c07cb-564">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-564">Boolean</span></span>|<span data-ttu-id="c07cb-565">Gibt an, ob das Ändern des Hintergrunds auf einem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="c07cb-565">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="c07cb-566">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="c07cb-566">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="c07cb-567">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c07cb-567">Boolean</span></span>|<span data-ttu-id="c07cb-568">Gibt an, ob erzwungen werden soll, dass das Gerät nur WLAN-Netzwerke aus Konfigurationsprofilen verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="c07cb-568">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="c07cb-569">Antwort</span><span class="sxs-lookup"><span data-stu-id="c07cb-569">Response</span></span>
<span data-ttu-id="c07cb-570">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c07cb-570">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c07cb-571">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c07cb-571">Example</span></span>
### <a name="request"></a><span data-ttu-id="c07cb-572">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c07cb-572">Request</span></span>
<span data-ttu-id="c07cb-573">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c07cb-573">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

### <a name="response"></a><span data-ttu-id="c07cb-574">Antwort</span><span class="sxs-lookup"><span data-stu-id="c07cb-574">Response</span></span>
<span data-ttu-id="c07cb-p127">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c07cb-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8013

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```


