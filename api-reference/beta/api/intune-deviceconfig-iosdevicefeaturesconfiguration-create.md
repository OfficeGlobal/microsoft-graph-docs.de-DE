---
title: Erstellen von „iosDeviceFeaturesConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs iosDeviceFeaturesConfiguration.
author: tfitzmac
ms.openlocfilehash: dcb9819505cf429f6217dc375fcbd0c3366dee89
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310885"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="7e044-103">Erstellen von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="7e044-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="7e044-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7e044-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e044-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7e044-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e044-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7e044-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e044-107">Diese Methode erstellt ein neues Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e044-107">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e044-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7e044-108">Prerequisites</span></span>
<span data-ttu-id="7e044-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e044-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e044-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7e044-111">Permission type</span></span>|<span data-ttu-id="7e044-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7e044-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e044-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7e044-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e044-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e044-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7e044-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7e044-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e044-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e044-116">Not supported.</span></span>|
|<span data-ttu-id="7e044-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7e044-117">Application</span></span>|<span data-ttu-id="7e044-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e044-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e044-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e044-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7e044-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7e044-120">Request headers</span></span>
|<span data-ttu-id="7e044-121">Header</span><span class="sxs-lookup"><span data-stu-id="7e044-121">Header</span></span>|<span data-ttu-id="7e044-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7e044-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e044-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7e044-123">Authorization</span></span>|<span data-ttu-id="7e044-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7e044-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e044-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7e044-125">Accept</span></span>|<span data-ttu-id="7e044-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e044-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e044-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7e044-127">Request body</span></span>
<span data-ttu-id="7e044-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosDeviceFeaturesConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="7e044-128">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="7e044-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosDeviceFeaturesConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="7e044-129">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="7e044-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e044-130">Property</span></span>|<span data-ttu-id="7e044-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7e044-131">Type</span></span>|<span data-ttu-id="7e044-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e044-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e044-133">id</span><span class="sxs-lookup"><span data-stu-id="7e044-133">id</span></span>|<span data-ttu-id="7e044-134">String</span><span class="sxs-lookup"><span data-stu-id="7e044-134">String</span></span>|<span data-ttu-id="7e044-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7e044-135">Key of the entity.</span></span> <span data-ttu-id="7e044-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e044-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e044-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e044-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7e044-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e044-138">DateTimeOffset</span></span>|<span data-ttu-id="7e044-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7e044-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7e044-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e044-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e044-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7e044-141">roleScopeTagIds</span></span>|<span data-ttu-id="7e044-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="7e044-142">String collection</span></span>|<span data-ttu-id="7e044-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="7e044-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7e044-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e044-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e044-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7e044-145">supportsScopeTags</span></span>|<span data-ttu-id="7e044-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="7e044-146">Boolean</span></span>|<span data-ttu-id="7e044-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7e044-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7e044-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="7e044-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7e044-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="7e044-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7e044-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7e044-150">This property is read-only.</span></span> <span data-ttu-id="7e044-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e044-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e044-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e044-152">createdDateTime</span></span>|<span data-ttu-id="7e044-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e044-153">DateTimeOffset</span></span>|<span data-ttu-id="7e044-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7e044-154">DateTime the object was created.</span></span> <span data-ttu-id="7e044-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e044-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e044-156">description</span><span class="sxs-lookup"><span data-stu-id="7e044-156">description</span></span>|<span data-ttu-id="7e044-157">String</span><span class="sxs-lookup"><span data-stu-id="7e044-157">String</span></span>|<span data-ttu-id="7e044-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7e044-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7e044-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e044-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e044-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7e044-160">displayName</span></span>|<span data-ttu-id="7e044-161">String</span><span class="sxs-lookup"><span data-stu-id="7e044-161">String</span></span>|<span data-ttu-id="7e044-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7e044-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7e044-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e044-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e044-164">Version</span><span class="sxs-lookup"><span data-stu-id="7e044-164">version</span></span>|<span data-ttu-id="7e044-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7e044-165">Int32</span></span>|<span data-ttu-id="7e044-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7e044-166">Version of the device configuration.</span></span> <span data-ttu-id="7e044-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7e044-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e044-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="7e044-168">airPrintDestinations</span></span>|<span data-ttu-id="7e044-169">[AirPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7e044-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="7e044-170">Ein Array von AirPrint aus, die immer angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="7e044-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="7e044-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="7e044-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7e044-172">Geerbt von [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="7e044-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="7e044-173">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="7e044-173">assetTagTemplate</span></span>|<span data-ttu-id="7e044-174">String</span><span class="sxs-lookup"><span data-stu-id="7e044-174">String</span></span>|<span data-ttu-id="7e044-175">Bestandskennzeicheninformationen zum Gerät. Sie werden im Anmeldefenster und im Sperrbildschirm angezeigt.</span><span class="sxs-lookup"><span data-stu-id="7e044-175">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="7e044-176">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="7e044-176">contentFilterSettings</span></span>|[<span data-ttu-id="7e044-177">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="7e044-177">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="7e044-178">Ruft ab oder legt diesen fest iOS Einstellungen für die Inhaltsfilterung Web, nur überwachten Modus</span><span class="sxs-lookup"><span data-stu-id="7e044-178">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="7e044-179">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="7e044-179">lockScreenFootnote</span></span>|<span data-ttu-id="7e044-180">String</span><span class="sxs-lookup"><span data-stu-id="7e044-180">String</span></span>|<span data-ttu-id="7e044-181">Fußnote, die im Anmeldefenster und im Sperrbildschirm angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="7e044-181">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="7e044-182">Verfügbar ab iOS 9.3.1.</span><span class="sxs-lookup"><span data-stu-id="7e044-182">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="7e044-183">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="7e044-183">homeScreenDockIcons</span></span>|<span data-ttu-id="7e044-184">Collection von Objekten des Typs [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="7e044-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="7e044-185">Liste der Apps und Ordner, die im Home-Bildschirm-Dock angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="7e044-185">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="7e044-186">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="7e044-186">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7e044-187">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="7e044-187">homeScreenPages</span></span>|<span data-ttu-id="7e044-188">Collection von Objekten des Typs [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="7e044-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="7e044-189">Liste der Seiten auf dem Home-Bildschirm.</span><span class="sxs-lookup"><span data-stu-id="7e044-189">A list of pages on the Home Screen.</span></span> <span data-ttu-id="7e044-190">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="7e044-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7e044-191">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="7e044-191">notificationSettings</span></span>|<span data-ttu-id="7e044-192">Collection von Objekten des Typs [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="7e044-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="7e044-193">Benachrichtigungseinstellungen für jede Bundle-ID. Gilt nur für Geräte im Betreuungsmodus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="7e044-193">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="7e044-194">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="7e044-194">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7e044-195">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="7e044-195">singleSignOnSettings</span></span>|[<span data-ttu-id="7e044-196">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="7e044-196">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="7e044-197">Die Kerberos-anmeldeeinstellungen, mit denen apps auf das Empfangen von Geräten reibungslos authentifizieren.</span><span class="sxs-lookup"><span data-stu-id="7e044-197">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|



## <a name="response"></a><span data-ttu-id="7e044-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e044-198">Response</span></span>
<span data-ttu-id="7e044-199">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7e044-199">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e044-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7e044-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e044-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e044-201">Request</span></span>
<span data-ttu-id="7e044-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7e044-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3543

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
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

### <a name="response"></a><span data-ttu-id="7e044-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e044-203">Response</span></span>
<span data-ttu-id="7e044-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e044-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





