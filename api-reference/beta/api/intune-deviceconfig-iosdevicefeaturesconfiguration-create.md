---
title: Erstellen von „iosDeviceFeaturesConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs iosDeviceFeaturesConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6f6a5fe84c5ecd4f95168c027a344237a55961b3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423195"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="ee411-103">Erstellen von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="ee411-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="ee411-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ee411-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee411-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ee411-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee411-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ee411-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee411-107">Diese Methode erstellt ein neues Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee411-107">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee411-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ee411-108">Prerequisites</span></span>
<span data-ttu-id="ee411-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee411-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ee411-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ee411-111">Permission type</span></span>|<span data-ttu-id="ee411-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ee411-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee411-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ee411-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee411-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee411-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee411-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ee411-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee411-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee411-116">Not supported.</span></span>|
|<span data-ttu-id="ee411-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ee411-117">Application</span></span>|<span data-ttu-id="ee411-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee411-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee411-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee411-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ee411-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ee411-120">Request headers</span></span>
|<span data-ttu-id="ee411-121">Header</span><span class="sxs-lookup"><span data-stu-id="ee411-121">Header</span></span>|<span data-ttu-id="ee411-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ee411-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee411-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ee411-123">Authorization</span></span>|<span data-ttu-id="ee411-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ee411-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee411-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ee411-125">Accept</span></span>|<span data-ttu-id="ee411-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee411-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee411-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ee411-127">Request body</span></span>
<span data-ttu-id="ee411-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosDeviceFeaturesConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="ee411-128">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="ee411-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosDeviceFeaturesConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ee411-129">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="ee411-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ee411-130">Property</span></span>|<span data-ttu-id="ee411-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ee411-131">Type</span></span>|<span data-ttu-id="ee411-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee411-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee411-133">id</span><span class="sxs-lookup"><span data-stu-id="ee411-133">id</span></span>|<span data-ttu-id="ee411-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee411-134">String</span></span>|<span data-ttu-id="ee411-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ee411-135">Key of the entity.</span></span> <span data-ttu-id="ee411-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee411-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee411-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee411-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ee411-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee411-138">DateTimeOffset</span></span>|<span data-ttu-id="ee411-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ee411-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ee411-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee411-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee411-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee411-141">roleScopeTagIds</span></span>|<span data-ttu-id="ee411-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="ee411-142">String collection</span></span>|<span data-ttu-id="ee411-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="ee411-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ee411-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee411-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee411-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ee411-145">supportsScopeTags</span></span>|<span data-ttu-id="ee411-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee411-146">Boolean</span></span>|<span data-ttu-id="ee411-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ee411-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ee411-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="ee411-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ee411-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="ee411-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ee411-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ee411-150">This property is read-only.</span></span> <span data-ttu-id="ee411-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee411-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee411-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee411-152">createdDateTime</span></span>|<span data-ttu-id="ee411-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee411-153">DateTimeOffset</span></span>|<span data-ttu-id="ee411-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ee411-154">DateTime the object was created.</span></span> <span data-ttu-id="ee411-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee411-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee411-156">description</span><span class="sxs-lookup"><span data-stu-id="ee411-156">description</span></span>|<span data-ttu-id="ee411-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee411-157">String</span></span>|<span data-ttu-id="ee411-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ee411-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ee411-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee411-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee411-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ee411-160">displayName</span></span>|<span data-ttu-id="ee411-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee411-161">String</span></span>|<span data-ttu-id="ee411-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ee411-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ee411-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee411-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee411-164">Version</span><span class="sxs-lookup"><span data-stu-id="ee411-164">version</span></span>|<span data-ttu-id="ee411-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ee411-165">Int32</span></span>|<span data-ttu-id="ee411-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ee411-166">Version of the device configuration.</span></span> <span data-ttu-id="ee411-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee411-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee411-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="ee411-168">airPrintDestinations</span></span>|<span data-ttu-id="ee411-169">[AirPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ee411-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="ee411-170">Ein Array von AirPrint aus, die immer angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ee411-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="ee411-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ee411-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ee411-172">Geerbt von [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="ee411-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="ee411-173">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="ee411-173">assetTagTemplate</span></span>|<span data-ttu-id="ee411-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee411-174">String</span></span>|<span data-ttu-id="ee411-175">Bestandskennzeicheninformationen zum Gerät. Sie werden im Anmeldefenster und im Sperrbildschirm angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ee411-175">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="ee411-176">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="ee411-176">contentFilterSettings</span></span>|[<span data-ttu-id="ee411-177">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="ee411-177">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="ee411-178">Ruft ab oder legt diesen fest iOS Einstellungen für die Inhaltsfilterung Web, nur überwachten Modus</span><span class="sxs-lookup"><span data-stu-id="ee411-178">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="ee411-179">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="ee411-179">lockScreenFootnote</span></span>|<span data-ttu-id="ee411-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee411-180">String</span></span>|<span data-ttu-id="ee411-181">Fußnote, die im Anmeldefenster und im Sperrbildschirm angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ee411-181">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="ee411-182">Verfügbar ab iOS 9.3.1.</span><span class="sxs-lookup"><span data-stu-id="ee411-182">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="ee411-183">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="ee411-183">homeScreenDockIcons</span></span>|<span data-ttu-id="ee411-184">Collection von Objekten des Typs [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="ee411-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="ee411-185">Liste der Apps und Ordner, die im Home-Bildschirm-Dock angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ee411-185">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="ee411-186">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ee411-186">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ee411-187">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="ee411-187">homeScreenPages</span></span>|<span data-ttu-id="ee411-188">Collection von Objekten des Typs [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="ee411-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="ee411-189">Liste der Seiten auf dem Home-Bildschirm.</span><span class="sxs-lookup"><span data-stu-id="ee411-189">A list of pages on the Home Screen.</span></span> <span data-ttu-id="ee411-190">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ee411-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ee411-191">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="ee411-191">notificationSettings</span></span>|<span data-ttu-id="ee411-192">Collection von Objekten des Typs [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ee411-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="ee411-193">Benachrichtigungseinstellungen für jede Bundle-ID. Gilt nur für Geräte im Betreuungsmodus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="ee411-193">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="ee411-194">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ee411-194">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ee411-195">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="ee411-195">singleSignOnSettings</span></span>|[<span data-ttu-id="ee411-196">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="ee411-196">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="ee411-197">Die Kerberos-anmeldeeinstellungen, mit denen apps auf das Empfangen von Geräten reibungslos authentifizieren.</span><span class="sxs-lookup"><span data-stu-id="ee411-197">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="ee411-198">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="ee411-198">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="ee411-199">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="ee411-199">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="ee411-200">Ein Hintergrundbild Speicherort Anzeigebezeichner.</span><span class="sxs-lookup"><span data-stu-id="ee411-200">A wallpaper display location specifier.</span></span> <span data-ttu-id="ee411-201">Mögliche Werte: sind `notConfigured`, `lockScreen`, `homeScreen` und `lockAndHomeScreens`.</span><span class="sxs-lookup"><span data-stu-id="ee411-201">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="ee411-202">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="ee411-202">wallpaperImage</span></span>|[<span data-ttu-id="ee411-203">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ee411-203">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ee411-204">Ein Hintergrundbild muss PNG- oder JPEG-Format aufweisen.</span><span class="sxs-lookup"><span data-stu-id="ee411-204">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="ee411-205">Eine überwachten Gerät mit iOS 8 oder höher benötigt.</span><span class="sxs-lookup"><span data-stu-id="ee411-205">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="ee411-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee411-206">Response</span></span>
<span data-ttu-id="ee411-207">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ee411-207">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee411-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ee411-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee411-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee411-209">Request</span></span>
<span data-ttu-id="ee411-210">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ee411-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee411-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee411-211">Response</span></span>
<span data-ttu-id="ee411-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee411-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




