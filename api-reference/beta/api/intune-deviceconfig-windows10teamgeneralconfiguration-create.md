---
title: windows10TeamGeneralConfiguration erstellen
description: Erstellt neue Objekte des Typs windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3ae4ff125219d470b4ae8bc8462f6b234adb0714
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985998"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="0ceba-103">windows10TeamGeneralConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="0ceba-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="0ceba-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0ceba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ceba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ceba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ceba-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0ceba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ceba-107">Erstellt neue Objekte des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ceba-107">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ceba-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0ceba-108">Prerequisites</span></span>
<span data-ttu-id="0ceba-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ceba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ceba-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0ceba-111">Permission type</span></span>|<span data-ttu-id="0ceba-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0ceba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ceba-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0ceba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ceba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ceba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ceba-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0ceba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ceba-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ceba-116">Not supported.</span></span>|
|<span data-ttu-id="0ceba-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0ceba-117">Application</span></span>|<span data-ttu-id="0ceba-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ceba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ceba-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ceba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0ceba-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ceba-120">Request headers</span></span>
|<span data-ttu-id="0ceba-121">Header</span><span class="sxs-lookup"><span data-stu-id="0ceba-121">Header</span></span>|<span data-ttu-id="0ceba-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0ceba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ceba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ceba-123">Authorization</span></span>|<span data-ttu-id="0ceba-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0ceba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ceba-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0ceba-125">Accept</span></span>|<span data-ttu-id="0ceba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ceba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ceba-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0ceba-127">Request body</span></span>
<span data-ttu-id="0ceba-128">Geben Sie im Anforderungstext eine JSON-Darstellung des windows10TeamGeneralConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0ceba-128">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="0ceba-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10TeamGeneralConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0ceba-129">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="0ceba-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0ceba-130">Property</span></span>|<span data-ttu-id="0ceba-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0ceba-131">Type</span></span>|<span data-ttu-id="0ceba-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ceba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ceba-133">id</span><span class="sxs-lookup"><span data-stu-id="0ceba-133">id</span></span>|<span data-ttu-id="0ceba-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ceba-134">String</span></span>|<span data-ttu-id="0ceba-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0ceba-135">Key of the entity.</span></span> <span data-ttu-id="0ceba-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ceba-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceba-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ceba-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0ceba-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ceba-138">DateTimeOffset</span></span>|<span data-ttu-id="0ceba-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0ceba-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0ceba-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ceba-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceba-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ceba-141">roleScopeTagIds</span></span>|<span data-ttu-id="0ceba-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="0ceba-142">String collection</span></span>|<span data-ttu-id="0ceba-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="0ceba-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ceba-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ceba-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceba-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0ceba-145">supportsScopeTags</span></span>|<span data-ttu-id="0ceba-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0ceba-146">Boolean</span></span>|<span data-ttu-id="0ceba-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ceba-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0ceba-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="0ceba-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0ceba-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="0ceba-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0ceba-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0ceba-150">This property is read-only.</span></span> <span data-ttu-id="0ceba-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ceba-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceba-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ceba-152">createdDateTime</span></span>|<span data-ttu-id="0ceba-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ceba-153">DateTimeOffset</span></span>|<span data-ttu-id="0ceba-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0ceba-154">DateTime the object was created.</span></span> <span data-ttu-id="0ceba-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ceba-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceba-156">description</span><span class="sxs-lookup"><span data-stu-id="0ceba-156">description</span></span>|<span data-ttu-id="0ceba-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ceba-157">String</span></span>|<span data-ttu-id="0ceba-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0ceba-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ceba-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ceba-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceba-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0ceba-160">displayName</span></span>|<span data-ttu-id="0ceba-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ceba-161">String</span></span>|<span data-ttu-id="0ceba-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0ceba-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ceba-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ceba-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceba-164">Version</span><span class="sxs-lookup"><span data-stu-id="0ceba-164">version</span></span>|<span data-ttu-id="0ceba-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0ceba-165">Int32</span></span>|<span data-ttu-id="0ceba-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0ceba-166">Version of the device configuration.</span></span> <span data-ttu-id="0ceba-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ceba-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ceba-168">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="0ceba-168">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="0ceba-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceba-169">Boolean</span></span>|<span data-ttu-id="0ceba-170">Gibt an, ob Azure Operational Insights blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="0ceba-170">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="0ceba-171">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="0ceba-171">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="0ceba-172">String</span><span class="sxs-lookup"><span data-stu-id="0ceba-172">String</span></span>|<span data-ttu-id="0ceba-173">ID des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="0ceba-173">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="0ceba-174">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="0ceba-174">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="0ceba-175">String</span><span class="sxs-lookup"><span data-stu-id="0ceba-175">String</span></span>|<span data-ttu-id="0ceba-176">Schlüssel des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="0ceba-176">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="0ceba-177">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="0ceba-177">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="0ceba-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceba-178">Boolean</span></span>|<span data-ttu-id="0ceba-179">Gibt an, ob die App „Verbinden“ automatisch gestartet werden soll, sobald eine Projektion initiiert wird.</span><span class="sxs-lookup"><span data-stu-id="0ceba-179">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="0ceba-180">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="0ceba-180">maintenanceWindowBlocked</span></span>|<span data-ttu-id="0ceba-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceba-181">Boolean</span></span>|<span data-ttu-id="0ceba-182">Gibt an, ob ein Wartungsfenster für Geräteupdates festgelegt werden darf.</span><span class="sxs-lookup"><span data-stu-id="0ceba-182">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="0ceba-183">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="0ceba-183">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="0ceba-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0ceba-184">Int32</span></span>|<span data-ttu-id="0ceba-185">Dauer des Wartungsfensters für Geräteupdates.</span><span class="sxs-lookup"><span data-stu-id="0ceba-185">Maintenance window duration for device updates.</span></span> <span data-ttu-id="0ceba-186">Gültige Werte: 0 bis 5.</span><span class="sxs-lookup"><span data-stu-id="0ceba-186">Valid values 0 to 5</span></span>|
|<span data-ttu-id="0ceba-187">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="0ceba-187">maintenanceWindowStartTime</span></span>|<span data-ttu-id="0ceba-188">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0ceba-188">TimeOfDay</span></span>|<span data-ttu-id="0ceba-189">Beginn des Wartungsfensters für Geräteupdates</span><span class="sxs-lookup"><span data-stu-id="0ceba-189">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="0ceba-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="0ceba-190">miracastChannel</span></span>|[<span data-ttu-id="0ceba-191">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="0ceba-191">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="0ceba-192">Kanal.</span><span class="sxs-lookup"><span data-stu-id="0ceba-192">The channel.</span></span> <span data-ttu-id="0ceba-193">Mögliche Werte sind: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne` und `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="0ceba-193">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="0ceba-194">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="0ceba-194">miracastBlocked</span></span>|<span data-ttu-id="0ceba-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceba-195">Boolean</span></span>|<span data-ttu-id="0ceba-196">Gibt an, ob eine drahtlose Projektion erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="0ceba-196">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="0ceba-197">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="0ceba-197">miracastRequirePin</span></span>|<span data-ttu-id="0ceba-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceba-198">Boolean</span></span>|<span data-ttu-id="0ceba-199">Gibt an, ob für eine drahtlose Projektion die Eingabe einer PIN erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="0ceba-199">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="0ceba-200">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="0ceba-200">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="0ceba-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceba-201">Boolean</span></span>|<span data-ttu-id="0ceba-202">Gibt an, ob die Funktion „Meine Besprechungen und Dateien“ im Startmenü deaktiviert werden soll. In diesem Bereich werden die Office 365-Besprechungen und -Dateien des angemeldeten Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0ceba-202">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="0ceba-203">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="0ceba-203">settingsBlockSessionResume</span></span>|<span data-ttu-id="0ceba-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceba-204">Boolean</span></span>|<span data-ttu-id="0ceba-205">Gibt an, ob Sitzungen nach einem Sitzungstimeout fortgeführt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="0ceba-205">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="0ceba-206">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="0ceba-206">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="0ceba-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceba-207">Boolean</span></span>|<span data-ttu-id="0ceba-208">Gibt an, ob das Anmeldedialogfeld automatisch mit den Eingeladenen aus geplanten Besprechungen befüllt werden darf.</span><span class="sxs-lookup"><span data-stu-id="0ceba-208">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="0ceba-209">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="0ceba-209">settingsDefaultVolume</span></span>|<span data-ttu-id="0ceba-210">Int32</span><span class="sxs-lookup"><span data-stu-id="0ceba-210">Int32</span></span>|<span data-ttu-id="0ceba-211">Legt die Standardlautstärke für neue Sitzungen fest.</span><span class="sxs-lookup"><span data-stu-id="0ceba-211">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="0ceba-212">Zulässige Werte sind 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="0ceba-212">Permitted values are 0-100.</span></span> <span data-ttu-id="0ceba-213">Der Standardwert lautet 45.</span><span class="sxs-lookup"><span data-stu-id="0ceba-213">The default is 45.</span></span> <span data-ttu-id="0ceba-214">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="0ceba-214">Valid values 0 to 100</span></span>|
|<span data-ttu-id="0ceba-215">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="0ceba-215">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="0ceba-216">Int32</span><span class="sxs-lookup"><span data-stu-id="0ceba-216">Int32</span></span>|<span data-ttu-id="0ceba-217">Gibt den Zeitraum in Minuten an, nach dem der Bildschirm des Hub-Systems abgeschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="0ceba-217">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="0ceba-218">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="0ceba-218">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="0ceba-219">Int32</span><span class="sxs-lookup"><span data-stu-id="0ceba-219">Int32</span></span>|<span data-ttu-id="0ceba-220">Gibt den Zeitraum in Minuten an, nach dem es zu einem Sitzungstimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="0ceba-220">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="0ceba-221">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="0ceba-221">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="0ceba-222">Int32</span><span class="sxs-lookup"><span data-stu-id="0ceba-222">Int32</span></span>|<span data-ttu-id="0ceba-223">Gibt den Zeitraum in Minuten an, nach dem das Hub-System in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="0ceba-223">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="0ceba-224">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="0ceba-224">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="0ceba-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ceba-225">Boolean</span></span>|<span data-ttu-id="0ceba-226">Gibt an, ob der Willkommensbildschirm automatisch angezeigt werden soll, sobald jemand den Raum betritt.</span><span class="sxs-lookup"><span data-stu-id="0ceba-226">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="0ceba-227">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="0ceba-227">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="0ceba-228">String</span><span class="sxs-lookup"><span data-stu-id="0ceba-228">String</span></span>|<span data-ttu-id="0ceba-229">URL zum Hintergrundbild für den Willkommensbildschirm.</span><span class="sxs-lookup"><span data-stu-id="0ceba-229">The welcome screen background image URL.</span></span> <span data-ttu-id="0ceba-230">Die URL muss das HTTPS-Protokoll verwenden und ein PNG-Bild zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="0ceba-230">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="0ceba-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="0ceba-231">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="0ceba-232">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="0ceba-232">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="0ceba-233">Die Informationen, die im Willkommensbildschirm angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0ceba-233">The welcome screen meeting information shown.</span></span> <span data-ttu-id="0ceba-234">Mögliche Werte sind: `userDefined`, `showOrganizerAndTimeOnly` und `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="0ceba-234">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="0ceba-235">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ceba-235">Response</span></span>
<span data-ttu-id="0ceba-236">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0ceba-236">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ceba-237">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ceba-237">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ceba-238">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ceba-238">Request</span></span>
<span data-ttu-id="0ceba-239">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0ceba-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1306

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="0ceba-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ceba-240">Response</span></span>
<span data-ttu-id="0ceba-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ceba-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





