---
title: iosUpdateConfiguration erstellen
description: Erstellen eines neuen iosUpdateConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14ac9743f0d94b2f4e273674921aadb9fe2e3ed4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963829"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="a09c8-103">iosUpdateConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="a09c8-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="a09c8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a09c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a09c8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a09c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a09c8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a09c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a09c8-107">Erstellen eines neuen [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a09c8-107">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a09c8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a09c8-108">Prerequisites</span></span>
<span data-ttu-id="a09c8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a09c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a09c8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a09c8-111">Permission type</span></span>|<span data-ttu-id="a09c8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a09c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a09c8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a09c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a09c8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a09c8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a09c8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a09c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a09c8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a09c8-116">Not supported.</span></span>|
|<span data-ttu-id="a09c8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a09c8-117">Application</span></span>|<span data-ttu-id="a09c8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a09c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a09c8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a09c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a09c8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a09c8-120">Request headers</span></span>
|<span data-ttu-id="a09c8-121">Header</span><span class="sxs-lookup"><span data-stu-id="a09c8-121">Header</span></span>|<span data-ttu-id="a09c8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a09c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a09c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a09c8-123">Authorization</span></span>|<span data-ttu-id="a09c8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a09c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a09c8-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a09c8-125">Accept</span></span>|<span data-ttu-id="a09c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a09c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a09c8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a09c8-127">Request body</span></span>
<span data-ttu-id="a09c8-128">Geben Sie im Anforderungstext eine JSON-Darstellung des iosUpdateConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a09c8-128">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="a09c8-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des iosUpdateConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a09c8-129">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="a09c8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a09c8-130">Property</span></span>|<span data-ttu-id="a09c8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a09c8-131">Type</span></span>|<span data-ttu-id="a09c8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a09c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a09c8-133">id</span><span class="sxs-lookup"><span data-stu-id="a09c8-133">id</span></span>|<span data-ttu-id="a09c8-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a09c8-134">String</span></span>|<span data-ttu-id="a09c8-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a09c8-135">Key of the entity.</span></span> <span data-ttu-id="a09c8-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a09c8-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09c8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a09c8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a09c8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a09c8-138">DateTimeOffset</span></span>|<span data-ttu-id="a09c8-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a09c8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a09c8-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a09c8-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09c8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a09c8-141">roleScopeTagIds</span></span>|<span data-ttu-id="a09c8-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="a09c8-142">String collection</span></span>|<span data-ttu-id="a09c8-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="a09c8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a09c8-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a09c8-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09c8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a09c8-145">supportsScopeTags</span></span>|<span data-ttu-id="a09c8-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a09c8-146">Boolean</span></span>|<span data-ttu-id="a09c8-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a09c8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a09c8-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a09c8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a09c8-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a09c8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a09c8-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a09c8-150">This property is read-only.</span></span> <span data-ttu-id="a09c8-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a09c8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09c8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a09c8-152">createdDateTime</span></span>|<span data-ttu-id="a09c8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a09c8-153">DateTimeOffset</span></span>|<span data-ttu-id="a09c8-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a09c8-154">DateTime the object was created.</span></span> <span data-ttu-id="a09c8-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a09c8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09c8-156">description</span><span class="sxs-lookup"><span data-stu-id="a09c8-156">description</span></span>|<span data-ttu-id="a09c8-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a09c8-157">String</span></span>|<span data-ttu-id="a09c8-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a09c8-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a09c8-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a09c8-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09c8-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a09c8-160">displayName</span></span>|<span data-ttu-id="a09c8-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a09c8-161">String</span></span>|<span data-ttu-id="a09c8-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a09c8-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a09c8-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a09c8-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09c8-164">Version</span><span class="sxs-lookup"><span data-stu-id="a09c8-164">version</span></span>|<span data-ttu-id="a09c8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a09c8-165">Int32</span></span>|<span data-ttu-id="a09c8-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a09c8-166">Version of the device configuration.</span></span> <span data-ttu-id="a09c8-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a09c8-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a09c8-168">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a09c8-168">isEnabled</span></span>|<span data-ttu-id="a09c8-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a09c8-169">Boolean</span></span>|<span data-ttu-id="a09c8-170">Die Einstellung wird in der Benutzeroberfläche aktiviert werden</span><span class="sxs-lookup"><span data-stu-id="a09c8-170">Is setting enabled in UI</span></span>|
|<span data-ttu-id="a09c8-171">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="a09c8-171">activeHoursStart</span></span>|<span data-ttu-id="a09c8-172">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a09c8-172">TimeOfDay</span></span>|<span data-ttu-id="a09c8-173">Beginn der aktiven Stunden (Als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Updates installiert werden sollen.)</span><span class="sxs-lookup"><span data-stu-id="a09c8-173">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="a09c8-174">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="a09c8-174">activeHoursEnd</span></span>|<span data-ttu-id="a09c8-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a09c8-175">TimeOfDay</span></span>|<span data-ttu-id="a09c8-176">Ende der aktiven Stunden (Als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Updates installiert werden sollen.)</span><span class="sxs-lookup"><span data-stu-id="a09c8-176">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="a09c8-177">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="a09c8-177">scheduledInstallDays</span></span>|<span data-ttu-id="a09c8-178">[DayOfWeek](../resources/intune-deviceconfig-dayofweek.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a09c8-178">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="a09c8-179">Tage in der Woche, für die aktive Stunden konfiguriert sind.</span><span class="sxs-lookup"><span data-stu-id="a09c8-179">Days in week for which active hours are configured.</span></span> <span data-ttu-id="a09c8-180">Diese Sammlung darf maximal 7 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a09c8-180">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="a09c8-181">Mögliche Werte sind: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday` und `saturday`.</span><span class="sxs-lookup"><span data-stu-id="a09c8-181">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="a09c8-182">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="a09c8-182">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="a09c8-183">Int32</span><span class="sxs-lookup"><span data-stu-id="a09c8-183">Int32</span></span>|<span data-ttu-id="a09c8-184">UTC-Zeitversatz in Minuten</span><span class="sxs-lookup"><span data-stu-id="a09c8-184">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="a09c8-185">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="a09c8-185">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="a09c8-186">Int32</span><span class="sxs-lookup"><span data-stu-id="a09c8-186">Int32</span></span>|<span data-ttu-id="a09c8-187">Tage vor Softwareupdates für iOS-Geräte, die im Bereich von 0 bis 90 inklusive sichtbar sind</span><span class="sxs-lookup"><span data-stu-id="a09c8-187">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="a09c8-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="a09c8-188">Response</span></span>
<span data-ttu-id="a09c8-189">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a09c8-189">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a09c8-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a09c8-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="a09c8-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a09c8-191">Request</span></span>
<span data-ttu-id="a09c8-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a09c8-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 546

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```

### <a name="response"></a><span data-ttu-id="a09c8-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="a09c8-193">Response</span></span>
<span data-ttu-id="a09c8-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a09c8-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 654

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```





