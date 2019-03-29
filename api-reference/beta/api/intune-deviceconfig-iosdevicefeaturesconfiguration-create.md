---
title: Erstellen von „iosDeviceFeaturesConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec2bcc7f6d18a98ad7e6cd83e1abf12ef7fa962d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967125"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="5c431-103">Erstellen von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="5c431-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="5c431-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5c431-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c431-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5c431-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c431-106">Diese Methode erstellt ein neues Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c431-106">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c431-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5c431-107">Prerequisites</span></span>
<span data-ttu-id="5c431-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c431-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c431-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c431-110">Permission type</span></span>|<span data-ttu-id="5c431-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c431-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c431-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c431-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c431-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c431-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c431-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c431-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c431-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c431-115">Not supported.</span></span>|
|<span data-ttu-id="5c431-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c431-116">Application</span></span>|<span data-ttu-id="5c431-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c431-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c431-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c431-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5c431-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5c431-119">Request headers</span></span>
|<span data-ttu-id="5c431-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5c431-120">Header</span></span>|<span data-ttu-id="5c431-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5c431-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c431-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c431-122">Authorization</span></span>|<span data-ttu-id="5c431-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5c431-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c431-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5c431-124">Accept</span></span>|<span data-ttu-id="5c431-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c431-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c431-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5c431-126">Request body</span></span>
<span data-ttu-id="5c431-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosDeviceFeaturesConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="5c431-127">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="5c431-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosDeviceFeaturesConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="5c431-128">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="5c431-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c431-129">Property</span></span>|<span data-ttu-id="5c431-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5c431-130">Type</span></span>|<span data-ttu-id="5c431-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c431-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c431-132">id</span><span class="sxs-lookup"><span data-stu-id="5c431-132">id</span></span>|<span data-ttu-id="5c431-133">String</span><span class="sxs-lookup"><span data-stu-id="5c431-133">String</span></span>|<span data-ttu-id="5c431-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5c431-134">Key of the entity.</span></span> <span data-ttu-id="5c431-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c431-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c431-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c431-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5c431-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c431-137">DateTimeOffset</span></span>|<span data-ttu-id="5c431-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5c431-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5c431-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c431-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c431-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="5c431-140">roleScopeTagIds</span></span>|<span data-ttu-id="5c431-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5c431-141">String collection</span></span>|<span data-ttu-id="5c431-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="5c431-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5c431-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c431-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c431-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5c431-144">supportsScopeTags</span></span>|<span data-ttu-id="5c431-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5c431-145">Boolean</span></span>|<span data-ttu-id="5c431-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5c431-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5c431-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="5c431-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5c431-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="5c431-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5c431-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5c431-149">This property is read-only.</span></span> <span data-ttu-id="5c431-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c431-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c431-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c431-151">createdDateTime</span></span>|<span data-ttu-id="5c431-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c431-152">DateTimeOffset</span></span>|<span data-ttu-id="5c431-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5c431-153">DateTime the object was created.</span></span> <span data-ttu-id="5c431-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c431-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c431-155">description</span><span class="sxs-lookup"><span data-stu-id="5c431-155">description</span></span>|<span data-ttu-id="5c431-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c431-156">String</span></span>|<span data-ttu-id="5c431-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5c431-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c431-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c431-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c431-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5c431-159">displayName</span></span>|<span data-ttu-id="5c431-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c431-160">String</span></span>|<span data-ttu-id="5c431-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5c431-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c431-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c431-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c431-163">Version</span><span class="sxs-lookup"><span data-stu-id="5c431-163">version</span></span>|<span data-ttu-id="5c431-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5c431-164">Int32</span></span>|<span data-ttu-id="5c431-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5c431-165">Version of the device configuration.</span></span> <span data-ttu-id="5c431-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c431-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c431-167">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="5c431-167">airPrintDestinations</span></span>|<span data-ttu-id="5c431-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="5c431-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="5c431-169">Ein Array von Druck Druckern, die immer angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5c431-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="5c431-170">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="5c431-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="5c431-171">Geerbt von [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="5c431-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="5c431-172">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="5c431-172">assetTagTemplate</span></span>|<span data-ttu-id="5c431-173">String</span><span class="sxs-lookup"><span data-stu-id="5c431-173">String</span></span>|<span data-ttu-id="5c431-174">Bestandskennzeicheninformationen zum Gerät. Sie werden im Anmeldefenster und im Sperrbildschirm angezeigt.</span><span class="sxs-lookup"><span data-stu-id="5c431-174">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="5c431-175">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="5c431-175">contentFilterSettings</span></span>|[<span data-ttu-id="5c431-176">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="5c431-176">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="5c431-177">Dient zum Abrufen oder Festlegen von iOS Web Content Filter-Einstellungen, nur überwachter Modus</span><span class="sxs-lookup"><span data-stu-id="5c431-177">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="5c431-178">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="5c431-178">lockScreenFootnote</span></span>|<span data-ttu-id="5c431-179">String</span><span class="sxs-lookup"><span data-stu-id="5c431-179">String</span></span>|<span data-ttu-id="5c431-180">Fußnote, die im Anmeldefenster und im Sperrbildschirm angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5c431-180">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="5c431-181">Verfügbar ab iOS 9.3.1.</span><span class="sxs-lookup"><span data-stu-id="5c431-181">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="5c431-182">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="5c431-182">homeScreenDockIcons</span></span>|<span data-ttu-id="5c431-183">Collection von Objekten des Typs [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="5c431-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="5c431-184">Liste der Apps und Ordner, die im Home-Bildschirm-Dock angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5c431-184">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="5c431-185">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="5c431-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5c431-186">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="5c431-186">homeScreenPages</span></span>|<span data-ttu-id="5c431-187">Collection von Objekten des Typs [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="5c431-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="5c431-188">Liste der Seiten auf dem Home-Bildschirm.</span><span class="sxs-lookup"><span data-stu-id="5c431-188">A list of pages on the Home Screen.</span></span> <span data-ttu-id="5c431-189">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="5c431-189">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5c431-190">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="5c431-190">notificationSettings</span></span>|<span data-ttu-id="5c431-191">Collection von Objekten des Typs [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="5c431-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="5c431-192">Benachrichtigungseinstellungen für jede Bundle-ID. Gilt nur für Geräte im Betreuungsmodus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="5c431-192">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="5c431-193">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="5c431-193">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5c431-194">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="5c431-194">singleSignOnSettings</span></span>|[<span data-ttu-id="5c431-195">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="5c431-195">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="5c431-196">Die Kerberos-Anmeldeeinstellungen, mit denen sich apps auf dem Empfangsgerät reibungslos authentifizieren können.</span><span class="sxs-lookup"><span data-stu-id="5c431-196">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="5c431-197">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="5c431-197">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="5c431-198">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="5c431-198">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="5c431-199">Ein Hintergrundanzeige-Standort Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="5c431-199">A wallpaper display location specifier.</span></span> <span data-ttu-id="5c431-200">Mögliche Werte sind: `notConfigured`, `lockScreen`, `homeScreen` und `lockAndHomeScreens`.</span><span class="sxs-lookup"><span data-stu-id="5c431-200">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="5c431-201">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="5c431-201">wallpaperImage</span></span>|[<span data-ttu-id="5c431-202">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5c431-202">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5c431-203">Ein Hintergrundbild muss im PNG-oder JPEG-Format vorliegen.</span><span class="sxs-lookup"><span data-stu-id="5c431-203">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="5c431-204">Es erfordert ein überwachte Gerät mit iOS 8 oder höher.</span><span class="sxs-lookup"><span data-stu-id="5c431-204">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="5c431-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c431-205">Response</span></span>
<span data-ttu-id="5c431-206">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5c431-206">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c431-207">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5c431-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c431-208">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c431-208">Request</span></span>
<span data-ttu-id="5c431-209">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5c431-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3656

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  },
  "wallpaperDisplayLocation": "lockScreen",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="5c431-210">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c431-210">Response</span></span>
<span data-ttu-id="5c431-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c431-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3828

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  },
  "wallpaperDisplayLocation": "lockScreen",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```




