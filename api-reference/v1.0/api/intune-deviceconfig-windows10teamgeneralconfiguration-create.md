---
title: windows10TeamGeneralConfiguration erstellen
description: Erstellt neue Objekte des Typs windows10TeamGeneralConfiguration.
author: tfitzmac
ms.openlocfilehash: 1634de20684f751dbb540b2fa619cd9153d8b0f1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340292"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="9d65a-103">windows10TeamGeneralConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="9d65a-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="9d65a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9d65a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d65a-105">Erstellt neue Objekte des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d65a-105">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d65a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9d65a-106">Prerequisites</span></span>
<span data-ttu-id="9d65a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d65a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d65a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d65a-109">Permission type</span></span>|<span data-ttu-id="9d65a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d65a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d65a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d65a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9d65a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d65a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d65a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d65a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d65a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d65a-114">Not supported.</span></span>|
|<span data-ttu-id="9d65a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d65a-115">Application</span></span>|<span data-ttu-id="9d65a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d65a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d65a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d65a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9d65a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d65a-118">Request headers</span></span>
|<span data-ttu-id="9d65a-119">Header</span><span class="sxs-lookup"><span data-stu-id="9d65a-119">Header</span></span>|<span data-ttu-id="9d65a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9d65a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d65a-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9d65a-121">Authorization</span></span>|<span data-ttu-id="9d65a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9d65a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d65a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9d65a-123">Accept</span></span>|<span data-ttu-id="9d65a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9d65a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d65a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d65a-125">Request body</span></span>
<span data-ttu-id="9d65a-126">Geben Sie im Anforderungstext eine JSON-Darstellung des windows10TeamGeneralConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="9d65a-126">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="9d65a-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10TeamGeneralConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9d65a-127">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="9d65a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9d65a-128">Property</span></span>|<span data-ttu-id="9d65a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9d65a-129">Type</span></span>|<span data-ttu-id="9d65a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d65a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d65a-131">id</span><span class="sxs-lookup"><span data-stu-id="9d65a-131">id</span></span>|<span data-ttu-id="9d65a-132">String</span><span class="sxs-lookup"><span data-stu-id="9d65a-132">String</span></span>|<span data-ttu-id="9d65a-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9d65a-133">Key of the entity.</span></span> <span data-ttu-id="9d65a-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d65a-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d65a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d65a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="9d65a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d65a-136">DateTimeOffset</span></span>|<span data-ttu-id="9d65a-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9d65a-137">DateTime the object was last modified.</span></span> <span data-ttu-id="9d65a-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d65a-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d65a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d65a-139">createdDateTime</span></span>|<span data-ttu-id="9d65a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d65a-140">DateTimeOffset</span></span>|<span data-ttu-id="9d65a-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9d65a-141">DateTime the object was created.</span></span> <span data-ttu-id="9d65a-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d65a-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d65a-143">description</span><span class="sxs-lookup"><span data-stu-id="9d65a-143">description</span></span>|<span data-ttu-id="9d65a-144">String</span><span class="sxs-lookup"><span data-stu-id="9d65a-144">String</span></span>|<span data-ttu-id="9d65a-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9d65a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9d65a-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d65a-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d65a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="9d65a-147">displayName</span></span>|<span data-ttu-id="9d65a-148">String</span><span class="sxs-lookup"><span data-stu-id="9d65a-148">String</span></span>|<span data-ttu-id="9d65a-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9d65a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9d65a-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d65a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d65a-151">Version</span><span class="sxs-lookup"><span data-stu-id="9d65a-151">version</span></span>|<span data-ttu-id="9d65a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9d65a-152">Int32</span></span>|<span data-ttu-id="9d65a-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9d65a-153">Version of the device configuration.</span></span> <span data-ttu-id="9d65a-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d65a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d65a-155">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="9d65a-155">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="9d65a-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d65a-156">Boolean</span></span>|<span data-ttu-id="9d65a-157">Gibt an, ob Azure Operational Insights blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9d65a-157">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="9d65a-158">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="9d65a-158">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="9d65a-159">String</span><span class="sxs-lookup"><span data-stu-id="9d65a-159">String</span></span>|<span data-ttu-id="9d65a-160">ID des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="9d65a-160">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="9d65a-161">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="9d65a-161">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="9d65a-162">String</span><span class="sxs-lookup"><span data-stu-id="9d65a-162">String</span></span>|<span data-ttu-id="9d65a-163">Schlüssel des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="9d65a-163">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="9d65a-164">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="9d65a-164">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="9d65a-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d65a-165">Boolean</span></span>|<span data-ttu-id="9d65a-166">Gibt an, ob die App „Verbinden“ automatisch gestartet werden soll, sobald eine Projektion initiiert wird.</span><span class="sxs-lookup"><span data-stu-id="9d65a-166">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="9d65a-167">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="9d65a-167">maintenanceWindowBlocked</span></span>|<span data-ttu-id="9d65a-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d65a-168">Boolean</span></span>|<span data-ttu-id="9d65a-169">Gibt an, ob ein Wartungsfenster für Geräteupdates festgelegt werden darf.</span><span class="sxs-lookup"><span data-stu-id="9d65a-169">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="9d65a-170">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="9d65a-170">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="9d65a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="9d65a-171">Int32</span></span>|<span data-ttu-id="9d65a-172">Dauer des Wartungsfensters für Geräteupdates.</span><span class="sxs-lookup"><span data-stu-id="9d65a-172">Maintenance window duration for device updates.</span></span> <span data-ttu-id="9d65a-173">Gültige Werte: 0 bis 5.</span><span class="sxs-lookup"><span data-stu-id="9d65a-173">Valid values 0 to 5</span></span>|
|<span data-ttu-id="9d65a-174">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="9d65a-174">maintenanceWindowStartTime</span></span>|<span data-ttu-id="9d65a-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9d65a-175">TimeOfDay</span></span>|<span data-ttu-id="9d65a-176">Beginn des Wartungsfensters für Geräteupdates</span><span class="sxs-lookup"><span data-stu-id="9d65a-176">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="9d65a-177">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="9d65a-177">miracastChannel</span></span>|[<span data-ttu-id="9d65a-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="9d65a-178">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="9d65a-179">Kanal.</span><span class="sxs-lookup"><span data-stu-id="9d65a-179">The channel.</span></span> <span data-ttu-id="9d65a-180">Mögliche Werte sind: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne` und `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="9d65a-180">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="9d65a-181">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="9d65a-181">miracastBlocked</span></span>|<span data-ttu-id="9d65a-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d65a-182">Boolean</span></span>|<span data-ttu-id="9d65a-183">Gibt an, ob eine drahtlose Projektion erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="9d65a-183">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="9d65a-184">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="9d65a-184">miracastRequirePin</span></span>|<span data-ttu-id="9d65a-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d65a-185">Boolean</span></span>|<span data-ttu-id="9d65a-186">Gibt an, ob für eine drahtlose Projektion die Eingabe einer PIN erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="9d65a-186">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="9d65a-187">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="9d65a-187">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="9d65a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d65a-188">Boolean</span></span>|<span data-ttu-id="9d65a-189">Gibt an, ob die Funktion „Meine Besprechungen und Dateien“ im Startmenü deaktiviert werden soll. In diesem Bereich werden die Office 365-Besprechungen und -Dateien des angemeldeten Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9d65a-189">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="9d65a-190">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="9d65a-190">settingsBlockSessionResume</span></span>|<span data-ttu-id="9d65a-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d65a-191">Boolean</span></span>|<span data-ttu-id="9d65a-192">Gibt an, ob Sitzungen nach einem Sitzungstimeout fortgeführt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="9d65a-192">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="9d65a-193">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="9d65a-193">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="9d65a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d65a-194">Boolean</span></span>|<span data-ttu-id="9d65a-195">Gibt an, ob das Anmeldedialogfeld automatisch mit den Eingeladenen aus geplanten Besprechungen befüllt werden darf.</span><span class="sxs-lookup"><span data-stu-id="9d65a-195">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="9d65a-196">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="9d65a-196">settingsDefaultVolume</span></span>|<span data-ttu-id="9d65a-197">Int32</span><span class="sxs-lookup"><span data-stu-id="9d65a-197">Int32</span></span>|<span data-ttu-id="9d65a-198">Legt die Standardlautstärke für neue Sitzungen fest.</span><span class="sxs-lookup"><span data-stu-id="9d65a-198">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="9d65a-199">Zulässige Werte sind 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="9d65a-199">Permitted values are 0-100.</span></span> <span data-ttu-id="9d65a-200">Der Standardwert lautet 45.</span><span class="sxs-lookup"><span data-stu-id="9d65a-200">The default is 45.</span></span> <span data-ttu-id="9d65a-201">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="9d65a-201">Valid values 0 to 100</span></span>|
|<span data-ttu-id="9d65a-202">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="9d65a-202">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="9d65a-203">Int32</span><span class="sxs-lookup"><span data-stu-id="9d65a-203">Int32</span></span>|<span data-ttu-id="9d65a-204">Gibt den Zeitraum in Minuten an, nach dem der Bildschirm des Hub-Systems abgeschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="9d65a-204">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="9d65a-205">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="9d65a-205">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="9d65a-206">Int32</span><span class="sxs-lookup"><span data-stu-id="9d65a-206">Int32</span></span>|<span data-ttu-id="9d65a-207">Gibt den Zeitraum in Minuten an, nach dem es zu einem Sitzungstimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="9d65a-207">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="9d65a-208">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="9d65a-208">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="9d65a-209">Int32</span><span class="sxs-lookup"><span data-stu-id="9d65a-209">Int32</span></span>|<span data-ttu-id="9d65a-210">Gibt den Zeitraum in Minuten an, nach dem das Hub-System in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="9d65a-210">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="9d65a-211">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="9d65a-211">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="9d65a-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d65a-212">Boolean</span></span>|<span data-ttu-id="9d65a-213">Gibt an, ob der Willkommensbildschirm automatisch angezeigt werden soll, sobald jemand den Raum betritt.</span><span class="sxs-lookup"><span data-stu-id="9d65a-213">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="9d65a-214">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="9d65a-214">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="9d65a-215">String</span><span class="sxs-lookup"><span data-stu-id="9d65a-215">String</span></span>|<span data-ttu-id="9d65a-216">URL zum Hintergrundbild für den Willkommensbildschirm.</span><span class="sxs-lookup"><span data-stu-id="9d65a-216">The welcome screen background image URL.</span></span> <span data-ttu-id="9d65a-217">Die URL muss das HTTPS-Protokoll verwenden und ein PNG-Bild zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="9d65a-217">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="9d65a-218">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="9d65a-218">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="9d65a-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="9d65a-219">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="9d65a-220">Die Informationen, die im Willkommensbildschirm angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9d65a-220">The welcome screen meeting information shown.</span></span> <span data-ttu-id="9d65a-221">Mögliche Werte sind: `userDefined`, `showOrganizerAndTimeOnly` und `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="9d65a-221">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="9d65a-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d65a-222">Response</span></span>
<span data-ttu-id="9d65a-223">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9d65a-223">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d65a-224">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d65a-224">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d65a-225">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d65a-225">Request</span></span>
<span data-ttu-id="9d65a-226">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9d65a-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="9d65a-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d65a-227">Response</span></span>
<span data-ttu-id="9d65a-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d65a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



