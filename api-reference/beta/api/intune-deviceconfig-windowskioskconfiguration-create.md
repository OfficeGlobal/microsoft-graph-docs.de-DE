---
title: WindowsKioskConfiguration erstellen
description: Erstellen eines neuen windowsKioskConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd32b23626c027cfc4a9cdac60b5a5a4a6c37973
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160746"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="00885-103">WindowsKioskConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="00885-103">Create windowsKioskConfiguration</span></span>

> <span data-ttu-id="00885-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00885-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00885-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="00885-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00885-106">Erstellen eines neuen [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="00885-106">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00885-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="00885-107">Prerequisites</span></span>
<span data-ttu-id="00885-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="00885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="00885-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00885-110">Permission type</span></span>|<span data-ttu-id="00885-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00885-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00885-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00885-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00885-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00885-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00885-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00885-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00885-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00885-115">Not supported.</span></span>|
|<span data-ttu-id="00885-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00885-116">Application</span></span>|<span data-ttu-id="00885-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00885-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00885-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00885-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="00885-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00885-119">Request headers</span></span>
|<span data-ttu-id="00885-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="00885-120">Header</span></span>|<span data-ttu-id="00885-121">Wert</span><span class="sxs-lookup"><span data-stu-id="00885-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00885-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00885-122">Authorization</span></span>|<span data-ttu-id="00885-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="00885-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00885-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="00885-124">Accept</span></span>|<span data-ttu-id="00885-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00885-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00885-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="00885-126">Request body</span></span>
<span data-ttu-id="00885-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsKioskConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="00885-127">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="00885-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsKioskConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="00885-128">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="00885-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00885-129">Property</span></span>|<span data-ttu-id="00885-130">Typ</span><span class="sxs-lookup"><span data-stu-id="00885-130">Type</span></span>|<span data-ttu-id="00885-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00885-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00885-132">id</span><span class="sxs-lookup"><span data-stu-id="00885-132">id</span></span>|<span data-ttu-id="00885-133">string</span><span class="sxs-lookup"><span data-stu-id="00885-133">String</span></span>|<span data-ttu-id="00885-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="00885-134">Key of the entity.</span></span> <span data-ttu-id="00885-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00885-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00885-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00885-136">lastModifiedDateTime</span></span>|<span data-ttu-id="00885-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00885-137">DateTimeOffset</span></span>|<span data-ttu-id="00885-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="00885-138">DateTime the object was last modified.</span></span> <span data-ttu-id="00885-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00885-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00885-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="00885-140">roleScopeTagIds</span></span>|<span data-ttu-id="00885-141">String collection</span><span class="sxs-lookup"><span data-stu-id="00885-141">String collection</span></span>|<span data-ttu-id="00885-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="00885-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="00885-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00885-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00885-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="00885-144">supportsScopeTags</span></span>|<span data-ttu-id="00885-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00885-145">Boolean</span></span>|<span data-ttu-id="00885-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00885-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="00885-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="00885-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="00885-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="00885-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="00885-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="00885-149">This property is read-only.</span></span> <span data-ttu-id="00885-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00885-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00885-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00885-151">createdDateTime</span></span>|<span data-ttu-id="00885-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00885-152">DateTimeOffset</span></span>|<span data-ttu-id="00885-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="00885-153">DateTime the object was created.</span></span> <span data-ttu-id="00885-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00885-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00885-155">description</span><span class="sxs-lookup"><span data-stu-id="00885-155">description</span></span>|<span data-ttu-id="00885-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00885-156">String</span></span>|<span data-ttu-id="00885-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="00885-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="00885-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00885-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00885-159">displayName</span><span class="sxs-lookup"><span data-stu-id="00885-159">displayName</span></span>|<span data-ttu-id="00885-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00885-160">String</span></span>|<span data-ttu-id="00885-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="00885-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="00885-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00885-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00885-163">Version</span><span class="sxs-lookup"><span data-stu-id="00885-163">version</span></span>|<span data-ttu-id="00885-164">Int32</span><span class="sxs-lookup"><span data-stu-id="00885-164">Int32</span></span>|<span data-ttu-id="00885-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="00885-165">Version of the device configuration.</span></span> <span data-ttu-id="00885-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00885-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00885-167">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="00885-167">kioskProfiles</span></span>|<span data-ttu-id="00885-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="00885-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="00885-169">Mit dieser Richtlinieneinstellung können Sie eine Liste der Kiosk Profile für eine Kiosk Konfiguration definieren.</span><span class="sxs-lookup"><span data-stu-id="00885-169">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="00885-170">Diese Auflistung kann maximal drei Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="00885-170">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="00885-171">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="00885-171">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="00885-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00885-172">String</span></span>|<span data-ttu-id="00885-173">Geben Sie die Standard-URL an, zu der der Browser beim Start navigieren soll.</span><span class="sxs-lookup"><span data-stu-id="00885-173">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="00885-174">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="00885-174">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="00885-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00885-175">Boolean</span></span>|<span data-ttu-id="00885-176">Aktivieren Sie die Schaltfläche Home des Kiosk Browsers.</span><span class="sxs-lookup"><span data-stu-id="00885-176">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="00885-177">Standardmäßig ist die Schaltfläche Start deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="00885-177">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="00885-178">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="00885-178">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="00885-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00885-179">Boolean</span></span>|<span data-ttu-id="00885-180">Aktivieren Sie die Navigationsschaltflächen des Kiosk Browsers (Forward/Back).</span><span class="sxs-lookup"><span data-stu-id="00885-180">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="00885-181">Standardmäßig sind die Navigationsschaltflächen deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="00885-181">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="00885-182">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="00885-182">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="00885-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00885-183">Boolean</span></span>|<span data-ttu-id="00885-184">Aktivieren Sie die Schaltfläche Endsitzung des Kiosk Browsers.</span><span class="sxs-lookup"><span data-stu-id="00885-184">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="00885-185">Standardmäßig ist die Schaltfläche Sitzung beenden deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="00885-185">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="00885-186">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="00885-186">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="00885-187">Int32</span><span class="sxs-lookup"><span data-stu-id="00885-187">Int32</span></span>|<span data-ttu-id="00885-188">Geben Sie die Anzahl der Minuten an, die die Sitzung inaktiv ist, bis der Kiosk-Browser neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="00885-188">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="00885-189">Gültige Werte sind 1-1440.</span><span class="sxs-lookup"><span data-stu-id="00885-189">Valid values are 1-1440.</span></span> <span data-ttu-id="00885-190">Gültige Werte 1 bis 1440</span><span class="sxs-lookup"><span data-stu-id="00885-190">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="00885-191">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="00885-191">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="00885-192">String collection</span><span class="sxs-lookup"><span data-stu-id="00885-192">String collection</span></span>|<span data-ttu-id="00885-193">Angeben von URLs, zu denen die Kiosk-Browser nicht navigieren sollen</span><span class="sxs-lookup"><span data-stu-id="00885-193">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="00885-194">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="00885-194">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="00885-195">String collection</span><span class="sxs-lookup"><span data-stu-id="00885-195">String collection</span></span>|<span data-ttu-id="00885-196">Angeben von URLs, zu denen der Kiosk Browser navigieren darf</span><span class="sxs-lookup"><span data-stu-id="00885-196">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="00885-197">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="00885-197">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="00885-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00885-198">Boolean</span></span>|<span data-ttu-id="00885-199">Aktivieren Sie das öffentliche Browsen im Kioskmodus für den Microsoft Edge-Browser.</span><span class="sxs-lookup"><span data-stu-id="00885-199">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="00885-200">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="00885-200">The Default is false.</span></span>|
|<span data-ttu-id="00885-201">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="00885-201">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="00885-202">Int32</span><span class="sxs-lookup"><span data-stu-id="00885-202">Int32</span></span>|<span data-ttu-id="00885-203">Gibt die Zeit in Minuten der letzten Benutzeraktivität an, bevor Microsoft Edge Kiosk zurückgesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="00885-203">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="00885-204">Gültige Werte sind 0-1440.</span><span class="sxs-lookup"><span data-stu-id="00885-204">Valid values are 0-1440.</span></span> <span data-ttu-id="00885-205">Der Standardwert ist 5.</span><span class="sxs-lookup"><span data-stu-id="00885-205">The default is 5.</span></span> <span data-ttu-id="00885-206">0 gibt keine Zurücksetzung an.</span><span class="sxs-lookup"><span data-stu-id="00885-206">0 indicates no reset.</span></span> <span data-ttu-id="00885-207">Gültige Werte 0 bis 1440</span><span class="sxs-lookup"><span data-stu-id="00885-207">Valid values 0 to 1440</span></span>|



## <a name="response"></a><span data-ttu-id="00885-208">Antwort</span><span class="sxs-lookup"><span data-stu-id="00885-208">Response</span></span>
<span data-ttu-id="00885-209">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="00885-209">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00885-210">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00885-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="00885-211">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00885-211">Request</span></span>
<span data-ttu-id="00885-212">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00885-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1719

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "Profile Id value",
      "profileName": "Profile Name value",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "small",
            "name": "Name value",
            "appType": "store",
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 6,
  "kioskBrowserBlockedURLs": [
    "Kiosk Browser Blocked URLs value"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "Kiosk Browser Blocked Url Exceptions value"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "edgeKioskResetAfterIdleTimeInMinutes": 4
}
```

### <a name="response"></a><span data-ttu-id="00885-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="00885-213">Response</span></span>
<span data-ttu-id="00885-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00885-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1891

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "id": "146a990b-990b-146a-0b99-6a140b996a14",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "Profile Id value",
      "profileName": "Profile Name value",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "small",
            "name": "Name value",
            "appType": "store",
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 6,
  "kioskBrowserBlockedURLs": [
    "Kiosk Browser Blocked URLs value"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "Kiosk Browser Blocked Url Exceptions value"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "edgeKioskResetAfterIdleTimeInMinutes": 4
}
```




