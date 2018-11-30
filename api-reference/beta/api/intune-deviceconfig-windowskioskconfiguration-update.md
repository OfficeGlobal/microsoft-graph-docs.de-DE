---
title: WindowsKioskConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsKioskConfiguration-Objekts.
ms.openlocfilehash: 87cc7db067f41e87d3ca4ae0ef77052cc9f0c53d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064888"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="0782f-103">WindowsKioskConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0782f-103">Update windowsKioskConfiguration</span></span>

> <span data-ttu-id="0782f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0782f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0782f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0782f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0782f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0782f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0782f-107">Aktualisieren Sie die Eigenschaften eines [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0782f-107">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0782f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0782f-108">Prerequisites</span></span>
<span data-ttu-id="0782f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0782f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0782f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0782f-111">Permission type</span></span>|<span data-ttu-id="0782f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0782f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0782f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0782f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0782f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0782f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0782f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0782f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0782f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0782f-116">Not supported.</span></span>|
|<span data-ttu-id="0782f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0782f-117">Application</span></span>|<span data-ttu-id="0782f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0782f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0782f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0782f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0782f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0782f-120">Request headers</span></span>
|<span data-ttu-id="0782f-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0782f-121">Header</span></span>|<span data-ttu-id="0782f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0782f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0782f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0782f-123">Authorization</span></span>|<span data-ttu-id="0782f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0782f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0782f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0782f-125">Accept</span></span>|<span data-ttu-id="0782f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0782f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0782f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0782f-127">Request body</span></span>
<span data-ttu-id="0782f-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0782f-128">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="0782f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="0782f-129">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="0782f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0782f-130">Property</span></span>|<span data-ttu-id="0782f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0782f-131">Type</span></span>|<span data-ttu-id="0782f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0782f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0782f-133">id</span><span class="sxs-lookup"><span data-stu-id="0782f-133">id</span></span>|<span data-ttu-id="0782f-134">String</span><span class="sxs-lookup"><span data-stu-id="0782f-134">String</span></span>|<span data-ttu-id="0782f-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0782f-135">Key of the entity.</span></span> <span data-ttu-id="0782f-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0782f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0782f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0782f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0782f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0782f-138">DateTimeOffset</span></span>|<span data-ttu-id="0782f-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0782f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0782f-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0782f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0782f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0782f-141">roleScopeTagIds</span></span>|<span data-ttu-id="0782f-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="0782f-142">String collection</span></span>|<span data-ttu-id="0782f-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="0782f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0782f-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0782f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0782f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0782f-145">supportsScopeTags</span></span>|<span data-ttu-id="0782f-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="0782f-146">Boolean</span></span>|<span data-ttu-id="0782f-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0782f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0782f-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="0782f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0782f-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="0782f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0782f-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0782f-150">This property is read-only.</span></span> <span data-ttu-id="0782f-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0782f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0782f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0782f-152">createdDateTime</span></span>|<span data-ttu-id="0782f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0782f-153">DateTimeOffset</span></span>|<span data-ttu-id="0782f-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0782f-154">DateTime the object was created.</span></span> <span data-ttu-id="0782f-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0782f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0782f-156">description</span><span class="sxs-lookup"><span data-stu-id="0782f-156">description</span></span>|<span data-ttu-id="0782f-157">String</span><span class="sxs-lookup"><span data-stu-id="0782f-157">String</span></span>|<span data-ttu-id="0782f-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0782f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0782f-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0782f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0782f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0782f-160">displayName</span></span>|<span data-ttu-id="0782f-161">String</span><span class="sxs-lookup"><span data-stu-id="0782f-161">String</span></span>|<span data-ttu-id="0782f-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0782f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0782f-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0782f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0782f-164">Version</span><span class="sxs-lookup"><span data-stu-id="0782f-164">version</span></span>|<span data-ttu-id="0782f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0782f-165">Int32</span></span>|<span data-ttu-id="0782f-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0782f-166">Version of the device configuration.</span></span> <span data-ttu-id="0782f-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0782f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0782f-168">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="0782f-168">kioskProfiles</span></span>|<span data-ttu-id="0782f-169">[WindowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0782f-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="0782f-170">Diese Richtlinie ermöglicht zum Definieren einer Liste von Kiosk-Profilen für eine Kiosk-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="0782f-170">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="0782f-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="0782f-171">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0782f-172">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="0782f-172">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="0782f-173">String</span><span class="sxs-lookup"><span data-stu-id="0782f-173">String</span></span>|<span data-ttu-id="0782f-174">Geben Sie den Standard-URL der Browser navigieren soll auf starten.</span><span class="sxs-lookup"><span data-stu-id="0782f-174">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="0782f-175">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="0782f-175">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="0782f-176">Boolesch</span><span class="sxs-lookup"><span data-stu-id="0782f-176">Boolean</span></span>|<span data-ttu-id="0782f-177">Aktivieren des Kiosk-Browsers home-Schaltfläche.</span><span class="sxs-lookup"><span data-stu-id="0782f-177">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="0782f-178">Die home-Schaltfläche ist standardmäßig deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="0782f-178">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="0782f-179">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="0782f-179">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="0782f-180">Boolesch</span><span class="sxs-lookup"><span data-stu-id="0782f-180">Boolean</span></span>|<span data-ttu-id="0782f-181">Aktivieren des Kiosk-Browsers Navigation buttons(forward/back).</span><span class="sxs-lookup"><span data-stu-id="0782f-181">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="0782f-182">Die Navigationsschaltflächen werden standardmäßig deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="0782f-182">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="0782f-183">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="0782f-183">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="0782f-184">Boolesch</span><span class="sxs-lookup"><span data-stu-id="0782f-184">Boolean</span></span>|<span data-ttu-id="0782f-185">Aktivieren des Kiosk-Browsers End Sitzung Schaltfläche.</span><span class="sxs-lookup"><span data-stu-id="0782f-185">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="0782f-186">Die Schaltfläche Beenden Sitzung ist standardmäßig deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="0782f-186">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="0782f-187">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="0782f-187">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="0782f-188">Int32</span><span class="sxs-lookup"><span data-stu-id="0782f-188">Int32</span></span>|<span data-ttu-id="0782f-189">Geben Sie die Anzahl der Minuten, die Sitzung im Leerlauf befindet, bis der Kiosk-Browser in einen neuen Status neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="0782f-189">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="0782f-190">Gültige Werte sind 1 und 1440.</span><span class="sxs-lookup"><span data-stu-id="0782f-190">Valid values are 1-1440.</span></span> <span data-ttu-id="0782f-191">Gültige Werte 1 bis 1440</span><span class="sxs-lookup"><span data-stu-id="0782f-191">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="0782f-192">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="0782f-192">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="0782f-193">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="0782f-193">String collection</span></span>|<span data-ttu-id="0782f-194">Geben Sie die URLs, die nicht die Kiosk-Browser navigieren soll</span><span class="sxs-lookup"><span data-stu-id="0782f-194">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="0782f-195">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="0782f-195">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="0782f-196">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="0782f-196">String collection</span></span>|<span data-ttu-id="0782f-197">Geben Sie die URLs, die im Browser Kiosk zulässig ist, zu dem navigiert</span><span class="sxs-lookup"><span data-stu-id="0782f-197">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|



## <a name="response"></a><span data-ttu-id="0782f-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="0782f-198">Response</span></span>
<span data-ttu-id="0782f-199">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0782f-199">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0782f-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0782f-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="0782f-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0782f-201">Request</span></span>
<span data-ttu-id="0782f-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0782f-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1598

{
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

### <a name="response"></a><span data-ttu-id="0782f-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="0782f-203">Response</span></span>
<span data-ttu-id="0782f-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0782f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





