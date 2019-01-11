---
title: iosGeneralDeviceConfiguration aktualisieren
description: Aktualisiert die Eigenschaften eines iosDeviceFeaturesConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8c4aa2af2946c7e99d8a17b3bc98a688b10efd04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854019"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="b96ef-103">iosGeneralDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b96ef-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="b96ef-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b96ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b96ef-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b96ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b96ef-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b96ef-107">Aktualisiert die Eigenschaften eines [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b96ef-107">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b96ef-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b96ef-108">Prerequisites</span></span>
<span data-ttu-id="b96ef-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b96ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b96ef-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b96ef-111">Permission type</span></span>|<span data-ttu-id="b96ef-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b96ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b96ef-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b96ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b96ef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b96ef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b96ef-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b96ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b96ef-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b96ef-116">Not supported.</span></span>|
|<span data-ttu-id="b96ef-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b96ef-117">Application</span></span>|<span data-ttu-id="b96ef-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b96ef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b96ef-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b96ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b96ef-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b96ef-120">Request headers</span></span>
|<span data-ttu-id="b96ef-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b96ef-121">Header</span></span>|<span data-ttu-id="b96ef-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b96ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b96ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b96ef-123">Authorization</span></span>|<span data-ttu-id="b96ef-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b96ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b96ef-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b96ef-125">Accept</span></span>|<span data-ttu-id="b96ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b96ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b96ef-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b96ef-127">Request body</span></span>
<span data-ttu-id="b96ef-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b96ef-128">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="b96ef-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b96ef-129">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="b96ef-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b96ef-130">Property</span></span>|<span data-ttu-id="b96ef-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b96ef-131">Type</span></span>|<span data-ttu-id="b96ef-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b96ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b96ef-133">id</span><span class="sxs-lookup"><span data-stu-id="b96ef-133">id</span></span>|<span data-ttu-id="b96ef-134">String</span><span class="sxs-lookup"><span data-stu-id="b96ef-134">String</span></span>|<span data-ttu-id="b96ef-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b96ef-135">Key of the entity.</span></span> <span data-ttu-id="b96ef-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b96ef-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b96ef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b96ef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b96ef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b96ef-138">DateTimeOffset</span></span>|<span data-ttu-id="b96ef-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b96ef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b96ef-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b96ef-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b96ef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b96ef-141">roleScopeTagIds</span></span>|<span data-ttu-id="b96ef-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b96ef-142">String collection</span></span>|<span data-ttu-id="b96ef-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b96ef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b96ef-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b96ef-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b96ef-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b96ef-145">supportsScopeTags</span></span>|<span data-ttu-id="b96ef-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-146">Boolean</span></span>|<span data-ttu-id="b96ef-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b96ef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b96ef-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b96ef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b96ef-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b96ef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b96ef-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b96ef-150">This property is read-only.</span></span> <span data-ttu-id="b96ef-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b96ef-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b96ef-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b96ef-152">createdDateTime</span></span>|<span data-ttu-id="b96ef-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b96ef-153">DateTimeOffset</span></span>|<span data-ttu-id="b96ef-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b96ef-154">DateTime the object was created.</span></span> <span data-ttu-id="b96ef-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b96ef-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b96ef-156">description</span><span class="sxs-lookup"><span data-stu-id="b96ef-156">description</span></span>|<span data-ttu-id="b96ef-157">String</span><span class="sxs-lookup"><span data-stu-id="b96ef-157">String</span></span>|<span data-ttu-id="b96ef-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b96ef-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b96ef-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b96ef-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b96ef-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b96ef-160">displayName</span></span>|<span data-ttu-id="b96ef-161">String</span><span class="sxs-lookup"><span data-stu-id="b96ef-161">String</span></span>|<span data-ttu-id="b96ef-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b96ef-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b96ef-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b96ef-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b96ef-164">Version</span><span class="sxs-lookup"><span data-stu-id="b96ef-164">version</span></span>|<span data-ttu-id="b96ef-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b96ef-165">Int32</span></span>|<span data-ttu-id="b96ef-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b96ef-166">Version of the device configuration.</span></span> <span data-ttu-id="b96ef-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b96ef-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b96ef-168">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="b96ef-168">accountBlockModification</span></span>|<span data-ttu-id="b96ef-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-169">Boolean</span></span>|<span data-ttu-id="b96ef-170">Gibt an, ob die Kontoänderung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-170">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-171">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="b96ef-171">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="b96ef-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-172">Boolean</span></span>|<span data-ttu-id="b96ef-173">Gibt an, ob die Aktivierungssperre zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-173">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="b96ef-174">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-174">airDropBlocked</span></span>|<span data-ttu-id="b96ef-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-175">Boolean</span></span>|<span data-ttu-id="b96ef-176">Gibt an, ob AirDrop zugelassen wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-176">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-177">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="b96ef-177">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="b96ef-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-178">Boolean</span></span>|<span data-ttu-id="b96ef-179">Gibt an, ob AirDrop als nicht verwaltetes Drop-Ziel (iOS 9.0 oder höher) betrachtet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-179">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b96ef-180">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="b96ef-180">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="b96ef-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-181">Boolean</span></span>|<span data-ttu-id="b96ef-182">Gibt an, ob erzwungen werden soll, dass alle Geräte, die AirPlay-Anforderungen von diesem Gerät erhalten, ein Kopplungskennwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="b96ef-182">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="b96ef-183">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="b96ef-183">appleWatchBlockPairing</span></span>|<span data-ttu-id="b96ef-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-184">Boolean</span></span>|<span data-ttu-id="b96ef-185">Gibt an, ob eine Apple Watch-Kopplung zulässig ist, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-185">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b96ef-186">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="b96ef-186">appleWatchForceWristDetection</span></span>|<span data-ttu-id="b96ef-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-187">Boolean</span></span>|<span data-ttu-id="b96ef-188">Gibt an, ob erzwungen werden soll, dass eine gekoppelte Apple Watch die Handgelenkerkennung (iOS 8.2 und höher) verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-188">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="b96ef-189">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-189">appleNewsBlocked</span></span>|<span data-ttu-id="b96ef-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-190">Boolean</span></span>|<span data-ttu-id="b96ef-191">Gibt an, ob verhindert werden soll, dass der Benutzer News verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-191">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b96ef-192">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="b96ef-192">appsSingleAppModeList</span></span>|<span data-ttu-id="b96ef-193">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b96ef-193">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b96ef-194">Ruft die Liste von iOS-Apps ab, die autonom in den Einzelanwendungsmodus wechseln können, ab oder legt diese fest.</span><span class="sxs-lookup"><span data-stu-id="b96ef-194">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="b96ef-195">Nur überwacht.</span><span class="sxs-lookup"><span data-stu-id="b96ef-195">Supervised only.</span></span> <span data-ttu-id="b96ef-196">iOS 7.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="b96ef-196">iOS 7.0 and later.</span></span> <span data-ttu-id="b96ef-197">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b96ef-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b96ef-198">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="b96ef-198">appsVisibilityList</span></span>|<span data-ttu-id="b96ef-199">[appListItem](../resources/intune-deviceconfig-applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b96ef-199">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b96ef-200">Liste von Apps in der Sichtbarkeitsliste (entweder eine Liste sichtbarer/startbarer Apps oder eine Liste ausgeblendeter/nicht startbarer Apps, gesteuert von AppsVisibilityListType) (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-200">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="b96ef-201">Diese Sammlung darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b96ef-201">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b96ef-202">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="b96ef-202">appsVisibilityListType</span></span>|[<span data-ttu-id="b96ef-203">appListType</span><span class="sxs-lookup"><span data-stu-id="b96ef-203">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b96ef-204">Typ der in „AppsVisibilityList“ enthaltenen Liste.</span><span class="sxs-lookup"><span data-stu-id="b96ef-204">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="b96ef-205">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="b96ef-205">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b96ef-206">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="b96ef-206">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="b96ef-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-207">Boolean</span></span>|<span data-ttu-id="b96ef-208">Gibt an, ob das automatische Herunterladen von Apps blockiert werden soll, die auf anderen Geräten gekauft wurden, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 oder höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-208">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b96ef-209">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-209">appStoreBlocked</span></span>|<span data-ttu-id="b96ef-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-210">Boolean</span></span>|<span data-ttu-id="b96ef-211">Gibt an, ob verhindert werden soll, dass der Benutzer den App Store verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-211">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="b96ef-212">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="b96ef-212">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="b96ef-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-213">Boolean</span></span>|<span data-ttu-id="b96ef-214">Gibt an, ob verhindert werden soll, dass der Benutzer In-App-Käufe tätigt.</span><span class="sxs-lookup"><span data-stu-id="b96ef-214">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="b96ef-215">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b96ef-215">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="b96ef-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-216">Boolean</span></span>|<span data-ttu-id="b96ef-217">Gibt an, ob die App Store-App blockiert werden soll, ohne die Installation über Host-Apps einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="b96ef-217">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="b96ef-218">Gilt nur für den überwachten Modus (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-218">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b96ef-219">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="b96ef-219">appStoreRequirePassword</span></span>|<span data-ttu-id="b96ef-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-220">Boolean</span></span>|<span data-ttu-id="b96ef-221">Gibt an, ob bei Verwendung des App Stores ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-221">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="b96ef-222">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="b96ef-222">bluetoothBlockModification</span></span>|<span data-ttu-id="b96ef-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-223">Boolean</span></span>|<span data-ttu-id="b96ef-224">Gibt an, ob das Ändern von Bluetooth-Einstellungen zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 10.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-224">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="b96ef-225">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-225">cameraBlocked</span></span>|<span data-ttu-id="b96ef-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-226">Boolean</span></span>|<span data-ttu-id="b96ef-227">Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.</span><span class="sxs-lookup"><span data-stu-id="b96ef-227">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="b96ef-228">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="b96ef-228">cellularBlockDataRoaming</span></span>|<span data-ttu-id="b96ef-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-229">Boolean</span></span>|<span data-ttu-id="b96ef-230">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-230">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="b96ef-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="b96ef-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="b96ef-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-232">Boolean</span></span>|<span data-ttu-id="b96ef-233">Gibt an, ob das globales Abrufen im Hintergrund beim Roaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-233">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="b96ef-234">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="b96ef-234">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="b96ef-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-235">Boolean</span></span>|<span data-ttu-id="b96ef-236">Gibt an, ob Änderungen an den Mobil-App-Daten zulässig sind, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-236">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-237">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="b96ef-237">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="b96ef-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-238">Boolean</span></span>|<span data-ttu-id="b96ef-239">Gibt an, ob der privater Hotspot blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-239">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="b96ef-240">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="b96ef-240">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="b96ef-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-241">Boolean</span></span>|<span data-ttu-id="b96ef-242">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-242">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="b96ef-243">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="b96ef-243">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="b96ef-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-244">Boolean</span></span>|<span data-ttu-id="b96ef-245">Gibt an, ob nicht vertrauenswürdige TLS-Zertifikate blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b96ef-245">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="b96ef-246">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b96ef-246">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="b96ef-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-247">Boolean</span></span>|<span data-ttu-id="b96ef-248">Gibt an, ob die Remotebildschirmüberwachung über die Classroom-App zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-248">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b96ef-249">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b96ef-249">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="b96ef-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-250">Boolean</span></span>|<span data-ttu-id="b96ef-251">Gibt an, ob dem Lehrer eines verwalteten Kurses in der Classroom-App automatisch die Berechtigung erteilt werden soll, den Bildschirm eines Kursteilnehmers ohne Aufforderung anzuzeigen, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-251">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-252">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="b96ef-252">compliantAppsList</span></span>|<span data-ttu-id="b96ef-253">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b96ef-253">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b96ef-254">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="b96ef-254">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="b96ef-255">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b96ef-255">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b96ef-256">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="b96ef-256">compliantAppListType</span></span>|[<span data-ttu-id="b96ef-257">appListType</span><span class="sxs-lookup"><span data-stu-id="b96ef-257">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b96ef-258">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="b96ef-258">List that is in the AppComplianceList.</span></span> <span data-ttu-id="b96ef-259">Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="b96ef-259">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b96ef-260">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="b96ef-260">configurationProfileBlockChanges</span></span>|<span data-ttu-id="b96ef-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-261">Boolean</span></span>|<span data-ttu-id="b96ef-262">Gibt an, ob verhindert werden soll, dass der Benutzer Konfigurationsprofile und Zertifikate interaktiv installiert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-262">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-263">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-263">definitionLookupBlocked</span></span>|<span data-ttu-id="b96ef-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-264">Boolean</span></span>|<span data-ttu-id="b96ef-265">Gibt an, ob die Definitionssuche zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-265">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="b96ef-266">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="b96ef-266">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="b96ef-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-267">Boolean</span></span>|<span data-ttu-id="b96ef-268">Gibt an, ob erlaubt werden soll, dass der Benutzer Einschränkungen in den Geräteeinstellungen aktiviert, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-268">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-269">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="b96ef-269">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="b96ef-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-270">Boolean</span></span>|<span data-ttu-id="b96ef-271">Gibt an, ob die Verwendung der Option zum Löschen aller Inhalte und Einstellungen auf dem Gerät zugelassen werden soll, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-271">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-272">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="b96ef-272">deviceBlockNameModification</span></span>|<span data-ttu-id="b96ef-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-273">Boolean</span></span>|<span data-ttu-id="b96ef-274">Gibt an, ob das Ändern des Gerätenamens zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-274">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b96ef-275">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="b96ef-275">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="b96ef-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-276">Boolean</span></span>|<span data-ttu-id="b96ef-277">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-277">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b96ef-278">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="b96ef-278">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="b96ef-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-279">Boolean</span></span>|<span data-ttu-id="b96ef-280">Gibt an, ob das Ändern der Einstellungen für die Diagnoseübermittlung zugelassen wird, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3.2 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-280">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="b96ef-281">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="b96ef-281">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="b96ef-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-282">Boolean</span></span>|<span data-ttu-id="b96ef-283">Gibt an, ob verhindert werden soll, dass der Benutzer verwaltete Dokumente in nicht verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="b96ef-283">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="b96ef-284">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="b96ef-284">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="b96ef-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-285">Boolean</span></span>|<span data-ttu-id="b96ef-286">Gibt an, ob verhindert werden soll, dass der Benutzer nicht verwaltete Dokumente in verwalteten Apps anzeigt.</span><span class="sxs-lookup"><span data-stu-id="b96ef-286">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="b96ef-287">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="b96ef-287">emailInDomainSuffixes</span></span>|<span data-ttu-id="b96ef-288">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b96ef-288">String collection</span></span>|<span data-ttu-id="b96ef-289">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="b96ef-289">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="b96ef-290">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="b96ef-290">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="b96ef-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-291">Boolean</span></span>|<span data-ttu-id="b96ef-292">Gibt an, ob verhindert werden soll, dass der Benutzer einer Unternehmens-App vertraut.</span><span class="sxs-lookup"><span data-stu-id="b96ef-292">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="b96ef-293">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="b96ef-293">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="b96ef-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-294">Boolean</span></span>|<span data-ttu-id="b96ef-295">Gibt an, ob verhindert werden soll, dass der Benutzer die Vertrauensstellungseinstellungen der Unternehmens-App ändert.</span><span class="sxs-lookup"><span data-stu-id="b96ef-295">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="b96ef-296">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-296">faceTimeBlocked</span></span>|<span data-ttu-id="b96ef-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-297">Boolean</span></span>|<span data-ttu-id="b96ef-298">Gibt an, ob verhindert werden soll, dass der Benutzer FaceTime verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-298">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="b96ef-299">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-299">findMyFriendsBlocked</span></span>|<span data-ttu-id="b96ef-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-300">Boolean</span></span>|<span data-ttu-id="b96ef-301">Gibt an, ob „Freunde suchen“ blockiert wird, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-301">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-302">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="b96ef-302">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="b96ef-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-303">Boolean</span></span>|<span data-ttu-id="b96ef-304">Gibt an, ob verhindert werden soll, dass der Benutzer Freunde im Game Center hat.</span><span class="sxs-lookup"><span data-stu-id="b96ef-304">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="b96ef-305">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="b96ef-305">gamingBlockMultiplayer</span></span>|<span data-ttu-id="b96ef-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-306">Boolean</span></span>|<span data-ttu-id="b96ef-307">Gibt an, ob verhindert werden soll, dass der Benutzer Multiplayerspiele verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-307">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="b96ef-308">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-308">gameCenterBlocked</span></span>|<span data-ttu-id="b96ef-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-309">Boolean</span></span>|<span data-ttu-id="b96ef-310">Gibt an, ob verhindert werden soll, dass der Benutzer Game Center verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-310">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-311">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-311">hostPairingBlocked</span></span>|<span data-ttu-id="b96ef-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-312">Boolean</span></span>|<span data-ttu-id="b96ef-313">Gibt an, ob die Hostkopplung blockiert werden soll, um zu steuern, mit welchen Geräten ein iOS-Gerät gekoppelt werden kann,wenn sich das iOS-Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-313">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-314">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-314">iBooksStoreBlocked</span></span>|<span data-ttu-id="b96ef-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-315">Boolean</span></span>|<span data-ttu-id="b96ef-316">Gibt an, ob verhindert werden soll, dass der Benutzer den iBooks Store verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-316">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-317">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="b96ef-317">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="b96ef-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-318">Boolean</span></span>|<span data-ttu-id="b96ef-319">Gibt an, ob verhindert werden soll, dass der Benutzer Medien aus dem iBook Store herunterlädt, die als Erotik gekennzeichnet sind.</span><span class="sxs-lookup"><span data-stu-id="b96ef-319">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="b96ef-320">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="b96ef-320">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="b96ef-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-321">Boolean</span></span>|<span data-ttu-id="b96ef-322">Gibt an, ob verhindert werden soll, dass der Benutzer eine Aufgabe, die er auf dem iOS-Gerät begonnen hat, auf einem anderen iOS- oder macOS-Gerät fortsetzt.</span><span class="sxs-lookup"><span data-stu-id="b96ef-322">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="b96ef-323">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="b96ef-323">iCloudBlockBackup</span></span>|<span data-ttu-id="b96ef-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-324">Boolean</span></span>|<span data-ttu-id="b96ef-325">Gibt an, ob die iCloud-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-325">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="b96ef-326">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="b96ef-326">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="b96ef-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-327">Boolean</span></span>|<span data-ttu-id="b96ef-328">Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-328">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="b96ef-329">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="b96ef-329">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="b96ef-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-330">Boolean</span></span>|<span data-ttu-id="b96ef-331">Gibt an, ob die Cloudsynchronisierung für verwaltete Apps blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-331">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="b96ef-332">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="b96ef-332">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="b96ef-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-333">Boolean</span></span>|<span data-ttu-id="b96ef-334">Gibt an, ob die iCloud-Fotomediathek blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-334">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="b96ef-335">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="b96ef-335">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="b96ef-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-336">Boolean</span></span>|<span data-ttu-id="b96ef-337">Gibt an, ob die Fotostream-Synchronisierung in iCloud blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-337">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="b96ef-338">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="b96ef-338">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="b96ef-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-339">Boolean</span></span>|<span data-ttu-id="b96ef-340">Gibt an, ob die Fotofreigabe blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-340">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="b96ef-341">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="b96ef-341">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="b96ef-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-342">Boolean</span></span>|<span data-ttu-id="b96ef-343">Gibt an, ob Sicherungen in iCloud verschlüsselt sein müssen.</span><span class="sxs-lookup"><span data-stu-id="b96ef-343">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="b96ef-344">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="b96ef-344">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="b96ef-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-345">Boolean</span></span>|<span data-ttu-id="b96ef-346">Gibt an, ob verhindert werden soll, dass der Benutzer auf anstößige Inhalte in iTunes und im App Store zugreift. </span><span class="sxs-lookup"><span data-stu-id="b96ef-346">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="b96ef-347">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="b96ef-347">iTunesBlockMusicService</span></span>|<span data-ttu-id="b96ef-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-348">Boolean</span></span>|<span data-ttu-id="b96ef-349">Gibt an, ob der Music-Dienst blockiert und die Music-App in den klassischen Modus zurückgesetzt werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher und Mac OS 10.12 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-349">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="b96ef-350">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="b96ef-350">iTunesBlockRadio</span></span>|<span data-ttu-id="b96ef-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-351">Boolean</span></span>|<span data-ttu-id="b96ef-352">Gibt an, ob verhindert werden soll, dass der Benutzer iTunes Radio verwendet, wenn sich das Gerät im überwachten Modus befindet (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-352">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b96ef-353">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="b96ef-353">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="b96ef-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-354">Boolean</span></span>|<span data-ttu-id="b96ef-355">Gibt an, ob die Autokorrektur der Tastatur blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-355">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b96ef-356">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="b96ef-356">keyboardBlockDictation</span></span>|<span data-ttu-id="b96ef-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-357">Boolean</span></span>|<span data-ttu-id="b96ef-358">Gibt an, ob verhindert werden soll, dass der Benutzer die Diktatfunktion verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-358">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-359">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="b96ef-359">keyboardBlockPredictive</span></span>|<span data-ttu-id="b96ef-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-360">Boolean</span></span>|<span data-ttu-id="b96ef-361">Gibt an, ob Tastaturwortvorschläge blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-361">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b96ef-362">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="b96ef-362">keyboardBlockShortcuts</span></span>|<span data-ttu-id="b96ef-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-363">Boolean</span></span>|<span data-ttu-id="b96ef-364">Gibt an, ob Tastenkombinationen blockiert werden sollen, wenn sich das Gerät im überwachten Modus befindet (iOS 9.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-364">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b96ef-365">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="b96ef-365">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="b96ef-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-366">Boolean</span></span>|<span data-ttu-id="b96ef-367">Gibt an, ob die Rechtschreibprüfung blockiert werden soll, wenn sich das Gerät im überwachten Modus befindet (iOS 8.1.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-367">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b96ef-368">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="b96ef-368">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="b96ef-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-369">Boolean</span></span>|<span data-ttu-id="b96ef-370">Gibt an, ob Sprachunterstützung im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-370">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-371">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="b96ef-371">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="b96ef-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-372">Boolean</span></span>|<span data-ttu-id="b96ef-373">Gibt an, ob Zugriff auf die Einstellungen der Touch-Unterstützung im Kiosk-Modus gewährt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-373">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-374">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="b96ef-374">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="b96ef-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-375">Boolean</span></span>|<span data-ttu-id="b96ef-376">Gibt an, ob die automatische Gerätesperre im Kiosk-Modus zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-376">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-377">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="b96ef-377">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="b96ef-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-378">Boolean</span></span>|<span data-ttu-id="b96ef-379">Gibt ab, ob der Zugriff auf die Farbinversionseinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-379">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-380">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="b96ef-380">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="b96ef-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-381">Boolean</span></span>|<span data-ttu-id="b96ef-382">Gibt ab, ob die Verwendung des Ruftonschalters im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-382">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-383">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="b96ef-383">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="b96ef-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-384">Boolean</span></span>|<span data-ttu-id="b96ef-385">Gibt ab, ob die Bildschirmdrehung im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-385">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-386">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="b96ef-386">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="b96ef-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-387">Boolean</span></span>|<span data-ttu-id="b96ef-388">Gibt ab, ob die Verwendung der Energiespartaste im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-388">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-389">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="b96ef-389">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="b96ef-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-390">Boolean</span></span>|<span data-ttu-id="b96ef-391">Gibt ab, ob die Verwendung des Touchscreens im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-391">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-392">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="b96ef-392">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="b96ef-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-393">Boolean</span></span>|<span data-ttu-id="b96ef-394">Gibt ab, ob der Zugriff auf die Einstellungen für Hintergrundkommentare im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-394">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-395">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="b96ef-395">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="b96ef-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-396">Boolean</span></span>|<span data-ttu-id="b96ef-397">Gibt ab, ob die Verwendung der Lautstärketasten im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-397">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-398">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="b96ef-398">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="b96ef-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-399">Boolean</span></span>|<span data-ttu-id="b96ef-400">Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b96ef-400">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="b96ef-401">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="b96ef-401">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="b96ef-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-402">Boolean</span></span>|<span data-ttu-id="b96ef-403">Gibt ab, ob der Zugriff auf die Zoomeinstellungen im Kiosk-Modus erlaubt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-403">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-404">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b96ef-404">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="b96ef-405">String</span><span class="sxs-lookup"><span data-stu-id="b96ef-405">String</span></span>|<span data-ttu-id="b96ef-406">URL im App Store zu der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-406">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="b96ef-407">Verwenden Sie diese, wenn „KioskModeManagedAppId“ nicht bekannt ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-407">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="b96ef-408">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="b96ef-408">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="b96ef-409">String</span><span class="sxs-lookup"><span data-stu-id="b96ef-409">String</span></span>|<span data-ttu-id="b96ef-410">ID für integrierte apps im Kioskmodus verwenden.</span><span class="sxs-lookup"><span data-stu-id="b96ef-410">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="b96ef-411">Verwendet, wenn KioskModeManagedAppId und KioskModeAppStoreUrl nicht festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b96ef-411">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="b96ef-412">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="b96ef-412">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="b96ef-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-413">Boolean</span></span>|<span data-ttu-id="b96ef-414">Gibt an, ob Touch-Unterstützung im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-414">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-415">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="b96ef-415">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="b96ef-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-416">Boolean</span></span>|<span data-ttu-id="b96ef-417">Gibt ab, ob die Farbinversion im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-417">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-418">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="b96ef-418">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="b96ef-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-419">Boolean</span></span>|<span data-ttu-id="b96ef-420">Gibt ab, ob Mono-Audio im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-420">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-421">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="b96ef-421">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="b96ef-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-422">Boolean</span></span>|<span data-ttu-id="b96ef-423">Gibt ab, ob Hintergrundkommentare im Kiosk-Modus erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b96ef-423">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-424">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="b96ef-424">kioskModeRequireZoom</span></span>|<span data-ttu-id="b96ef-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-425">Boolean</span></span>|<span data-ttu-id="b96ef-426">Gibt ab, ob Zoom im Kiosk-Modus erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-426">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="b96ef-427">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="b96ef-427">kioskModeManagedAppId</span></span>|<span data-ttu-id="b96ef-428">String</span><span class="sxs-lookup"><span data-stu-id="b96ef-428">String</span></span>|<span data-ttu-id="b96ef-429">Verwaltete App-ID der App, die für den Kiosk-Modus verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-429">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="b96ef-430">Wenn „KioskModeManagedAppId“ angegeben ist, wird „KioskModeAppStoreUrl“ ignoriert.</span><span class="sxs-lookup"><span data-stu-id="b96ef-430">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="b96ef-431">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="b96ef-431">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="b96ef-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-432">Boolean</span></span>|<span data-ttu-id="b96ef-433">Gibt an, ob verhindert werden soll, dass der Benutzer das Kontrollzentrum für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-433">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="b96ef-434">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="b96ef-434">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="b96ef-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-435">Boolean</span></span>|<span data-ttu-id="b96ef-436">Gibt an, ob verhindert werden soll, dass der Benutzer die Benachrichtigungsansicht auf dem Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-436">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="b96ef-437">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="b96ef-437">lockScreenBlockPassbook</span></span>|<span data-ttu-id="b96ef-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-438">Boolean</span></span>|<span data-ttu-id="b96ef-439">Gibt an, ob verhindert werden soll, dass der Benutzer Passbook verwendet, wenn das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-439">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="b96ef-440">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="b96ef-440">lockScreenBlockTodayView</span></span>|<span data-ttu-id="b96ef-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-441">Boolean</span></span>|<span data-ttu-id="b96ef-442">Gibt an, ob verhindert werden soll, dass der Benutzer die Ansicht „Heute“ für den Sperrbildschirm verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-442">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="b96ef-443">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b96ef-443">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="b96ef-444">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b96ef-444">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="b96ef-445">Einstellungen für Medieninhalte für Australien</span><span class="sxs-lookup"><span data-stu-id="b96ef-445">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="b96ef-446">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b96ef-446">mediaContentRatingCanada</span></span>|[<span data-ttu-id="b96ef-447">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b96ef-447">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="b96ef-448">Einstellungen für Medieninhalte für Kanada</span><span class="sxs-lookup"><span data-stu-id="b96ef-448">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="b96ef-449">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b96ef-449">mediaContentRatingFrance</span></span>|[<span data-ttu-id="b96ef-450">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b96ef-450">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="b96ef-451">Einstellungen für Medieninhalte für Frankreich</span><span class="sxs-lookup"><span data-stu-id="b96ef-451">Media content rating settings for France</span></span>|
|<span data-ttu-id="b96ef-452">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b96ef-452">mediaContentRatingGermany</span></span>|[<span data-ttu-id="b96ef-453">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b96ef-453">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="b96ef-454">Einstellungen für Medieninhalte für Deutschland</span><span class="sxs-lookup"><span data-stu-id="b96ef-454">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="b96ef-455">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b96ef-455">mediaContentRatingIreland</span></span>|[<span data-ttu-id="b96ef-456">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b96ef-456">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="b96ef-457">Einstellungen für Medieninhalte für Irland</span><span class="sxs-lookup"><span data-stu-id="b96ef-457">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="b96ef-458">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b96ef-458">mediaContentRatingJapan</span></span>|[<span data-ttu-id="b96ef-459">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b96ef-459">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="b96ef-460">Einstellungen für Medieninhalte für Japan</span><span class="sxs-lookup"><span data-stu-id="b96ef-460">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="b96ef-461">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b96ef-461">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="b96ef-462">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b96ef-462">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="b96ef-463">Einstellungen für Medieninhalte für Neuseeland</span><span class="sxs-lookup"><span data-stu-id="b96ef-463">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="b96ef-464">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b96ef-464">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="b96ef-465">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b96ef-465">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="b96ef-466">Einstellungen für Medieninhalte für das Vereinigte Königreich</span><span class="sxs-lookup"><span data-stu-id="b96ef-466">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="b96ef-467">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b96ef-467">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="b96ef-468">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b96ef-468">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="b96ef-469">Einstellungen für Medieninhalte für die USA</span><span class="sxs-lookup"><span data-stu-id="b96ef-469">Media content rating settings for United States</span></span>|
|<span data-ttu-id="b96ef-470">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="b96ef-470">networkUsageRules</span></span>|<span data-ttu-id="b96ef-471">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b96ef-471">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="b96ef-472">Liste verwalteter Apps und die Netzwerkregeln, die darauf angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="b96ef-472">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="b96ef-473">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b96ef-473">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b96ef-474">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="b96ef-474">mediaContentRatingApps</span></span>|[<span data-ttu-id="b96ef-475">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="b96ef-475">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="b96ef-476">Media content Bewertung Einstellungen für Apps.</span><span class="sxs-lookup"><span data-stu-id="b96ef-476">Media content rating settings for Apps.</span></span> <span data-ttu-id="b96ef-477">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12` und `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="b96ef-477">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="b96ef-478">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-478">messagesBlocked</span></span>|<span data-ttu-id="b96ef-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-479">Boolean</span></span>|<span data-ttu-id="b96ef-480">Gibt an, ob verhindert werden soll, dass der Benutzer die Nachrichten-App auf dem überwachten Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-480">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="b96ef-481">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="b96ef-481">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="b96ef-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-482">Boolean</span></span>|<span data-ttu-id="b96ef-483">Gibt an, ob die Änderung von Benachrichtigungseinstellungen zugelassen wird (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-483">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b96ef-484">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="b96ef-484">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="b96ef-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-485">Boolean</span></span>|<span data-ttu-id="b96ef-486">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-486">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="b96ef-487">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="b96ef-487">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="b96ef-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-488">Boolean</span></span>|<span data-ttu-id="b96ef-489">Blockiert das Ändern registrierter Touch ID-Fingerabdrücke im überwachten Modus.</span><span class="sxs-lookup"><span data-stu-id="b96ef-489">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-490">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="b96ef-490">passcodeBlockModification</span></span>|<span data-ttu-id="b96ef-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-491">Boolean</span></span>|<span data-ttu-id="b96ef-492">Gibt an, ob das Ändern der Kennung auf dem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-492">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b96ef-493">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b96ef-493">passcodeBlockSimple</span></span>|<span data-ttu-id="b96ef-494">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-494">Boolean</span></span>|<span data-ttu-id="b96ef-495">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="b96ef-495">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="b96ef-496">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b96ef-496">passcodeExpirationDays</span></span>|<span data-ttu-id="b96ef-497">Int32</span><span class="sxs-lookup"><span data-stu-id="b96ef-497">Int32</span></span>|<span data-ttu-id="b96ef-498">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="b96ef-498">Number of days before the passcode expires.</span></span> <span data-ttu-id="b96ef-499">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="b96ef-499">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b96ef-500">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b96ef-500">passcodeMinimumLength</span></span>|<span data-ttu-id="b96ef-501">Int32</span><span class="sxs-lookup"><span data-stu-id="b96ef-501">Int32</span></span>|<span data-ttu-id="b96ef-502">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="b96ef-502">Minimum length of passcode.</span></span> <span data-ttu-id="b96ef-503">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="b96ef-503">Valid values 4 to 14</span></span>|
|<span data-ttu-id="b96ef-504">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b96ef-504">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b96ef-505">Int32</span><span class="sxs-lookup"><span data-stu-id="b96ef-505">Int32</span></span>|<span data-ttu-id="b96ef-506">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-506">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="b96ef-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b96ef-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b96ef-508">Int32</span><span class="sxs-lookup"><span data-stu-id="b96ef-508">Int32</span></span>|<span data-ttu-id="b96ef-509">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="b96ef-509">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b96ef-510">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b96ef-510">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="b96ef-511">Int32</span><span class="sxs-lookup"><span data-stu-id="b96ef-511">Int32</span></span>|<span data-ttu-id="b96ef-512">Anzahl von Zeichensätzen, die eine Kennung enthalten muss</span><span class="sxs-lookup"><span data-stu-id="b96ef-512">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="b96ef-513">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="b96ef-513">Valid values 0 to 4</span></span>|
|<span data-ttu-id="b96ef-514">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="b96ef-514">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="b96ef-515">Int32</span><span class="sxs-lookup"><span data-stu-id="b96ef-515">Int32</span></span>|<span data-ttu-id="b96ef-516">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="b96ef-516">Number of previous passcodes to block.</span></span> <span data-ttu-id="b96ef-517">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="b96ef-517">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b96ef-518">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="b96ef-518">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="b96ef-519">Int32</span><span class="sxs-lookup"><span data-stu-id="b96ef-519">Int32</span></span>|<span data-ttu-id="b96ef-520">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung des Geräts durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="b96ef-520">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="b96ef-521">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="b96ef-521">Valid values 4 to 11</span></span>|
|<span data-ttu-id="b96ef-522">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="b96ef-522">passcodeRequiredType</span></span>|[<span data-ttu-id="b96ef-523">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b96ef-523">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b96ef-524">Geforderter Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="b96ef-524">Type of passcode that is required.</span></span> <span data-ttu-id="b96ef-525">Mögliche Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b96ef-525">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b96ef-526">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="b96ef-526">passcodeRequired</span></span>|<span data-ttu-id="b96ef-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-527">Boolean</span></span>|<span data-ttu-id="b96ef-528">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-528">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="b96ef-529">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-529">podcastsBlocked</span></span>|<span data-ttu-id="b96ef-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-530">Boolean</span></span>|<span data-ttu-id="b96ef-531">Gibt an, ob verhindert werden soll, dass der Benutzer Podcasts auf dem überwachten Gerät verwendet (iOS 8.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-531">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="b96ef-532">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b96ef-532">safariBlockAutofill</span></span>|<span data-ttu-id="b96ef-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-533">Boolean</span></span>|<span data-ttu-id="b96ef-534">Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-534">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="b96ef-535">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b96ef-535">safariBlockJavaScript</span></span>|<span data-ttu-id="b96ef-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-536">Boolean</span></span>|<span data-ttu-id="b96ef-537">Gibt an, ob JavaScript in Safari blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-537">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="b96ef-538">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b96ef-538">safariBlockPopups</span></span>|<span data-ttu-id="b96ef-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-539">Boolean</span></span>|<span data-ttu-id="b96ef-540">Gibt an, ob Popups in Safari blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b96ef-540">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="b96ef-541">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-541">safariBlocked</span></span>|<span data-ttu-id="b96ef-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-542">Boolean</span></span>|<span data-ttu-id="b96ef-543">Gibt an, ob verhindert werden soll, dass der Benutzer Safari verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-543">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="b96ef-544">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b96ef-544">safariCookieSettings</span></span>|[<span data-ttu-id="b96ef-545">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b96ef-545">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="b96ef-546">Cokkieeinstellungen für Safari.</span><span class="sxs-lookup"><span data-stu-id="b96ef-546">Cookie settings for Safari.</span></span> <span data-ttu-id="b96ef-547">Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="b96ef-547">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="b96ef-548">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="b96ef-548">safariManagedDomains</span></span>|<span data-ttu-id="b96ef-549">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b96ef-549">String collection</span></span>|<span data-ttu-id="b96ef-550">URLs, die mit den hier aufgeführten Mustern übereinstimmen, werden als verwaltet betrachtet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-550">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="b96ef-551">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="b96ef-551">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="b96ef-552">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b96ef-552">String collection</span></span>|<span data-ttu-id="b96ef-553">Benutzer können Kennwörter in Safari nur von URLs speichern, die mit den hier aufgeführten Mustern übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="b96ef-553">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="b96ef-554">Gilt für Geräte im überwachten Modus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-554">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b96ef-555">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="b96ef-555">safariRequireFraudWarning</span></span>|<span data-ttu-id="b96ef-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-556">Boolean</span></span>|<span data-ttu-id="b96ef-557">Gibt an, ob eine Betrugswarnung in Safari erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-557">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="b96ef-558">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-558">screenCaptureBlocked</span></span>|<span data-ttu-id="b96ef-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-559">Boolean</span></span>|<span data-ttu-id="b96ef-560">Gibt an, ob verhindert werden soll, dass der Benutzer Screenshots macht.</span><span class="sxs-lookup"><span data-stu-id="b96ef-560">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="b96ef-561">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-561">siriBlocked</span></span>|<span data-ttu-id="b96ef-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-562">Boolean</span></span>|<span data-ttu-id="b96ef-563">Gibt an, ob verhindert werden soll, dass der Benutzer Siri verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-563">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="b96ef-564">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-564">siriBlockedWhenLocked</span></span>|<span data-ttu-id="b96ef-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-565">Boolean</span></span>|<span data-ttu-id="b96ef-566">Gibt an, ob verhindert werden soll, dass der Benutzer Siri bei Sperrung verwendet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-566">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="b96ef-567">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="b96ef-567">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="b96ef-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-568">Boolean</span></span>|<span data-ttu-id="b96ef-569">Gibt an, ob Siri bei Verwendung auf einem überwachten Gerät davon abgehalten werden soll, benutzergenerierte Inhalte abzufragen.</span><span class="sxs-lookup"><span data-stu-id="b96ef-569">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="b96ef-570">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="b96ef-570">siriRequireProfanityFilter</span></span>|<span data-ttu-id="b96ef-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-571">Boolean</span></span>|<span data-ttu-id="b96ef-572">Gibt an, ob verhindert werden soll, dass Siri anstößige Ausdrücke auf dem überwachten Gerät diktiert oder spricht.</span><span class="sxs-lookup"><span data-stu-id="b96ef-572">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="b96ef-573">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="b96ef-573">spotlightBlockInternetResults</span></span>|<span data-ttu-id="b96ef-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-574">Boolean</span></span>|<span data-ttu-id="b96ef-575">Gibt an, ob verhindert werden soll, dass die Spotlight-Suche Internetergebnisse auf dem überwachten Gerät zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="b96ef-575">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="b96ef-576">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-576">voiceDialingBlocked</span></span>|<span data-ttu-id="b96ef-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-577">Boolean</span></span>|<span data-ttu-id="b96ef-578">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b96ef-578">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="b96ef-579">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="b96ef-579">wallpaperBlockModification</span></span>|<span data-ttu-id="b96ef-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-580">Boolean</span></span>|<span data-ttu-id="b96ef-581">Gibt an, ob das Ändern des Hintergrunds auf einem überwachten Gerät (iOS 9.0 und höher) zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-581">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="b96ef-582">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="b96ef-582">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="b96ef-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-583">Boolean</span></span>|<span data-ttu-id="b96ef-584">Gibt an, ob erzwungen werden soll, dass das Gerät nur WLAN-Netzwerke aus Konfigurationsprofilen verwendet, wenn sich das Gerät im überwachten Modus befindet.</span><span class="sxs-lookup"><span data-stu-id="b96ef-584">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b96ef-585">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="b96ef-585">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="b96ef-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-586">Boolean</span></span>|<span data-ttu-id="b96ef-587">Gibt an, ob in einer nicht verwalteten Kurs über vor Ort registriert Student Berechtigung aus der Schulungsleiter anfordern soll, bei dem Versuch, lassen Sie den Kurs (iOS 11.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-587">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="b96ef-588">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="b96ef-588">keychainBlockCloudSync</span></span>|<span data-ttu-id="b96ef-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-589">Boolean</span></span>|<span data-ttu-id="b96ef-590">Gibt an, ob iCloud Schlüsselsammlung Synchronisierung ausgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="b96ef-590">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="b96ef-591">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="b96ef-591">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="b96ef-592">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-592">Boolean</span></span>|<span data-ttu-id="b96ef-593">Gibt an, ob over-the PKI-Updates blockiert sind.</span><span class="sxs-lookup"><span data-stu-id="b96ef-593">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="b96ef-594">Wenn Sie diese Einschränkung deaktivieren false nicht Zertifikatsperrlisten und OCSP-Prüfungen (iOS 7.0 und höher) festlegen.</span><span class="sxs-lookup"><span data-stu-id="b96ef-594">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="b96ef-595">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="b96ef-595">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="b96ef-596">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-596">Boolean</span></span>|<span data-ttu-id="b96ef-597">Gibt an, ob Ad nachverfolgen beschränkt ist. (iOS 7.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-597">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="b96ef-598">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="b96ef-598">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="b96ef-599">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-599">Boolean</span></span>|<span data-ttu-id="b96ef-600">Gibt an, dass unabhängig davon, ob Enterprise zum Sichern von Buch ausgeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="b96ef-600">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="b96ef-601">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="b96ef-601">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="b96ef-602">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-602">Boolean</span></span>|<span data-ttu-id="b96ef-603">Gibt an, ob Enterprise Adressbuch Notizen und highlights zur Synchronisierung ausgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="b96ef-603">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="b96ef-604">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="b96ef-604">airPrintBlocked</span></span>|<span data-ttu-id="b96ef-605">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-605">Boolean</span></span>|<span data-ttu-id="b96ef-606">Gibt an, ob AirPrint blockierte (iOS 11.0 und höher) ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-606">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b96ef-607">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="b96ef-607">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="b96ef-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-608">Boolean</span></span>|<span data-ttu-id="b96ef-609">Gibt an, ob Schlüsselsammlung Speicherung von Benutzername und Kennwort für Airprint blockierte (iOS 11.0 und höher) ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-609">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b96ef-610">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="b96ef-610">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="b96ef-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-611">Boolean</span></span>|<span data-ttu-id="b96ef-612">Gibt an, ob vertrauenswürdige Zertifikate für Drucken TLS-Kommunikation (iOS 11.0 und höher) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b96ef-612">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b96ef-613">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="b96ef-613">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="b96ef-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-614">Boolean</span></span>|<span data-ttu-id="b96ef-615">Gibt an, ob iBeacon Ermittlung von AirPrint Drucker ausgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="b96ef-615">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="b96ef-616">Dies verhindert, dass falsche AirPrint Bluetooth Beacons vor Phishing für den Netzwerkdatenverkehr (iOS 11.0 und höher).</span><span class="sxs-lookup"><span data-stu-id="b96ef-616">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b96ef-617">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="b96ef-617">blockSystemAppRemoval</span></span>|<span data-ttu-id="b96ef-618">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-618">Boolean</span></span>|<span data-ttu-id="b96ef-619">Gibt an, ob das Entfernen der System apps aus dem Gerät auf einem überwachten Gerät (iOS 11.0 und höher) ausgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="b96ef-619">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b96ef-620">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="b96ef-620">vpnBlockCreation</span></span>|<span data-ttu-id="b96ef-621">Boolean</span><span class="sxs-lookup"><span data-stu-id="b96ef-621">Boolean</span></span>|<span data-ttu-id="b96ef-622">Gibt an, ob die Erstellung des VPN-Konfigurationen blockierte (iOS 11.0 und höher) ist.</span><span class="sxs-lookup"><span data-stu-id="b96ef-622">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|



## <a name="response"></a><span data-ttu-id="b96ef-623">Antwort</span><span class="sxs-lookup"><span data-stu-id="b96ef-623">Response</span></span>
<span data-ttu-id="b96ef-624">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b96ef-624">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b96ef-625">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b96ef-625">Example</span></span>
### <a name="request"></a><span data-ttu-id="b96ef-626">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b96ef-626">Request</span></span>
<span data-ttu-id="b96ef-627">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b96ef-627">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 8428

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "vpnBlockCreation": true
}
```

### <a name="response"></a><span data-ttu-id="b96ef-628">Antwort</span><span class="sxs-lookup"><span data-stu-id="b96ef-628">Response</span></span>
<span data-ttu-id="b96ef-p132">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b96ef-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8604

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
  "vpnBlockCreation": true
}
```





