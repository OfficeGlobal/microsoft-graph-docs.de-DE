---
title: Aktualisieren von „windows10TeamGeneralConfiguration“
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 44ea0c4f76bd95d84ecd5126bec32e988b40a6f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858366"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="5aab4-103">Aktualisieren von „windows10TeamGeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="5aab4-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="5aab4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5aab4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5aab4-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aab4-105">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5aab4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5aab4-106">Prerequisites</span></span>
<span data-ttu-id="5aab4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5aab4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5aab4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5aab4-109">Permission type</span></span>|<span data-ttu-id="5aab4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5aab4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5aab4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5aab4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5aab4-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5aab4-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5aab4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5aab4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5aab4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5aab4-114">Not supported.</span></span>|
|<span data-ttu-id="5aab4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5aab4-115">Application</span></span>|<span data-ttu-id="5aab4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5aab4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5aab4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5aab4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5aab4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5aab4-118">Request headers</span></span>
|<span data-ttu-id="5aab4-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5aab4-119">Header</span></span>|<span data-ttu-id="5aab4-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5aab4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5aab4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5aab4-121">Authorization</span></span>|<span data-ttu-id="5aab4-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5aab4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5aab4-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5aab4-123">Accept</span></span>|<span data-ttu-id="5aab4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5aab4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5aab4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5aab4-125">Request body</span></span>
<span data-ttu-id="5aab4-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="5aab4-126">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="5aab4-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5aab4-127">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="5aab4-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5aab4-128">Property</span></span>|<span data-ttu-id="5aab4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5aab4-129">Type</span></span>|<span data-ttu-id="5aab4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5aab4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5aab4-131">id</span><span class="sxs-lookup"><span data-stu-id="5aab4-131">id</span></span>|<span data-ttu-id="5aab4-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5aab4-132">String</span></span>|<span data-ttu-id="5aab4-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5aab4-133">Key of the entity.</span></span> <span data-ttu-id="5aab4-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aab4-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aab4-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5aab4-135">lastModifiedDateTime</span></span>|<span data-ttu-id="5aab4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5aab4-136">DateTimeOffset</span></span>|<span data-ttu-id="5aab4-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5aab4-137">DateTime the object was last modified.</span></span> <span data-ttu-id="5aab4-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aab4-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aab4-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5aab4-139">createdDateTime</span></span>|<span data-ttu-id="5aab4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5aab4-140">DateTimeOffset</span></span>|<span data-ttu-id="5aab4-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5aab4-141">DateTime the object was created.</span></span> <span data-ttu-id="5aab4-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aab4-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aab4-143">description</span><span class="sxs-lookup"><span data-stu-id="5aab4-143">description</span></span>|<span data-ttu-id="5aab4-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5aab4-144">String</span></span>|<span data-ttu-id="5aab4-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5aab4-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5aab4-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aab4-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aab4-147">displayName</span><span class="sxs-lookup"><span data-stu-id="5aab4-147">displayName</span></span>|<span data-ttu-id="5aab4-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5aab4-148">String</span></span>|<span data-ttu-id="5aab4-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5aab4-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5aab4-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aab4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aab4-151">Version</span><span class="sxs-lookup"><span data-stu-id="5aab4-151">version</span></span>|<span data-ttu-id="5aab4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5aab4-152">Int32</span></span>|<span data-ttu-id="5aab4-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5aab4-153">Version of the device configuration.</span></span> <span data-ttu-id="5aab4-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5aab4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5aab4-155">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="5aab4-155">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="5aab4-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aab4-156">Boolean</span></span>|<span data-ttu-id="5aab4-157">Gibt an, ob Azure Operational Insights blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="5aab4-157">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="5aab4-158">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="5aab4-158">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="5aab4-159">String</span><span class="sxs-lookup"><span data-stu-id="5aab4-159">String</span></span>|<span data-ttu-id="5aab4-160">ID des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="5aab4-160">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="5aab4-161">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="5aab4-161">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="5aab4-162">String</span><span class="sxs-lookup"><span data-stu-id="5aab4-162">String</span></span>|<span data-ttu-id="5aab4-163">Schlüssel des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="5aab4-163">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="5aab4-164">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="5aab4-164">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="5aab4-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aab4-165">Boolean</span></span>|<span data-ttu-id="5aab4-166">Gibt an, ob die App „Verbinden“ automatisch gestartet werden soll, sobald eine Projektion initiiert wird.</span><span class="sxs-lookup"><span data-stu-id="5aab4-166">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="5aab4-167">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="5aab4-167">maintenanceWindowBlocked</span></span>|<span data-ttu-id="5aab4-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aab4-168">Boolean</span></span>|<span data-ttu-id="5aab4-169">Gibt an, ob ein Wartungsfenster für Geräteupdates festgelegt werden darf.</span><span class="sxs-lookup"><span data-stu-id="5aab4-169">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="5aab4-170">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="5aab4-170">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="5aab4-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5aab4-171">Int32</span></span>|<span data-ttu-id="5aab4-172">Dauer des Wartungsfensters für Geräteupdates.</span><span class="sxs-lookup"><span data-stu-id="5aab4-172">Maintenance window duration for device updates.</span></span> <span data-ttu-id="5aab4-173">Gültige Werte: 0 bis 5.</span><span class="sxs-lookup"><span data-stu-id="5aab4-173">Valid values 0 to 5</span></span>|
|<span data-ttu-id="5aab4-174">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="5aab4-174">maintenanceWindowStartTime</span></span>|<span data-ttu-id="5aab4-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5aab4-175">TimeOfDay</span></span>|<span data-ttu-id="5aab4-176">Beginn des Wartungsfensters für Geräteupdates</span><span class="sxs-lookup"><span data-stu-id="5aab4-176">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="5aab4-177">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="5aab4-177">miracastChannel</span></span>|[<span data-ttu-id="5aab4-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="5aab4-178">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="5aab4-179">Kanal.</span><span class="sxs-lookup"><span data-stu-id="5aab4-179">The channel.</span></span> <span data-ttu-id="5aab4-180">Mögliche Werte sind: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne` und `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="5aab4-180">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="5aab4-181">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="5aab4-181">miracastBlocked</span></span>|<span data-ttu-id="5aab4-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aab4-182">Boolean</span></span>|<span data-ttu-id="5aab4-183">Gibt an, ob eine drahtlose Projektion erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="5aab4-183">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="5aab4-184">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="5aab4-184">miracastRequirePin</span></span>|<span data-ttu-id="5aab4-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aab4-185">Boolean</span></span>|<span data-ttu-id="5aab4-186">Gibt an, ob für eine drahtlose Projektion die Eingabe einer PIN erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="5aab4-186">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="5aab4-187">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="5aab4-187">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="5aab4-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aab4-188">Boolean</span></span>|<span data-ttu-id="5aab4-189">Gibt an, ob die Funktion „Meine Besprechungen und Dateien“ im Startmenü deaktiviert werden soll. In diesem Bereich werden die Office 365-Besprechungen und -Dateien des angemeldeten Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="5aab4-189">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="5aab4-190">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="5aab4-190">settingsBlockSessionResume</span></span>|<span data-ttu-id="5aab4-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aab4-191">Boolean</span></span>|<span data-ttu-id="5aab4-192">Gibt an, ob Sitzungen nach einem Sitzungstimeout fortgeführt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="5aab4-192">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="5aab4-193">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="5aab4-193">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="5aab4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aab4-194">Boolean</span></span>|<span data-ttu-id="5aab4-195">Gibt an, ob das Anmeldedialogfeld automatisch mit den Eingeladenen aus geplanten Besprechungen befüllt werden darf.</span><span class="sxs-lookup"><span data-stu-id="5aab4-195">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="5aab4-196">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="5aab4-196">settingsDefaultVolume</span></span>|<span data-ttu-id="5aab4-197">Int32</span><span class="sxs-lookup"><span data-stu-id="5aab4-197">Int32</span></span>|<span data-ttu-id="5aab4-198">Legt die Standardlautstärke für neue Sitzungen fest.</span><span class="sxs-lookup"><span data-stu-id="5aab4-198">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="5aab4-199">Zulässige Werte sind 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="5aab4-199">Permitted values are 0-100.</span></span> <span data-ttu-id="5aab4-200">Der Standardwert lautet 45.</span><span class="sxs-lookup"><span data-stu-id="5aab4-200">The default is 45.</span></span> <span data-ttu-id="5aab4-201">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="5aab4-201">Valid values 0 to 100</span></span>|
|<span data-ttu-id="5aab4-202">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="5aab4-202">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="5aab4-203">Int32</span><span class="sxs-lookup"><span data-stu-id="5aab4-203">Int32</span></span>|<span data-ttu-id="5aab4-204">Gibt den Zeitraum in Minuten an, nach dem der Bildschirm des Hub-Systems abgeschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="5aab4-204">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="5aab4-205">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="5aab4-205">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="5aab4-206">Int32</span><span class="sxs-lookup"><span data-stu-id="5aab4-206">Int32</span></span>|<span data-ttu-id="5aab4-207">Gibt den Zeitraum in Minuten an, nach dem es zu einem Sitzungstimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="5aab4-207">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="5aab4-208">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="5aab4-208">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="5aab4-209">Int32</span><span class="sxs-lookup"><span data-stu-id="5aab4-209">Int32</span></span>|<span data-ttu-id="5aab4-210">Gibt den Zeitraum in Minuten an, nach dem das Hub-System in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="5aab4-210">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="5aab4-211">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="5aab4-211">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="5aab4-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aab4-212">Boolean</span></span>|<span data-ttu-id="5aab4-213">Gibt an, ob der Willkommensbildschirm automatisch angezeigt werden soll, sobald jemand den Raum betritt.</span><span class="sxs-lookup"><span data-stu-id="5aab4-213">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="5aab4-214">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="5aab4-214">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="5aab4-215">String</span><span class="sxs-lookup"><span data-stu-id="5aab4-215">String</span></span>|<span data-ttu-id="5aab4-216">URL zum Hintergrundbild für den Willkommensbildschirm.</span><span class="sxs-lookup"><span data-stu-id="5aab4-216">The welcome screen background image URL.</span></span> <span data-ttu-id="5aab4-217">Die URL muss das HTTPS-Protokoll verwenden und ein PNG-Bild zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="5aab4-217">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="5aab4-218">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="5aab4-218">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="5aab4-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="5aab4-219">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="5aab4-220">Die Informationen, die im Willkommensbildschirm angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5aab4-220">The welcome screen meeting information shown.</span></span> <span data-ttu-id="5aab4-221">Mögliche Werte sind: `userDefined`, `showOrganizerAndTimeOnly` und `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="5aab4-221">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="5aab4-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="5aab4-222">Response</span></span>
<span data-ttu-id="5aab4-223">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5aab4-223">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5aab4-224">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5aab4-224">Example</span></span>
### <a name="request"></a><span data-ttu-id="5aab4-225">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5aab4-225">Request</span></span>
<span data-ttu-id="5aab4-226">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5aab4-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1150

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a><span data-ttu-id="5aab4-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="5aab4-227">Response</span></span>
<span data-ttu-id="5aab4-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5aab4-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1322

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```



