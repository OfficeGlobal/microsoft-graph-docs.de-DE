# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="fa266-101">windows10TeamGeneralConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="fa266-101">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="fa266-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fa266-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa266-103">Erstellt neue Objekte des Typs [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa266-103">Create a new [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa266-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa266-104">Prerequisites</span></span>
<span data-ttu-id="fa266-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa266-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fa266-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa266-107">Permission type</span></span>|<span data-ttu-id="fa266-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa266-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa266-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa266-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fa266-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa266-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa266-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa266-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa266-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa266-112">Not supported.</span></span>|
|<span data-ttu-id="fa266-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa266-113">Application</span></span>|<span data-ttu-id="fa266-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa266-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa266-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa266-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa266-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa266-116">Request headers</span></span>
|<span data-ttu-id="fa266-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fa266-117">Header</span></span>|<span data-ttu-id="fa266-118">Wert</span><span class="sxs-lookup"><span data-stu-id="fa266-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa266-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa266-119">Authorization</span></span>|<span data-ttu-id="fa266-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa266-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa266-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fa266-121">Accept</span></span>|<span data-ttu-id="fa266-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fa266-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa266-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa266-123">Request body</span></span>
<span data-ttu-id="fa266-124">Geben Sie im Anforderungstext eine JSON-Darstellung des windows10TeamGeneralConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="fa266-124">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="fa266-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10TeamGeneralConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fa266-125">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="fa266-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa266-126">Property</span></span>|<span data-ttu-id="fa266-127">Typ</span><span class="sxs-lookup"><span data-stu-id="fa266-127">Type</span></span>|<span data-ttu-id="fa266-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa266-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa266-129">id</span><span class="sxs-lookup"><span data-stu-id="fa266-129">id</span></span>|<span data-ttu-id="fa266-130">String</span><span class="sxs-lookup"><span data-stu-id="fa266-130">String</span></span>|<span data-ttu-id="fa266-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="fa266-131">Key of the entity.</span></span> <span data-ttu-id="fa266-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa266-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa266-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa266-133">lastModifiedDateTime</span></span>|<span data-ttu-id="fa266-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa266-134">DateTimeOffset</span></span>|<span data-ttu-id="fa266-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa266-135">DateTime the object was last modified.</span></span> <span data-ttu-id="fa266-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa266-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa266-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa266-137">createdDateTime</span></span>|<span data-ttu-id="fa266-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa266-138">DateTimeOffset</span></span>|<span data-ttu-id="fa266-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa266-139">DateTime the object was created.</span></span> <span data-ttu-id="fa266-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa266-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa266-141">description</span><span class="sxs-lookup"><span data-stu-id="fa266-141">description</span></span>|<span data-ttu-id="fa266-142">String</span><span class="sxs-lookup"><span data-stu-id="fa266-142">String</span></span>|<span data-ttu-id="fa266-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="fa266-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fa266-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa266-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa266-145">displayName</span><span class="sxs-lookup"><span data-stu-id="fa266-145">displayName</span></span>|<span data-ttu-id="fa266-146">String</span><span class="sxs-lookup"><span data-stu-id="fa266-146">String</span></span>|<span data-ttu-id="fa266-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="fa266-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fa266-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa266-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa266-149">version</span><span class="sxs-lookup"><span data-stu-id="fa266-149">version</span></span>|<span data-ttu-id="fa266-150">Int32</span><span class="sxs-lookup"><span data-stu-id="fa266-150">Int32</span></span>|<span data-ttu-id="fa266-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="fa266-151">Version of the device configuration.</span></span> <span data-ttu-id="fa266-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa266-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa266-153">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="fa266-153">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="fa266-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa266-154">Boolean</span></span>|<span data-ttu-id="fa266-155">Gibt an, ob Azure Operational Insights blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="fa266-155">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="fa266-156">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="fa266-156">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="fa266-157">String</span><span class="sxs-lookup"><span data-stu-id="fa266-157">String</span></span>|<span data-ttu-id="fa266-158">ID des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="fa266-158">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="fa266-159">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="fa266-159">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="fa266-160">String</span><span class="sxs-lookup"><span data-stu-id="fa266-160">String</span></span>|<span data-ttu-id="fa266-161">Schlüssel des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="fa266-161">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="fa266-162">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="fa266-162">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="fa266-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa266-163">Boolean</span></span>|<span data-ttu-id="fa266-164">Gibt an, ob die App „Verbinden“ automatisch gestartet werden soll, sobald eine Projektion initiiert wird.</span><span class="sxs-lookup"><span data-stu-id="fa266-164">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="fa266-165">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="fa266-165">maintenanceWindowBlocked</span></span>|<span data-ttu-id="fa266-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa266-166">Boolean</span></span>|<span data-ttu-id="fa266-167">Gibt an, ob ein Wartungsfenster für Geräteupdates festgelegt werden darf.</span><span class="sxs-lookup"><span data-stu-id="fa266-167">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="fa266-168">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="fa266-168">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="fa266-169">Int32</span><span class="sxs-lookup"><span data-stu-id="fa266-169">Int32</span></span>|<span data-ttu-id="fa266-170">Dauer des Wartungsfensters für Geräteupdates.</span><span class="sxs-lookup"><span data-stu-id="fa266-170">Maintenance window duration for device updates.</span></span> <span data-ttu-id="fa266-171">Gültige Werte: 0 bis 5.</span><span class="sxs-lookup"><span data-stu-id="fa266-171">Valid values 1 to 5</span></span>|
|<span data-ttu-id="fa266-172">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="fa266-172">maintenanceWindowStartTime</span></span>|<span data-ttu-id="fa266-173">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fa266-173">TimeOfDay</span></span>|<span data-ttu-id="fa266-174">Beginn des Wartungsfensters für Geräteupdates</span><span class="sxs-lookup"><span data-stu-id="fa266-174">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="fa266-175">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="fa266-175">miracastChannel</span></span>|<span data-ttu-id="fa266-176">String</span><span class="sxs-lookup"><span data-stu-id="fa266-176">String</span></span>|<span data-ttu-id="fa266-177">Kanal.</span><span class="sxs-lookup"><span data-stu-id="fa266-177">The channel.</span></span> <span data-ttu-id="fa266-178">Mögliche Werte sind: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne` und `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="fa266-178">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="fa266-179">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="fa266-179">miracastBlocked</span></span>|<span data-ttu-id="fa266-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa266-180">Boolean</span></span>|<span data-ttu-id="fa266-181">Gibt an, ob eine drahtlose Projektion erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="fa266-181">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="fa266-182">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="fa266-182">miracastRequirePin</span></span>|<span data-ttu-id="fa266-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa266-183">Boolean</span></span>|<span data-ttu-id="fa266-184">Gibt an, ob für eine drahtlose Projektion die Eingabe einer PIN erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="fa266-184">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="fa266-185">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="fa266-185">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="fa266-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa266-186">Boolean</span></span>|<span data-ttu-id="fa266-187">Gibt an, ob die Funktion „Meine Besprechungen und Dateien“ im Startmenü deaktiviert werden soll. In diesem Bereich werden die Office 365-Besprechungen und -Dateien des angemeldeten Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="fa266-187">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="fa266-188">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="fa266-188">settingsBlockSessionResume</span></span>|<span data-ttu-id="fa266-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa266-189">Boolean</span></span>|<span data-ttu-id="fa266-190">Gibt an, ob Sitzungen nach einem Sitzungstimeout fortgeführt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="fa266-190">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="fa266-191">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="fa266-191">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="fa266-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa266-192">Boolean</span></span>|<span data-ttu-id="fa266-193">Gibt an, ob das Anmeldedialogfeld automatisch mit den Eingeladenen aus geplanten Besprechungen befüllt werden darf.</span><span class="sxs-lookup"><span data-stu-id="fa266-193">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="fa266-194">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="fa266-194">settingsDefaultVolume</span></span>|<span data-ttu-id="fa266-195">Int32</span><span class="sxs-lookup"><span data-stu-id="fa266-195">Int32</span></span>|<span data-ttu-id="fa266-196">Legt die Standardlautstärke für neue Sitzungen fest.</span><span class="sxs-lookup"><span data-stu-id="fa266-196">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="fa266-197">Zulässige Werte sind 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="fa266-197">Permitted values are 0-100.</span></span> <span data-ttu-id="fa266-198">Der Standardwert lautet 45.</span><span class="sxs-lookup"><span data-stu-id="fa266-198">The default is 45.</span></span> <span data-ttu-id="fa266-199">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="fa266-199">Valid values 0 to 100</span></span>|
|<span data-ttu-id="fa266-200">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="fa266-200">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="fa266-201">Int32</span><span class="sxs-lookup"><span data-stu-id="fa266-201">Int32</span></span>|<span data-ttu-id="fa266-202">Gibt den Zeitraum in Minuten an, nach dem der Bildschirm des Hub-Systems abgeschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="fa266-202">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="fa266-203">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="fa266-203">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="fa266-204">Int32</span><span class="sxs-lookup"><span data-stu-id="fa266-204">Int32</span></span>|<span data-ttu-id="fa266-205">Gibt den Zeitraum in Minuten an, nach dem es zu einem Sitzungstimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="fa266-205">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="fa266-206">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="fa266-206">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="fa266-207">Int32</span><span class="sxs-lookup"><span data-stu-id="fa266-207">Int32</span></span>|<span data-ttu-id="fa266-208">Gibt den Zeitraum in Minuten an, nach dem das Hub-System in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="fa266-208">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="fa266-209">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="fa266-209">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="fa266-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa266-210">Boolean</span></span>|<span data-ttu-id="fa266-211">Gibt an, ob der Willkommensbildschirm automatisch angezeigt werden soll, sobald jemand den Raum betritt.</span><span class="sxs-lookup"><span data-stu-id="fa266-211">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="fa266-212">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="fa266-212">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="fa266-213">String</span><span class="sxs-lookup"><span data-stu-id="fa266-213">String</span></span>|<span data-ttu-id="fa266-214">URL zum Hintergrundbild für den Willkommensbildschirm.</span><span class="sxs-lookup"><span data-stu-id="fa266-214">The welcome screen background image URL.</span></span> <span data-ttu-id="fa266-215">Die URL muss das HTTPS-Protokoll verwenden und ein PNG-Bild zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="fa266-215">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="fa266-216">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="fa266-216">welcomeScreenMeetingInformation</span></span>|<span data-ttu-id="fa266-217">String</span><span class="sxs-lookup"><span data-stu-id="fa266-217">String</span></span>|<span data-ttu-id="fa266-218">Die Informationen, die im Willkommensbildschirm angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="fa266-218">The welcome screen meeting information shown.</span></span> <span data-ttu-id="fa266-219">Mögliche Werte sind: `userDefined`, `showOrganizerAndTimeOnly` und `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="fa266-219">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="fa266-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa266-220">Response</span></span>
<span data-ttu-id="fa266-221">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fa266-221">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa266-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa266-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa266-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa266-223">Request</span></span>
<span data-ttu-id="fa266-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa266-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1214

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="fa266-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa266-225">Response</span></span>
<span data-ttu-id="fa266-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa266-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



