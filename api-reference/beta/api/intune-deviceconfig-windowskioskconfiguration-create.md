---
title: Erstellen von windowsKioskConfiguration
description: Erstellen eines neuen WindowsKioskConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 75e500ae8cf8ce272ee8571de24f18723f0594e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868376"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="c2490-103">Erstellen von windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2490-103">Create windowsKioskConfiguration</span></span>

> <span data-ttu-id="c2490-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c2490-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2490-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c2490-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2490-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c2490-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2490-107">Erstellen eines neuen [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c2490-107">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2490-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c2490-108">Prerequisites</span></span>
<span data-ttu-id="c2490-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2490-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2490-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c2490-111">Permission type</span></span>|<span data-ttu-id="c2490-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c2490-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2490-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c2490-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2490-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2490-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2490-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c2490-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2490-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2490-116">Not supported.</span></span>|
|<span data-ttu-id="c2490-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c2490-117">Application</span></span>|<span data-ttu-id="c2490-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2490-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2490-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2490-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c2490-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c2490-120">Request headers</span></span>
|<span data-ttu-id="c2490-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c2490-121">Header</span></span>|<span data-ttu-id="c2490-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c2490-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2490-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2490-123">Authorization</span></span>|<span data-ttu-id="c2490-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c2490-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2490-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c2490-125">Accept</span></span>|<span data-ttu-id="c2490-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2490-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2490-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c2490-127">Request body</span></span>
<span data-ttu-id="c2490-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsKioskConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c2490-128">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="c2490-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsKioskConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="c2490-129">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="c2490-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c2490-130">Property</span></span>|<span data-ttu-id="c2490-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c2490-131">Type</span></span>|<span data-ttu-id="c2490-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2490-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2490-133">id</span><span class="sxs-lookup"><span data-stu-id="c2490-133">id</span></span>|<span data-ttu-id="c2490-134">String</span><span class="sxs-lookup"><span data-stu-id="c2490-134">String</span></span>|<span data-ttu-id="c2490-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c2490-135">Key of the entity.</span></span> <span data-ttu-id="c2490-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2490-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2490-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2490-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c2490-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2490-138">DateTimeOffset</span></span>|<span data-ttu-id="c2490-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c2490-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c2490-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2490-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2490-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c2490-141">roleScopeTagIds</span></span>|<span data-ttu-id="c2490-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c2490-142">String collection</span></span>|<span data-ttu-id="c2490-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="c2490-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c2490-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2490-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2490-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c2490-145">supportsScopeTags</span></span>|<span data-ttu-id="c2490-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2490-146">Boolean</span></span>|<span data-ttu-id="c2490-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c2490-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c2490-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c2490-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c2490-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="c2490-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c2490-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c2490-150">This property is read-only.</span></span> <span data-ttu-id="c2490-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2490-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2490-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2490-152">createdDateTime</span></span>|<span data-ttu-id="c2490-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2490-153">DateTimeOffset</span></span>|<span data-ttu-id="c2490-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c2490-154">DateTime the object was created.</span></span> <span data-ttu-id="c2490-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2490-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2490-156">description</span><span class="sxs-lookup"><span data-stu-id="c2490-156">description</span></span>|<span data-ttu-id="c2490-157">String</span><span class="sxs-lookup"><span data-stu-id="c2490-157">String</span></span>|<span data-ttu-id="c2490-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c2490-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c2490-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2490-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2490-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c2490-160">displayName</span></span>|<span data-ttu-id="c2490-161">String</span><span class="sxs-lookup"><span data-stu-id="c2490-161">String</span></span>|<span data-ttu-id="c2490-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c2490-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c2490-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2490-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2490-164">Version</span><span class="sxs-lookup"><span data-stu-id="c2490-164">version</span></span>|<span data-ttu-id="c2490-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c2490-165">Int32</span></span>|<span data-ttu-id="c2490-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c2490-166">Version of the device configuration.</span></span> <span data-ttu-id="c2490-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2490-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2490-168">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="c2490-168">kioskProfiles</span></span>|<span data-ttu-id="c2490-169">[WindowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c2490-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="c2490-170">Diese Richtlinie ermöglicht zum Definieren einer Liste von Kiosk-Profilen für eine Kiosk-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="c2490-170">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="c2490-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c2490-171">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c2490-172">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="c2490-172">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="c2490-173">String</span><span class="sxs-lookup"><span data-stu-id="c2490-173">String</span></span>|<span data-ttu-id="c2490-174">Geben Sie den Standard-URL der Browser navigieren soll auf starten.</span><span class="sxs-lookup"><span data-stu-id="c2490-174">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="c2490-175">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="c2490-175">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="c2490-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2490-176">Boolean</span></span>|<span data-ttu-id="c2490-177">Aktivieren des Kiosk-Browsers home-Schaltfläche.</span><span class="sxs-lookup"><span data-stu-id="c2490-177">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="c2490-178">Die home-Schaltfläche ist standardmäßig deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="c2490-178">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="c2490-179">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="c2490-179">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="c2490-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2490-180">Boolean</span></span>|<span data-ttu-id="c2490-181">Aktivieren des Kiosk-Browsers Navigation buttons(forward/back).</span><span class="sxs-lookup"><span data-stu-id="c2490-181">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="c2490-182">Die Navigationsschaltflächen werden standardmäßig deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="c2490-182">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="c2490-183">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="c2490-183">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="c2490-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2490-184">Boolean</span></span>|<span data-ttu-id="c2490-185">Aktivieren des Kiosk-Browsers End Sitzung Schaltfläche.</span><span class="sxs-lookup"><span data-stu-id="c2490-185">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="c2490-186">Die Schaltfläche Beenden Sitzung ist standardmäßig deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="c2490-186">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="c2490-187">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="c2490-187">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="c2490-188">Int32</span><span class="sxs-lookup"><span data-stu-id="c2490-188">Int32</span></span>|<span data-ttu-id="c2490-189">Geben Sie die Anzahl der Minuten, die Sitzung im Leerlauf befindet, bis der Kiosk-Browser in einen neuen Status neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="c2490-189">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="c2490-190">Gültige Werte sind 1 und 1440.</span><span class="sxs-lookup"><span data-stu-id="c2490-190">Valid values are 1-1440.</span></span> <span data-ttu-id="c2490-191">Gültige Werte 1 bis 1440</span><span class="sxs-lookup"><span data-stu-id="c2490-191">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="c2490-192">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="c2490-192">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="c2490-193">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c2490-193">String collection</span></span>|<span data-ttu-id="c2490-194">Geben Sie die URLs, die nicht die Kiosk-Browser navigieren soll</span><span class="sxs-lookup"><span data-stu-id="c2490-194">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="c2490-195">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="c2490-195">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="c2490-196">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c2490-196">String collection</span></span>|<span data-ttu-id="c2490-197">Geben Sie die URLs, die im Browser Kiosk zulässig ist, zu dem navigiert</span><span class="sxs-lookup"><span data-stu-id="c2490-197">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|



## <a name="response"></a><span data-ttu-id="c2490-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2490-198">Response</span></span>
<span data-ttu-id="c2490-199">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c2490-199">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2490-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c2490-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2490-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2490-201">Request</span></span>
<span data-ttu-id="c2490-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c2490-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1662

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="c2490-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2490-203">Response</span></span>
<span data-ttu-id="c2490-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c2490-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1770

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
  ]
}
```





