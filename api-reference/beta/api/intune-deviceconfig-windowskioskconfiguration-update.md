---
title: WindowsKioskConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsKioskConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 767acd4136226e2687977cf09d2c08f6c413fcb8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414886"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="474d3-103">WindowsKioskConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="474d3-103">Update windowsKioskConfiguration</span></span>

> <span data-ttu-id="474d3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="474d3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="474d3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="474d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="474d3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="474d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="474d3-107">Aktualisieren Sie die Eigenschaften eines [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="474d3-107">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="474d3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="474d3-108">Prerequisites</span></span>
<span data-ttu-id="474d3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="474d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="474d3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="474d3-111">Permission type</span></span>|<span data-ttu-id="474d3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="474d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="474d3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="474d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="474d3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="474d3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="474d3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="474d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="474d3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="474d3-116">Not supported.</span></span>|
|<span data-ttu-id="474d3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="474d3-117">Application</span></span>|<span data-ttu-id="474d3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="474d3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="474d3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="474d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="474d3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="474d3-120">Request headers</span></span>
|<span data-ttu-id="474d3-121">Header</span><span class="sxs-lookup"><span data-stu-id="474d3-121">Header</span></span>|<span data-ttu-id="474d3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="474d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="474d3-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="474d3-123">Authorization</span></span>|<span data-ttu-id="474d3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="474d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="474d3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="474d3-125">Accept</span></span>|<span data-ttu-id="474d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="474d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="474d3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="474d3-127">Request body</span></span>
<span data-ttu-id="474d3-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="474d3-128">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="474d3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="474d3-129">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="474d3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="474d3-130">Property</span></span>|<span data-ttu-id="474d3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="474d3-131">Type</span></span>|<span data-ttu-id="474d3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="474d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="474d3-133">id</span><span class="sxs-lookup"><span data-stu-id="474d3-133">id</span></span>|<span data-ttu-id="474d3-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="474d3-134">String</span></span>|<span data-ttu-id="474d3-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="474d3-135">Key of the entity.</span></span> <span data-ttu-id="474d3-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="474d3-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474d3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="474d3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="474d3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="474d3-138">DateTimeOffset</span></span>|<span data-ttu-id="474d3-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="474d3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="474d3-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="474d3-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474d3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="474d3-141">roleScopeTagIds</span></span>|<span data-ttu-id="474d3-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="474d3-142">String collection</span></span>|<span data-ttu-id="474d3-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="474d3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="474d3-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="474d3-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474d3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="474d3-145">supportsScopeTags</span></span>|<span data-ttu-id="474d3-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="474d3-146">Boolean</span></span>|<span data-ttu-id="474d3-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="474d3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="474d3-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="474d3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="474d3-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="474d3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="474d3-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="474d3-150">This property is read-only.</span></span> <span data-ttu-id="474d3-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="474d3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474d3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="474d3-152">createdDateTime</span></span>|<span data-ttu-id="474d3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="474d3-153">DateTimeOffset</span></span>|<span data-ttu-id="474d3-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="474d3-154">DateTime the object was created.</span></span> <span data-ttu-id="474d3-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="474d3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474d3-156">description</span><span class="sxs-lookup"><span data-stu-id="474d3-156">description</span></span>|<span data-ttu-id="474d3-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="474d3-157">String</span></span>|<span data-ttu-id="474d3-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="474d3-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="474d3-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="474d3-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474d3-160">displayName</span><span class="sxs-lookup"><span data-stu-id="474d3-160">displayName</span></span>|<span data-ttu-id="474d3-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="474d3-161">String</span></span>|<span data-ttu-id="474d3-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="474d3-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="474d3-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="474d3-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474d3-164">Version</span><span class="sxs-lookup"><span data-stu-id="474d3-164">version</span></span>|<span data-ttu-id="474d3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="474d3-165">Int32</span></span>|<span data-ttu-id="474d3-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="474d3-166">Version of the device configuration.</span></span> <span data-ttu-id="474d3-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="474d3-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="474d3-168">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="474d3-168">kioskProfiles</span></span>|<span data-ttu-id="474d3-169">[WindowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="474d3-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="474d3-170">Diese Richtlinie ermöglicht zum Definieren einer Liste von Kiosk-Profilen für eine Kiosk-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="474d3-170">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="474d3-171">Diese Sammlung kann maximal 3 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="474d3-171">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="474d3-172">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="474d3-172">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="474d3-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="474d3-173">String</span></span>|<span data-ttu-id="474d3-174">Geben Sie den Standard-URL der Browser navigieren soll auf starten.</span><span class="sxs-lookup"><span data-stu-id="474d3-174">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="474d3-175">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="474d3-175">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="474d3-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="474d3-176">Boolean</span></span>|<span data-ttu-id="474d3-177">Aktivieren des Kiosk-Browsers home-Schaltfläche.</span><span class="sxs-lookup"><span data-stu-id="474d3-177">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="474d3-178">Die home-Schaltfläche ist standardmäßig deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="474d3-178">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="474d3-179">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="474d3-179">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="474d3-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="474d3-180">Boolean</span></span>|<span data-ttu-id="474d3-181">Aktivieren des Kiosk-Browsers Navigation buttons(forward/back).</span><span class="sxs-lookup"><span data-stu-id="474d3-181">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="474d3-182">Die Navigationsschaltflächen werden standardmäßig deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="474d3-182">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="474d3-183">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="474d3-183">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="474d3-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="474d3-184">Boolean</span></span>|<span data-ttu-id="474d3-185">Aktivieren des Kiosk-Browsers End Sitzung Schaltfläche.</span><span class="sxs-lookup"><span data-stu-id="474d3-185">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="474d3-186">Die Schaltfläche Beenden Sitzung ist standardmäßig deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="474d3-186">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="474d3-187">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="474d3-187">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="474d3-188">Int32</span><span class="sxs-lookup"><span data-stu-id="474d3-188">Int32</span></span>|<span data-ttu-id="474d3-189">Geben Sie die Anzahl der Minuten, die Sitzung im Leerlauf befindet, bis der Kiosk-Browser in einen neuen Status neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="474d3-189">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="474d3-190">Gültige Werte sind 1 und 1440.</span><span class="sxs-lookup"><span data-stu-id="474d3-190">Valid values are 1-1440.</span></span> <span data-ttu-id="474d3-191">Gültige Werte 1 bis 1440</span><span class="sxs-lookup"><span data-stu-id="474d3-191">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="474d3-192">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="474d3-192">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="474d3-193">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="474d3-193">String collection</span></span>|<span data-ttu-id="474d3-194">Geben Sie die URLs, die nicht die Kiosk-Browser navigieren soll</span><span class="sxs-lookup"><span data-stu-id="474d3-194">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="474d3-195">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="474d3-195">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="474d3-196">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="474d3-196">String collection</span></span>|<span data-ttu-id="474d3-197">Geben Sie die URLs, die im Browser Kiosk zulässig ist, zu dem navigiert</span><span class="sxs-lookup"><span data-stu-id="474d3-197">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="474d3-198">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="474d3-198">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="474d3-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="474d3-199">Boolean</span></span>|<span data-ttu-id="474d3-200">Aktivieren Sie öffentliche browsing Kioskmodus für den Microsoft-Edge-Browser.</span><span class="sxs-lookup"><span data-stu-id="474d3-200">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="474d3-201">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="474d3-201">The Default is false.</span></span>|
|<span data-ttu-id="474d3-202">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="474d3-202">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="474d3-203">Int32</span><span class="sxs-lookup"><span data-stu-id="474d3-203">Int32</span></span>|<span data-ttu-id="474d3-204">Gibt die Zeitspanne in Minuten aus der letzten Benutzeraktivität, bevor Microsoft Edge Kiosk zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="474d3-204">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="474d3-205">Gültige Werte sind 0 und 1440.</span><span class="sxs-lookup"><span data-stu-id="474d3-205">Valid values are 0-1440.</span></span> <span data-ttu-id="474d3-206">Der Standardwert ist 5.</span><span class="sxs-lookup"><span data-stu-id="474d3-206">The default is 5.</span></span> <span data-ttu-id="474d3-207">0 gibt keine zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="474d3-207">0 indicates no reset.</span></span> <span data-ttu-id="474d3-208">Gültige Werte von 0 bis 1440</span><span class="sxs-lookup"><span data-stu-id="474d3-208">Valid values 0 to 1440</span></span>|



## <a name="response"></a><span data-ttu-id="474d3-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="474d3-209">Response</span></span>
<span data-ttu-id="474d3-210">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="474d3-210">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="474d3-211">Beispiel</span><span class="sxs-lookup"><span data-stu-id="474d3-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="474d3-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="474d3-212">Request</span></span>
<span data-ttu-id="474d3-213">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="474d3-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="474d3-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="474d3-214">Response</span></span>
<span data-ttu-id="474d3-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="474d3-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




