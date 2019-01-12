---
title: Aktualisieren von „windows10TeamGeneralConfiguration“
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1a0a9b98c889633c576c5538e868e319e4c3ea71
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941975"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="0121d-103">Aktualisieren von „windows10TeamGeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="0121d-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="0121d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0121d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0121d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0121d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0121d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0121d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0121d-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0121d-107">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0121d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0121d-108">Prerequisites</span></span>
<span data-ttu-id="0121d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0121d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0121d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0121d-111">Permission type</span></span>|<span data-ttu-id="0121d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0121d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0121d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0121d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0121d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0121d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0121d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0121d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0121d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0121d-116">Not supported.</span></span>|
|<span data-ttu-id="0121d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0121d-117">Application</span></span>|<span data-ttu-id="0121d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0121d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0121d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0121d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0121d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0121d-120">Request headers</span></span>
|<span data-ttu-id="0121d-121">Header</span><span class="sxs-lookup"><span data-stu-id="0121d-121">Header</span></span>|<span data-ttu-id="0121d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0121d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0121d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0121d-123">Authorization</span></span>|<span data-ttu-id="0121d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0121d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0121d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0121d-125">Accept</span></span>|<span data-ttu-id="0121d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0121d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0121d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0121d-127">Request body</span></span>
<span data-ttu-id="0121d-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="0121d-128">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="0121d-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="0121d-129">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="0121d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0121d-130">Property</span></span>|<span data-ttu-id="0121d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0121d-131">Type</span></span>|<span data-ttu-id="0121d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0121d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0121d-133">id</span><span class="sxs-lookup"><span data-stu-id="0121d-133">id</span></span>|<span data-ttu-id="0121d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0121d-134">String</span></span>|<span data-ttu-id="0121d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0121d-135">Key of the entity.</span></span> <span data-ttu-id="0121d-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0121d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0121d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0121d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0121d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0121d-138">DateTimeOffset</span></span>|<span data-ttu-id="0121d-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0121d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0121d-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0121d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0121d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0121d-141">roleScopeTagIds</span></span>|<span data-ttu-id="0121d-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="0121d-142">String collection</span></span>|<span data-ttu-id="0121d-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="0121d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0121d-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0121d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0121d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0121d-145">supportsScopeTags</span></span>|<span data-ttu-id="0121d-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0121d-146">Boolean</span></span>|<span data-ttu-id="0121d-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0121d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0121d-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="0121d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0121d-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="0121d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0121d-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0121d-150">This property is read-only.</span></span> <span data-ttu-id="0121d-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0121d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0121d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0121d-152">createdDateTime</span></span>|<span data-ttu-id="0121d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0121d-153">DateTimeOffset</span></span>|<span data-ttu-id="0121d-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0121d-154">DateTime the object was created.</span></span> <span data-ttu-id="0121d-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0121d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0121d-156">description</span><span class="sxs-lookup"><span data-stu-id="0121d-156">description</span></span>|<span data-ttu-id="0121d-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0121d-157">String</span></span>|<span data-ttu-id="0121d-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0121d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0121d-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0121d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0121d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0121d-160">displayName</span></span>|<span data-ttu-id="0121d-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0121d-161">String</span></span>|<span data-ttu-id="0121d-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0121d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0121d-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0121d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0121d-164">Version</span><span class="sxs-lookup"><span data-stu-id="0121d-164">version</span></span>|<span data-ttu-id="0121d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0121d-165">Int32</span></span>|<span data-ttu-id="0121d-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0121d-166">Version of the device configuration.</span></span> <span data-ttu-id="0121d-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0121d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0121d-168">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="0121d-168">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="0121d-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="0121d-169">Boolean</span></span>|<span data-ttu-id="0121d-170">Gibt an, ob Azure Operational Insights blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="0121d-170">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="0121d-171">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="0121d-171">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="0121d-172">String</span><span class="sxs-lookup"><span data-stu-id="0121d-172">String</span></span>|<span data-ttu-id="0121d-173">ID des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="0121d-173">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="0121d-174">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="0121d-174">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="0121d-175">String</span><span class="sxs-lookup"><span data-stu-id="0121d-175">String</span></span>|<span data-ttu-id="0121d-176">Schlüssel des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="0121d-176">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="0121d-177">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="0121d-177">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="0121d-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="0121d-178">Boolean</span></span>|<span data-ttu-id="0121d-179">Gibt an, ob die App „Verbinden“ automatisch gestartet werden soll, sobald eine Projektion initiiert wird.</span><span class="sxs-lookup"><span data-stu-id="0121d-179">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="0121d-180">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="0121d-180">maintenanceWindowBlocked</span></span>|<span data-ttu-id="0121d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="0121d-181">Boolean</span></span>|<span data-ttu-id="0121d-182">Gibt an, ob ein Wartungsfenster für Geräteupdates festgelegt werden darf.</span><span class="sxs-lookup"><span data-stu-id="0121d-182">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="0121d-183">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="0121d-183">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="0121d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0121d-184">Int32</span></span>|<span data-ttu-id="0121d-185">Dauer des Wartungsfensters für Geräteupdates.</span><span class="sxs-lookup"><span data-stu-id="0121d-185">Maintenance window duration for device updates.</span></span> <span data-ttu-id="0121d-186">Gültige Werte: 0 bis 5.</span><span class="sxs-lookup"><span data-stu-id="0121d-186">Valid values 0 to 5</span></span>|
|<span data-ttu-id="0121d-187">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="0121d-187">maintenanceWindowStartTime</span></span>|<span data-ttu-id="0121d-188">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0121d-188">TimeOfDay</span></span>|<span data-ttu-id="0121d-189">Beginn des Wartungsfensters für Geräteupdates</span><span class="sxs-lookup"><span data-stu-id="0121d-189">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="0121d-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="0121d-190">miracastChannel</span></span>|[<span data-ttu-id="0121d-191">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="0121d-191">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="0121d-192">Kanal.</span><span class="sxs-lookup"><span data-stu-id="0121d-192">The channel.</span></span> <span data-ttu-id="0121d-193">Mögliche Werte sind: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne` und `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="0121d-193">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="0121d-194">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="0121d-194">miracastBlocked</span></span>|<span data-ttu-id="0121d-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="0121d-195">Boolean</span></span>|<span data-ttu-id="0121d-196">Gibt an, ob eine drahtlose Projektion erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="0121d-196">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="0121d-197">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="0121d-197">miracastRequirePin</span></span>|<span data-ttu-id="0121d-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="0121d-198">Boolean</span></span>|<span data-ttu-id="0121d-199">Gibt an, ob für eine drahtlose Projektion die Eingabe einer PIN erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="0121d-199">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="0121d-200">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="0121d-200">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="0121d-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="0121d-201">Boolean</span></span>|<span data-ttu-id="0121d-202">Gibt an, ob die Funktion „Meine Besprechungen und Dateien“ im Startmenü deaktiviert werden soll. In diesem Bereich werden die Office 365-Besprechungen und -Dateien des angemeldeten Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0121d-202">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="0121d-203">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="0121d-203">settingsBlockSessionResume</span></span>|<span data-ttu-id="0121d-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="0121d-204">Boolean</span></span>|<span data-ttu-id="0121d-205">Gibt an, ob Sitzungen nach einem Sitzungstimeout fortgeführt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="0121d-205">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="0121d-206">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="0121d-206">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="0121d-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="0121d-207">Boolean</span></span>|<span data-ttu-id="0121d-208">Gibt an, ob das Anmeldedialogfeld automatisch mit den Eingeladenen aus geplanten Besprechungen befüllt werden darf.</span><span class="sxs-lookup"><span data-stu-id="0121d-208">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="0121d-209">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="0121d-209">settingsDefaultVolume</span></span>|<span data-ttu-id="0121d-210">Int32</span><span class="sxs-lookup"><span data-stu-id="0121d-210">Int32</span></span>|<span data-ttu-id="0121d-211">Legt die Standardlautstärke für neue Sitzungen fest.</span><span class="sxs-lookup"><span data-stu-id="0121d-211">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="0121d-212">Zulässige Werte sind 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="0121d-212">Permitted values are 0-100.</span></span> <span data-ttu-id="0121d-213">Der Standardwert lautet 45.</span><span class="sxs-lookup"><span data-stu-id="0121d-213">The default is 45.</span></span> <span data-ttu-id="0121d-214">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="0121d-214">Valid values 0 to 100</span></span>|
|<span data-ttu-id="0121d-215">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="0121d-215">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="0121d-216">Int32</span><span class="sxs-lookup"><span data-stu-id="0121d-216">Int32</span></span>|<span data-ttu-id="0121d-217">Gibt den Zeitraum in Minuten an, nach dem der Bildschirm des Hub-Systems abgeschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="0121d-217">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="0121d-218">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="0121d-218">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="0121d-219">Int32</span><span class="sxs-lookup"><span data-stu-id="0121d-219">Int32</span></span>|<span data-ttu-id="0121d-220">Gibt den Zeitraum in Minuten an, nach dem es zu einem Sitzungstimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="0121d-220">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="0121d-221">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="0121d-221">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="0121d-222">Int32</span><span class="sxs-lookup"><span data-stu-id="0121d-222">Int32</span></span>|<span data-ttu-id="0121d-223">Gibt den Zeitraum in Minuten an, nach dem das Hub-System in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="0121d-223">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="0121d-224">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="0121d-224">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="0121d-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="0121d-225">Boolean</span></span>|<span data-ttu-id="0121d-226">Gibt an, ob der Willkommensbildschirm automatisch angezeigt werden soll, sobald jemand den Raum betritt.</span><span class="sxs-lookup"><span data-stu-id="0121d-226">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="0121d-227">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="0121d-227">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="0121d-228">String</span><span class="sxs-lookup"><span data-stu-id="0121d-228">String</span></span>|<span data-ttu-id="0121d-229">URL zum Hintergrundbild für den Willkommensbildschirm.</span><span class="sxs-lookup"><span data-stu-id="0121d-229">The welcome screen background image URL.</span></span> <span data-ttu-id="0121d-230">Die URL muss das HTTPS-Protokoll verwenden und ein PNG-Bild zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="0121d-230">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="0121d-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="0121d-231">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="0121d-232">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="0121d-232">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="0121d-233">Die Informationen, die im Willkommensbildschirm angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0121d-233">The welcome screen meeting information shown.</span></span> <span data-ttu-id="0121d-234">Mögliche Werte sind: `userDefined`, `showOrganizerAndTimeOnly` und `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="0121d-234">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="0121d-235">Antwort</span><span class="sxs-lookup"><span data-stu-id="0121d-235">Response</span></span>
<span data-ttu-id="0121d-236">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0121d-236">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0121d-237">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0121d-237">Example</span></span>
### <a name="request"></a><span data-ttu-id="0121d-238">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0121d-238">Request</span></span>
<span data-ttu-id="0121d-239">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0121d-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1234

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="0121d-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="0121d-240">Response</span></span>
<span data-ttu-id="0121d-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0121d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





