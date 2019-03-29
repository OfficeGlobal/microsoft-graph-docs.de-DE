---
title: Aktualisieren von „windows10TeamGeneralConfiguration“
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf291aab92197a4d0ab54bbc578e01766bf35eb2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967958"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="7b9fd-103">Aktualisieren von „windows10TeamGeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="7b9fd-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="7b9fd-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b9fd-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b9fd-105">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b9fd-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7b9fd-106">Prerequisites</span></span>
<span data-ttu-id="7b9fd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b9fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b9fd-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b9fd-109">Permission type</span></span>|<span data-ttu-id="7b9fd-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b9fd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b9fd-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b9fd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7b9fd-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b9fd-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b9fd-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b9fd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b9fd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b9fd-114">Not supported.</span></span>|
|<span data-ttu-id="7b9fd-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b9fd-115">Application</span></span>|<span data-ttu-id="7b9fd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b9fd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b9fd-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b9fd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7b9fd-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b9fd-118">Request headers</span></span>
|<span data-ttu-id="7b9fd-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7b9fd-119">Header</span></span>|<span data-ttu-id="7b9fd-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7b9fd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b9fd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b9fd-121">Authorization</span></span>|<span data-ttu-id="7b9fd-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7b9fd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b9fd-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7b9fd-123">Accept</span></span>|<span data-ttu-id="7b9fd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7b9fd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b9fd-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b9fd-125">Request body</span></span>
<span data-ttu-id="7b9fd-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-126">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="7b9fd-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-127">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="7b9fd-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7b9fd-128">Property</span></span>|<span data-ttu-id="7b9fd-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7b9fd-129">Type</span></span>|<span data-ttu-id="7b9fd-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b9fd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b9fd-131">id</span><span class="sxs-lookup"><span data-stu-id="7b9fd-131">id</span></span>|<span data-ttu-id="7b9fd-132">String</span><span class="sxs-lookup"><span data-stu-id="7b9fd-132">String</span></span>|<span data-ttu-id="7b9fd-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7b9fd-133">Key of the entity.</span></span> <span data-ttu-id="7b9fd-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b9fd-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b9fd-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b9fd-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7b9fd-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b9fd-136">DateTimeOffset</span></span>|<span data-ttu-id="7b9fd-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-137">DateTime the object was last modified.</span></span> <span data-ttu-id="7b9fd-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b9fd-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b9fd-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b9fd-139">createdDateTime</span></span>|<span data-ttu-id="7b9fd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b9fd-140">DateTimeOffset</span></span>|<span data-ttu-id="7b9fd-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-141">DateTime the object was created.</span></span> <span data-ttu-id="7b9fd-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b9fd-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b9fd-143">description</span><span class="sxs-lookup"><span data-stu-id="7b9fd-143">description</span></span>|<span data-ttu-id="7b9fd-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7b9fd-144">String</span></span>|<span data-ttu-id="7b9fd-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7b9fd-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b9fd-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b9fd-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b9fd-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7b9fd-147">displayName</span></span>|<span data-ttu-id="7b9fd-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7b9fd-148">String</span></span>|<span data-ttu-id="7b9fd-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7b9fd-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b9fd-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b9fd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b9fd-151">Version</span><span class="sxs-lookup"><span data-stu-id="7b9fd-151">version</span></span>|<span data-ttu-id="7b9fd-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7b9fd-152">Int32</span></span>|<span data-ttu-id="7b9fd-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-153">Version of the device configuration.</span></span> <span data-ttu-id="7b9fd-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b9fd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b9fd-155">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="7b9fd-155">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="7b9fd-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7b9fd-156">Boolean</span></span>|<span data-ttu-id="7b9fd-157">Gibt an, ob Azure Operational Insights blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-157">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="7b9fd-158">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="7b9fd-158">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="7b9fd-159">String</span><span class="sxs-lookup"><span data-stu-id="7b9fd-159">String</span></span>|<span data-ttu-id="7b9fd-160">ID des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="7b9fd-160">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="7b9fd-161">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="7b9fd-161">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="7b9fd-162">String</span><span class="sxs-lookup"><span data-stu-id="7b9fd-162">String</span></span>|<span data-ttu-id="7b9fd-163">Schlüssel des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="7b9fd-163">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="7b9fd-164">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="7b9fd-164">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="7b9fd-165">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7b9fd-165">Boolean</span></span>|<span data-ttu-id="7b9fd-166">Gibt an, ob die App „Verbinden“ automatisch gestartet werden soll, sobald eine Projektion initiiert wird.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-166">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="7b9fd-167">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="7b9fd-167">maintenanceWindowBlocked</span></span>|<span data-ttu-id="7b9fd-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7b9fd-168">Boolean</span></span>|<span data-ttu-id="7b9fd-169">Gibt an, ob ein Wartungsfenster für Geräteupdates festgelegt werden darf.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-169">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="7b9fd-170">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="7b9fd-170">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="7b9fd-171">Int32</span><span class="sxs-lookup"><span data-stu-id="7b9fd-171">Int32</span></span>|<span data-ttu-id="7b9fd-172">Dauer des Wartungsfensters für Geräteupdates.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-172">Maintenance window duration for device updates.</span></span> <span data-ttu-id="7b9fd-173">Gültige Werte: 0 bis 5.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-173">Valid values 0 to 5</span></span>|
|<span data-ttu-id="7b9fd-174">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="7b9fd-174">maintenanceWindowStartTime</span></span>|<span data-ttu-id="7b9fd-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7b9fd-175">TimeOfDay</span></span>|<span data-ttu-id="7b9fd-176">Beginn des Wartungsfensters für Geräteupdates</span><span class="sxs-lookup"><span data-stu-id="7b9fd-176">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="7b9fd-177">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="7b9fd-177">miracastChannel</span></span>|[<span data-ttu-id="7b9fd-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="7b9fd-178">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="7b9fd-179">Kanal.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-179">The channel.</span></span> <span data-ttu-id="7b9fd-180">Mögliche Werte sind: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne` und `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-180">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="7b9fd-181">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="7b9fd-181">miracastBlocked</span></span>|<span data-ttu-id="7b9fd-182">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7b9fd-182">Boolean</span></span>|<span data-ttu-id="7b9fd-183">Gibt an, ob eine drahtlose Projektion erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-183">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="7b9fd-184">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="7b9fd-184">miracastRequirePin</span></span>|<span data-ttu-id="7b9fd-185">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7b9fd-185">Boolean</span></span>|<span data-ttu-id="7b9fd-186">Gibt an, ob für eine drahtlose Projektion die Eingabe einer PIN erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-186">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="7b9fd-187">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="7b9fd-187">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="7b9fd-188">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7b9fd-188">Boolean</span></span>|<span data-ttu-id="7b9fd-189">Gibt an, ob die Funktion „Meine Besprechungen und Dateien“ im Startmenü deaktiviert werden soll. In diesem Bereich werden die Office 365-Besprechungen und -Dateien des angemeldeten Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-189">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="7b9fd-190">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="7b9fd-190">settingsBlockSessionResume</span></span>|<span data-ttu-id="7b9fd-191">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7b9fd-191">Boolean</span></span>|<span data-ttu-id="7b9fd-192">Gibt an, ob Sitzungen nach einem Sitzungstimeout fortgeführt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-192">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="7b9fd-193">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="7b9fd-193">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="7b9fd-194">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7b9fd-194">Boolean</span></span>|<span data-ttu-id="7b9fd-195">Gibt an, ob das Anmeldedialogfeld automatisch mit den Eingeladenen aus geplanten Besprechungen befüllt werden darf.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-195">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="7b9fd-196">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="7b9fd-196">settingsDefaultVolume</span></span>|<span data-ttu-id="7b9fd-197">Int32</span><span class="sxs-lookup"><span data-stu-id="7b9fd-197">Int32</span></span>|<span data-ttu-id="7b9fd-198">Legt die Standardlautstärke für neue Sitzungen fest.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-198">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="7b9fd-199">Zulässige Werte sind 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-199">Permitted values are 0-100.</span></span> <span data-ttu-id="7b9fd-200">Der Standardwert lautet 45.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-200">The default is 45.</span></span> <span data-ttu-id="7b9fd-201">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-201">Valid values 0 to 100</span></span>|
|<span data-ttu-id="7b9fd-202">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7b9fd-202">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="7b9fd-203">Int32</span><span class="sxs-lookup"><span data-stu-id="7b9fd-203">Int32</span></span>|<span data-ttu-id="7b9fd-204">Gibt den Zeitraum in Minuten an, nach dem der Bildschirm des Hub-Systems abgeschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-204">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="7b9fd-205">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7b9fd-205">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="7b9fd-206">Int32</span><span class="sxs-lookup"><span data-stu-id="7b9fd-206">Int32</span></span>|<span data-ttu-id="7b9fd-207">Gibt den Zeitraum in Minuten an, nach dem es zu einem Sitzungstimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-207">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="7b9fd-208">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7b9fd-208">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="7b9fd-209">Int32</span><span class="sxs-lookup"><span data-stu-id="7b9fd-209">Int32</span></span>|<span data-ttu-id="7b9fd-210">Gibt den Zeitraum in Minuten an, nach dem das Hub-System in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-210">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="7b9fd-211">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="7b9fd-211">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="7b9fd-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b9fd-212">Boolean</span></span>|<span data-ttu-id="7b9fd-213">Gibt an, ob der Willkommensbildschirm automatisch angezeigt werden soll, sobald jemand den Raum betritt.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-213">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="7b9fd-214">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="7b9fd-214">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="7b9fd-215">String</span><span class="sxs-lookup"><span data-stu-id="7b9fd-215">String</span></span>|<span data-ttu-id="7b9fd-216">URL zum Hintergrundbild für den Willkommensbildschirm.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-216">The welcome screen background image URL.</span></span> <span data-ttu-id="7b9fd-217">Die URL muss das HTTPS-Protokoll verwenden und ein PNG-Bild zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-217">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="7b9fd-218">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="7b9fd-218">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="7b9fd-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="7b9fd-219">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="7b9fd-220">Die Informationen, die im Willkommensbildschirm angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-220">The welcome screen meeting information shown.</span></span> <span data-ttu-id="7b9fd-221">Mögliche Werte sind: `userDefined`, `showOrganizerAndTimeOnly` und `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-221">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="7b9fd-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b9fd-222">Response</span></span>
<span data-ttu-id="7b9fd-223">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-223">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b9fd-224">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b9fd-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b9fd-225">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b9fd-225">Request</span></span>
<span data-ttu-id="7b9fd-226">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-226">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7b9fd-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b9fd-227">Response</span></span>
<span data-ttu-id="7b9fd-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b9fd-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



