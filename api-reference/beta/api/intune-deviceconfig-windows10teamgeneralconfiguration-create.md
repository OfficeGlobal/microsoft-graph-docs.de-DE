---
title: windows10TeamGeneralConfiguration erstellen
description: Erstellt neue Objekte des Typs windows10TeamGeneralConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7b45845608a486dffea655faf6d4d06a0b51e463
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411302"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="10bd7-103">windows10TeamGeneralConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="10bd7-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="10bd7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="10bd7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="10bd7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10bd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10bd7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10bd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10bd7-107">Erstellt neue Objekte des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10bd7-107">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10bd7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="10bd7-108">Prerequisites</span></span>
<span data-ttu-id="10bd7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="10bd7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="10bd7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10bd7-111">Permission type</span></span>|<span data-ttu-id="10bd7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10bd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10bd7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10bd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10bd7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10bd7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10bd7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10bd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10bd7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10bd7-116">Not supported.</span></span>|
|<span data-ttu-id="10bd7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10bd7-117">Application</span></span>|<span data-ttu-id="10bd7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10bd7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10bd7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10bd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="10bd7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10bd7-120">Request headers</span></span>
|<span data-ttu-id="10bd7-121">Header</span><span class="sxs-lookup"><span data-stu-id="10bd7-121">Header</span></span>|<span data-ttu-id="10bd7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="10bd7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10bd7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="10bd7-123">Authorization</span></span>|<span data-ttu-id="10bd7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="10bd7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10bd7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="10bd7-125">Accept</span></span>|<span data-ttu-id="10bd7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10bd7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10bd7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10bd7-127">Request body</span></span>
<span data-ttu-id="10bd7-128">Geben Sie im Anforderungstext eine JSON-Darstellung des windows10TeamGeneralConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="10bd7-128">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="10bd7-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10TeamGeneralConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="10bd7-129">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="10bd7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10bd7-130">Property</span></span>|<span data-ttu-id="10bd7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="10bd7-131">Type</span></span>|<span data-ttu-id="10bd7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10bd7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10bd7-133">id</span><span class="sxs-lookup"><span data-stu-id="10bd7-133">id</span></span>|<span data-ttu-id="10bd7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10bd7-134">String</span></span>|<span data-ttu-id="10bd7-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="10bd7-135">Key of the entity.</span></span> <span data-ttu-id="10bd7-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10bd7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10bd7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10bd7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="10bd7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10bd7-138">DateTimeOffset</span></span>|<span data-ttu-id="10bd7-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="10bd7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="10bd7-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10bd7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10bd7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="10bd7-141">roleScopeTagIds</span></span>|<span data-ttu-id="10bd7-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="10bd7-142">String collection</span></span>|<span data-ttu-id="10bd7-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="10bd7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="10bd7-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10bd7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10bd7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="10bd7-145">supportsScopeTags</span></span>|<span data-ttu-id="10bd7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="10bd7-146">Boolean</span></span>|<span data-ttu-id="10bd7-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10bd7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="10bd7-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="10bd7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="10bd7-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="10bd7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="10bd7-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10bd7-150">This property is read-only.</span></span> <span data-ttu-id="10bd7-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10bd7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10bd7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10bd7-152">createdDateTime</span></span>|<span data-ttu-id="10bd7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10bd7-153">DateTimeOffset</span></span>|<span data-ttu-id="10bd7-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="10bd7-154">DateTime the object was created.</span></span> <span data-ttu-id="10bd7-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10bd7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10bd7-156">description</span><span class="sxs-lookup"><span data-stu-id="10bd7-156">description</span></span>|<span data-ttu-id="10bd7-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10bd7-157">String</span></span>|<span data-ttu-id="10bd7-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="10bd7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="10bd7-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10bd7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10bd7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="10bd7-160">displayName</span></span>|<span data-ttu-id="10bd7-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10bd7-161">String</span></span>|<span data-ttu-id="10bd7-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="10bd7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="10bd7-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10bd7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10bd7-164">Version</span><span class="sxs-lookup"><span data-stu-id="10bd7-164">version</span></span>|<span data-ttu-id="10bd7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="10bd7-165">Int32</span></span>|<span data-ttu-id="10bd7-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="10bd7-166">Version of the device configuration.</span></span> <span data-ttu-id="10bd7-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10bd7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10bd7-168">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="10bd7-168">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="10bd7-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="10bd7-169">Boolean</span></span>|<span data-ttu-id="10bd7-170">Gibt an, ob Azure Operational Insights blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="10bd7-170">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="10bd7-171">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="10bd7-171">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="10bd7-172">String</span><span class="sxs-lookup"><span data-stu-id="10bd7-172">String</span></span>|<span data-ttu-id="10bd7-173">ID des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="10bd7-173">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="10bd7-174">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="10bd7-174">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="10bd7-175">String</span><span class="sxs-lookup"><span data-stu-id="10bd7-175">String</span></span>|<span data-ttu-id="10bd7-176">Schlüssel des Azure Operational Insights-Arbeitsbereichs</span><span class="sxs-lookup"><span data-stu-id="10bd7-176">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="10bd7-177">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="10bd7-177">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="10bd7-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="10bd7-178">Boolean</span></span>|<span data-ttu-id="10bd7-179">Gibt an, ob die App „Verbinden“ automatisch gestartet werden soll, sobald eine Projektion initiiert wird.</span><span class="sxs-lookup"><span data-stu-id="10bd7-179">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="10bd7-180">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="10bd7-180">maintenanceWindowBlocked</span></span>|<span data-ttu-id="10bd7-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="10bd7-181">Boolean</span></span>|<span data-ttu-id="10bd7-182">Gibt an, ob ein Wartungsfenster für Geräteupdates festgelegt werden darf.</span><span class="sxs-lookup"><span data-stu-id="10bd7-182">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="10bd7-183">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="10bd7-183">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="10bd7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="10bd7-184">Int32</span></span>|<span data-ttu-id="10bd7-185">Dauer des Wartungsfensters für Geräteupdates.</span><span class="sxs-lookup"><span data-stu-id="10bd7-185">Maintenance window duration for device updates.</span></span> <span data-ttu-id="10bd7-186">Gültige Werte: 0 bis 5.</span><span class="sxs-lookup"><span data-stu-id="10bd7-186">Valid values 0 to 5</span></span>|
|<span data-ttu-id="10bd7-187">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="10bd7-187">maintenanceWindowStartTime</span></span>|<span data-ttu-id="10bd7-188">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="10bd7-188">TimeOfDay</span></span>|<span data-ttu-id="10bd7-189">Beginn des Wartungsfensters für Geräteupdates</span><span class="sxs-lookup"><span data-stu-id="10bd7-189">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="10bd7-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="10bd7-190">miracastChannel</span></span>|[<span data-ttu-id="10bd7-191">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="10bd7-191">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="10bd7-192">Kanal.</span><span class="sxs-lookup"><span data-stu-id="10bd7-192">The channel.</span></span> <span data-ttu-id="10bd7-193">Mögliche Werte sind: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne` und `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="10bd7-193">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="10bd7-194">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="10bd7-194">miracastBlocked</span></span>|<span data-ttu-id="10bd7-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="10bd7-195">Boolean</span></span>|<span data-ttu-id="10bd7-196">Gibt an, ob eine drahtlose Projektion erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="10bd7-196">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="10bd7-197">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="10bd7-197">miracastRequirePin</span></span>|<span data-ttu-id="10bd7-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="10bd7-198">Boolean</span></span>|<span data-ttu-id="10bd7-199">Gibt an, ob für eine drahtlose Projektion die Eingabe einer PIN erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="10bd7-199">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="10bd7-200">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="10bd7-200">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="10bd7-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="10bd7-201">Boolean</span></span>|<span data-ttu-id="10bd7-202">Gibt an, ob die Funktion „Meine Besprechungen und Dateien“ im Startmenü deaktiviert werden soll. In diesem Bereich werden die Office 365-Besprechungen und -Dateien des angemeldeten Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="10bd7-202">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="10bd7-203">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="10bd7-203">settingsBlockSessionResume</span></span>|<span data-ttu-id="10bd7-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="10bd7-204">Boolean</span></span>|<span data-ttu-id="10bd7-205">Gibt an, ob Sitzungen nach einem Sitzungstimeout fortgeführt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="10bd7-205">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="10bd7-206">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="10bd7-206">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="10bd7-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="10bd7-207">Boolean</span></span>|<span data-ttu-id="10bd7-208">Gibt an, ob das Anmeldedialogfeld automatisch mit den Eingeladenen aus geplanten Besprechungen befüllt werden darf.</span><span class="sxs-lookup"><span data-stu-id="10bd7-208">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="10bd7-209">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="10bd7-209">settingsDefaultVolume</span></span>|<span data-ttu-id="10bd7-210">Int32</span><span class="sxs-lookup"><span data-stu-id="10bd7-210">Int32</span></span>|<span data-ttu-id="10bd7-211">Legt die Standardlautstärke für neue Sitzungen fest.</span><span class="sxs-lookup"><span data-stu-id="10bd7-211">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="10bd7-212">Zulässige Werte sind 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="10bd7-212">Permitted values are 0-100.</span></span> <span data-ttu-id="10bd7-213">Der Standardwert lautet 45.</span><span class="sxs-lookup"><span data-stu-id="10bd7-213">The default is 45.</span></span> <span data-ttu-id="10bd7-214">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="10bd7-214">Valid values 0 to 100</span></span>|
|<span data-ttu-id="10bd7-215">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="10bd7-215">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="10bd7-216">Int32</span><span class="sxs-lookup"><span data-stu-id="10bd7-216">Int32</span></span>|<span data-ttu-id="10bd7-217">Gibt den Zeitraum in Minuten an, nach dem der Bildschirm des Hub-Systems abgeschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="10bd7-217">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="10bd7-218">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="10bd7-218">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="10bd7-219">Int32</span><span class="sxs-lookup"><span data-stu-id="10bd7-219">Int32</span></span>|<span data-ttu-id="10bd7-220">Gibt den Zeitraum in Minuten an, nach dem es zu einem Sitzungstimeout kommt.</span><span class="sxs-lookup"><span data-stu-id="10bd7-220">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="10bd7-221">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="10bd7-221">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="10bd7-222">Int32</span><span class="sxs-lookup"><span data-stu-id="10bd7-222">Int32</span></span>|<span data-ttu-id="10bd7-223">Gibt den Zeitraum in Minuten an, nach dem das Hub-System in den Energiesparmodus geschaltet wird.</span><span class="sxs-lookup"><span data-stu-id="10bd7-223">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="10bd7-224">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="10bd7-224">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="10bd7-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="10bd7-225">Boolean</span></span>|<span data-ttu-id="10bd7-226">Gibt an, ob der Willkommensbildschirm automatisch angezeigt werden soll, sobald jemand den Raum betritt.</span><span class="sxs-lookup"><span data-stu-id="10bd7-226">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="10bd7-227">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="10bd7-227">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="10bd7-228">String</span><span class="sxs-lookup"><span data-stu-id="10bd7-228">String</span></span>|<span data-ttu-id="10bd7-229">URL zum Hintergrundbild für den Willkommensbildschirm.</span><span class="sxs-lookup"><span data-stu-id="10bd7-229">The welcome screen background image URL.</span></span> <span data-ttu-id="10bd7-230">Die URL muss das HTTPS-Protokoll verwenden und ein PNG-Bild zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="10bd7-230">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="10bd7-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="10bd7-231">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="10bd7-232">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="10bd7-232">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="10bd7-233">Die Informationen, die im Willkommensbildschirm angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="10bd7-233">The welcome screen meeting information shown.</span></span> <span data-ttu-id="10bd7-234">Mögliche Werte sind: `userDefined`, `showOrganizerAndTimeOnly` und `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="10bd7-234">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="10bd7-235">Antwort</span><span class="sxs-lookup"><span data-stu-id="10bd7-235">Response</span></span>
<span data-ttu-id="10bd7-236">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="10bd7-236">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10bd7-237">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10bd7-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="10bd7-238">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10bd7-238">Request</span></span>
<span data-ttu-id="10bd7-239">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10bd7-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="10bd7-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="10bd7-240">Response</span></span>
<span data-ttu-id="10bd7-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10bd7-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




