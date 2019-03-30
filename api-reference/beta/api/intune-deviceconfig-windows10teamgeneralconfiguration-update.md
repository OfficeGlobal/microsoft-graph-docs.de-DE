---
title: Aktualisieren von „windows10TeamGeneralConfiguration“
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea49d65b395b8f3804f0cd9b42c33852832caa5f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988714"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="d4d2c-103">Aktualisieren von „windows10TeamGeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="d4d2c-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="d4d2c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4d2c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4d2c-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4d2c-106">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4d2c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d4d2c-107">Prerequisites</span></span>
<span data-ttu-id="d4d2c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4d2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4d2c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4d2c-110">Permission type</span></span>|<span data-ttu-id="d4d2c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4d2c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4d2c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4d2c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4d2c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4d2c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4d2c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4d2c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4d2c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4d2c-115">Not supported.</span></span>|
|<span data-ttu-id="d4d2c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4d2c-116">Application</span></span>|<span data-ttu-id="d4d2c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4d2c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4d2c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4d2c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d4d2c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4d2c-119">Request headers</span></span>
|<span data-ttu-id="d4d2c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d4d2c-120">Header</span></span>|<span data-ttu-id="d4d2c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d4d2c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4d2c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4d2c-122">Authorization</span></span>|<span data-ttu-id="d4d2c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4d2c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4d2c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d4d2c-124">Accept</span></span>|<span data-ttu-id="d4d2c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4d2c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4d2c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4d2c-126">Request body</span></span>
<span data-ttu-id="d4d2c-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-127">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="d4d2c-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-128">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="d4d2c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4d2c-129">Property</span></span>|<span data-ttu-id="d4d2c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d4d2c-130">Type</span></span>|<span data-ttu-id="d4d2c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4d2c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4d2c-132">id</span><span class="sxs-lookup"><span data-stu-id="d4d2c-132">id</span></span>|<span data-ttu-id="d4d2c-133">String</span><span class="sxs-lookup"><span data-stu-id="d4d2c-133">String</span></span>|<span data-ttu-id="d4d2c-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d4d2c-134">Key of the entity.</span></span> <span data-ttu-id="d4d2c-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4d2c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4d2c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4d2c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d4d2c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4d2c-137">DateTimeOffset</span></span>|<span data-ttu-id="d4d2c-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d4d2c-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4d2c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4d2c-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="d4d2c-140">roleScopeTagIds</span></span>|<span data-ttu-id="d4d2c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d4d2c-141">String collection</span></span>|<span data-ttu-id="d4d2c-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d4d2c-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4d2c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4d2c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d4d2c-144">supportsScopeTags</span></span>|<span data-ttu-id="d4d2c-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4d2c-145">Boolean</span></span>|<span data-ttu-id="d4d2c-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d4d2c-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d4d2c-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d4d2c-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-149">This property is read-only.</span></span> <span data-ttu-id="d4d2c-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4d2c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4d2c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4d2c-151">createdDateTime</span></span>|<span data-ttu-id="d4d2c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4d2c-152">DateTimeOffset</span></span>|<span data-ttu-id="d4d2c-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-153">DateTime the object was created.</span></span> <span data-ttu-id="d4d2c-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4d2c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4d2c-155">description</span><span class="sxs-lookup"><span data-stu-id="d4d2c-155">description</span></span>|<span data-ttu-id="d4d2c-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4d2c-156">String</span></span>|<span data-ttu-id="d4d2c-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d4d2c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d4d2c-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4d2c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4d2c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d4d2c-159">displayName</span></span>|<span data-ttu-id="d4d2c-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4d2c-160">String</span></span>|<span data-ttu-id="d4d2c-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d4d2c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d4d2c-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4d2c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4d2c-163">Version</span><span class="sxs-lookup"><span data-stu-id="d4d2c-163">version</span></span>|<span data-ttu-id="d4d2c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d4d2c-164">Int32</span></span>|<span data-ttu-id="d4d2c-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-165">Version of the device configuration.</span></span> <span data-ttu-id="d4d2c-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4d2c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4d2c-167">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="d4d2c-167">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="d4d2c-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4d2c-168">Boolean</span></span>|<span data-ttu-id="d4d2c-169">Gibt an, ob Azure Operational Insights blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-169">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="d4d2c-170">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="d4d2c-170">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="d4d2c-171">String</span><span class="sxs-lookup"><span data-stu-id="d4d2c-171">String</span></span>|<span data-ttu-id="d4d2c-172">ID des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="d4d2c-172">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="d4d2c-173">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="d4d2c-173">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="d4d2c-174">String</span><span class="sxs-lookup"><span data-stu-id="d4d2c-174">String</span></span>|<span data-ttu-id="d4d2c-175">Schlüssel des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="d4d2c-175">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="d4d2c-176">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="d4d2c-176">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="d4d2c-177">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4d2c-177">Boolean</span></span>|<span data-ttu-id="d4d2c-178">Gibt an, ob die App „Verbinden“ automatisch gestartet werden soll, sobald eine Projektion initiiert wird.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-178">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="d4d2c-179">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="d4d2c-179">maintenanceWindowBlocked</span></span>|<span data-ttu-id="d4d2c-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4d2c-180">Boolean</span></span>|<span data-ttu-id="d4d2c-181">Gibt an, ob ein Wartungsfenster für Geräteupdates festgelegt werden darf.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-181">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="d4d2c-182">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="d4d2c-182">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="d4d2c-183">Int32</span><span class="sxs-lookup"><span data-stu-id="d4d2c-183">Int32</span></span>|<span data-ttu-id="d4d2c-184">Dauer des Wartungsfensters für Geräteupdates.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-184">Maintenance window duration for device updates.</span></span> <span data-ttu-id="d4d2c-185">Gültige Werte: 0 bis 5.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-185">Valid values 0 to 5</span></span>|
|<span data-ttu-id="d4d2c-186">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="d4d2c-186">maintenanceWindowStartTime</span></span>|<span data-ttu-id="d4d2c-187">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d4d2c-187">TimeOfDay</span></span>|<span data-ttu-id="d4d2c-188">Beginn des Wartungsfensters für Geräteupdates</span><span class="sxs-lookup"><span data-stu-id="d4d2c-188">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="d4d2c-189">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="d4d2c-189">miracastChannel</span></span>|[<span data-ttu-id="d4d2c-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="d4d2c-190">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="d4d2c-191">Kanal.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-191">The channel.</span></span> <span data-ttu-id="d4d2c-192">Mögliche Werte sind: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne` und `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-192">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="d4d2c-193">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="d4d2c-193">miracastBlocked</span></span>|<span data-ttu-id="d4d2c-194">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4d2c-194">Boolean</span></span>|<span data-ttu-id="d4d2c-195">Gibt an, ob eine drahtlose Projektion erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-195">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="d4d2c-196">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="d4d2c-196">miracastRequirePin</span></span>|<span data-ttu-id="d4d2c-197">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4d2c-197">Boolean</span></span>|<span data-ttu-id="d4d2c-198">Gibt an, ob für eine drahtlose Projektion die Eingabe einer PIN erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-198">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="d4d2c-199">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="d4d2c-199">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="d4d2c-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4d2c-200">Boolean</span></span>|<span data-ttu-id="d4d2c-201">Gibt an, ob die Funktion „Meine Besprechungen und Dateien“ im Startmenü deaktiviert werden soll. In diesem Bereich werden die Office 365-Besprechungen und -Dateien des angemeldeten Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-201">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="d4d2c-202">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="d4d2c-202">settingsBlockSessionResume</span></span>|<span data-ttu-id="d4d2c-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4d2c-203">Boolean</span></span>|<span data-ttu-id="d4d2c-204">Gibt an, ob Sitzungen nach einem Sitzungstimeout fortgeführt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-204">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="d4d2c-205">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="d4d2c-205">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="d4d2c-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4d2c-206">Boolean</span></span>|<span data-ttu-id="d4d2c-207">Gibt an, ob das Anmeldedialogfeld automatisch mit den Eingeladenen aus geplanten Besprechungen befüllt werden darf.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-207">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="d4d2c-208">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="d4d2c-208">settingsDefaultVolume</span></span>|<span data-ttu-id="d4d2c-209">Int32</span><span class="sxs-lookup"><span data-stu-id="d4d2c-209">Int32</span></span>|<span data-ttu-id="d4d2c-210">Legt die Standardlautstärke für neue Sitzungen fest.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-210">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="d4d2c-211">Zulässige Werte sind 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-211">Permitted values are 0-100.</span></span> <span data-ttu-id="d4d2c-212">Der Standardwert lautet 45.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-212">The default is 45.</span></span> <span data-ttu-id="d4d2c-213">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-213">Valid values 0 to 100</span></span>|
|<span data-ttu-id="d4d2c-214">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d4d2c-214">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="d4d2c-215">Int32</span><span class="sxs-lookup"><span data-stu-id="d4d2c-215">Int32</span></span>|<span data-ttu-id="d4d2c-216">Gibt den Zeitraum in Minuten an, nach dem der Bildschirm des Hub-Systems abgeschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-216">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="d4d2c-217">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d4d2c-217">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="d4d2c-218">Int32</span><span class="sxs-lookup"><span data-stu-id="d4d2c-218">Int32</span></span>|<span data-ttu-id="d4d2c-219">Gibt den Zeitraum in Minuten an, nach dem es zu einem Sitzungstimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-219">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="d4d2c-220">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d4d2c-220">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="d4d2c-221">Int32</span><span class="sxs-lookup"><span data-stu-id="d4d2c-221">Int32</span></span>|<span data-ttu-id="d4d2c-222">Gibt den Zeitraum in Minuten an, nach dem das Hub-System in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-222">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="d4d2c-223">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="d4d2c-223">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="d4d2c-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4d2c-224">Boolean</span></span>|<span data-ttu-id="d4d2c-225">Gibt an, ob der Willkommensbildschirm automatisch angezeigt werden soll, sobald jemand den Raum betritt.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-225">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="d4d2c-226">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="d4d2c-226">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="d4d2c-227">String</span><span class="sxs-lookup"><span data-stu-id="d4d2c-227">String</span></span>|<span data-ttu-id="d4d2c-228">URL zum Hintergrundbild für den Willkommensbildschirm.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-228">The welcome screen background image URL.</span></span> <span data-ttu-id="d4d2c-229">Die URL muss das HTTPS-Protokoll verwenden und ein PNG-Bild zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-229">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="d4d2c-230">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="d4d2c-230">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="d4d2c-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="d4d2c-231">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="d4d2c-232">Die Informationen, die im Willkommensbildschirm angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-232">The welcome screen meeting information shown.</span></span> <span data-ttu-id="d4d2c-233">Mögliche Werte sind: `userDefined`, `showOrganizerAndTimeOnly` und `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-233">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="d4d2c-234">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4d2c-234">Response</span></span>
<span data-ttu-id="d4d2c-235">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-235">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4d2c-236">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4d2c-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4d2c-237">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4d2c-237">Request</span></span>
<span data-ttu-id="d4d2c-238">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1242

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="d4d2c-239">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4d2c-239">Response</span></span>
<span data-ttu-id="d4d2c-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4d2c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1414

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




