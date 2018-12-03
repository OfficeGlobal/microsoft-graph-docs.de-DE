---
title: Aktualisieren von „iosDeviceFeaturesConfiguration“
description: Aktualisiert die Eigenschaften eines iosDeviceFeaturesConfiguration-Objekts.
ms.openlocfilehash: c058f7730b94d412e5ea9aa3c0c7a984aeb35f1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065787"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="e4c77-103">Aktualisieren von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="e4c77-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="e4c77-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e4c77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4c77-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4c77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4c77-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e4c77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4c77-107">Aktualisiert die Eigenschaften eines [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4c77-107">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4c77-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e4c77-108">Prerequisites</span></span>
<span data-ttu-id="e4c77-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4c77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4c77-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4c77-111">Permission type</span></span>|<span data-ttu-id="e4c77-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4c77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4c77-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4c77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4c77-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4c77-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4c77-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4c77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4c77-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4c77-116">Not supported.</span></span>|
|<span data-ttu-id="e4c77-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4c77-117">Application</span></span>|<span data-ttu-id="e4c77-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4c77-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4c77-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4c77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e4c77-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4c77-120">Request headers</span></span>
|<span data-ttu-id="e4c77-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e4c77-121">Header</span></span>|<span data-ttu-id="e4c77-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e4c77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4c77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4c77-123">Authorization</span></span>|<span data-ttu-id="e4c77-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e4c77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4c77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4c77-125">Accept</span></span>|<span data-ttu-id="e4c77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4c77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4c77-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4c77-127">Request body</span></span>
<span data-ttu-id="e4c77-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e4c77-128">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="e4c77-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e4c77-129">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="e4c77-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4c77-130">Property</span></span>|<span data-ttu-id="e4c77-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e4c77-131">Type</span></span>|<span data-ttu-id="e4c77-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4c77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4c77-133">id</span><span class="sxs-lookup"><span data-stu-id="e4c77-133">id</span></span>|<span data-ttu-id="e4c77-134">String</span><span class="sxs-lookup"><span data-stu-id="e4c77-134">String</span></span>|<span data-ttu-id="e4c77-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e4c77-135">Key of the entity.</span></span> <span data-ttu-id="e4c77-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4c77-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4c77-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4c77-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e4c77-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4c77-138">DateTimeOffset</span></span>|<span data-ttu-id="e4c77-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4c77-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e4c77-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4c77-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4c77-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e4c77-141">roleScopeTagIds</span></span>|<span data-ttu-id="e4c77-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="e4c77-142">String collection</span></span>|<span data-ttu-id="e4c77-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="e4c77-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e4c77-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4c77-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4c77-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e4c77-145">supportsScopeTags</span></span>|<span data-ttu-id="e4c77-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="e4c77-146">Boolean</span></span>|<span data-ttu-id="e4c77-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4c77-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e4c77-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="e4c77-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e4c77-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="e4c77-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e4c77-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e4c77-150">This property is read-only.</span></span> <span data-ttu-id="e4c77-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4c77-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4c77-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4c77-152">createdDateTime</span></span>|<span data-ttu-id="e4c77-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4c77-153">DateTimeOffset</span></span>|<span data-ttu-id="e4c77-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4c77-154">DateTime the object was created.</span></span> <span data-ttu-id="e4c77-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4c77-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4c77-156">description</span><span class="sxs-lookup"><span data-stu-id="e4c77-156">description</span></span>|<span data-ttu-id="e4c77-157">String</span><span class="sxs-lookup"><span data-stu-id="e4c77-157">String</span></span>|<span data-ttu-id="e4c77-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e4c77-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e4c77-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4c77-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4c77-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e4c77-160">displayName</span></span>|<span data-ttu-id="e4c77-161">String</span><span class="sxs-lookup"><span data-stu-id="e4c77-161">String</span></span>|<span data-ttu-id="e4c77-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e4c77-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e4c77-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4c77-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4c77-164">Version</span><span class="sxs-lookup"><span data-stu-id="e4c77-164">version</span></span>|<span data-ttu-id="e4c77-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e4c77-165">Int32</span></span>|<span data-ttu-id="e4c77-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e4c77-166">Version of the device configuration.</span></span> <span data-ttu-id="e4c77-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4c77-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4c77-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="e4c77-168">airPrintDestinations</span></span>|<span data-ttu-id="e4c77-169">[AirPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e4c77-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="e4c77-170">Ein Array von AirPrint aus, die immer angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e4c77-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="e4c77-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="e4c77-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e4c77-172">Geerbt von [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="e4c77-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="e4c77-173">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="e4c77-173">assetTagTemplate</span></span>|<span data-ttu-id="e4c77-174">String</span><span class="sxs-lookup"><span data-stu-id="e4c77-174">String</span></span>|<span data-ttu-id="e4c77-175">Bestandskennzeicheninformationen zum Gerät. Sie werden im Anmeldefenster und im Sperrbildschirm angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e4c77-175">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="e4c77-176">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="e4c77-176">contentFilterSettings</span></span>|[<span data-ttu-id="e4c77-177">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="e4c77-177">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="e4c77-178">Ruft ab oder legt diesen fest iOS Einstellungen für die Inhaltsfilterung Web, nur überwachten Modus</span><span class="sxs-lookup"><span data-stu-id="e4c77-178">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="e4c77-179">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="e4c77-179">lockScreenFootnote</span></span>|<span data-ttu-id="e4c77-180">String</span><span class="sxs-lookup"><span data-stu-id="e4c77-180">String</span></span>|<span data-ttu-id="e4c77-181">Fußnote, die im Anmeldefenster und im Sperrbildschirm angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e4c77-181">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="e4c77-182">Verfügbar ab iOS 9.3.1.</span><span class="sxs-lookup"><span data-stu-id="e4c77-182">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="e4c77-183">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="e4c77-183">homeScreenDockIcons</span></span>|<span data-ttu-id="e4c77-184">Collection von Objekten des Typs [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="e4c77-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="e4c77-185">Liste der Apps und Ordner, die im Home-Bildschirm-Dock angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e4c77-185">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="e4c77-186">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="e4c77-186">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e4c77-187">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="e4c77-187">homeScreenPages</span></span>|<span data-ttu-id="e4c77-188">Collection von Objekten des Typs [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="e4c77-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="e4c77-189">Liste der Seiten auf dem Home-Bildschirm.</span><span class="sxs-lookup"><span data-stu-id="e4c77-189">A list of pages on the Home Screen.</span></span> <span data-ttu-id="e4c77-190">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="e4c77-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e4c77-191">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="e4c77-191">notificationSettings</span></span>|<span data-ttu-id="e4c77-192">Collection von Objekten des Typs [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e4c77-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="e4c77-193">Benachrichtigungseinstellungen für jede Bundle-ID. Gilt nur für Geräte im Betreuungsmodus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="e4c77-193">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="e4c77-194">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="e4c77-194">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e4c77-195">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="e4c77-195">singleSignOnSettings</span></span>|[<span data-ttu-id="e4c77-196">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="e4c77-196">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="e4c77-197">Die Kerberos-anmeldeeinstellungen, mit denen apps auf das Empfangen von Geräten reibungslos authentifizieren.</span><span class="sxs-lookup"><span data-stu-id="e4c77-197">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|



## <a name="response"></a><span data-ttu-id="e4c77-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4c77-198">Response</span></span>
<span data-ttu-id="e4c77-199">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e4c77-199">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4c77-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4c77-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4c77-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4c77-201">Request</span></span>
<span data-ttu-id="e4c77-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4c77-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3474

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  }
}
```

### <a name="response"></a><span data-ttu-id="e4c77-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4c77-203">Response</span></span>
<span data-ttu-id="e4c77-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4c77-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3651

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  }
}
```





