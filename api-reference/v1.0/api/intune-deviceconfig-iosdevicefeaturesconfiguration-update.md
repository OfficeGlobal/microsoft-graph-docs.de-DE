---
title: Aktualisieren von „iosDeviceFeaturesConfiguration“
description: Aktualisiert die Eigenschaften eines iosDeviceFeaturesConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32746cfbbdd65255108c9cc0df3fa9dd587ba09a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962358"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="ea1ef-103">Aktualisieren von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="ea1ef-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="ea1ef-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea1ef-105">Aktualisiert die Eigenschaften eines [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-105">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea1ef-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ea1ef-106">Prerequisites</span></span>
<span data-ttu-id="ea1ef-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea1ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea1ef-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea1ef-109">Permission type</span></span>|<span data-ttu-id="ea1ef-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea1ef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea1ef-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea1ef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ea1ef-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea1ef-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea1ef-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea1ef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea1ef-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea1ef-114">Not supported.</span></span>|
|<span data-ttu-id="ea1ef-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea1ef-115">Application</span></span>|<span data-ttu-id="ea1ef-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea1ef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea1ef-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea1ef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ea1ef-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea1ef-118">Request headers</span></span>
|<span data-ttu-id="ea1ef-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ea1ef-119">Header</span></span>|<span data-ttu-id="ea1ef-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ea1ef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea1ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea1ef-121">Authorization</span></span>|<span data-ttu-id="ea1ef-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ea1ef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea1ef-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ea1ef-123">Accept</span></span>|<span data-ttu-id="ea1ef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ea1ef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea1ef-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea1ef-125">Request body</span></span>
<span data-ttu-id="ea1ef-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-126">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="ea1ef-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-127">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="ea1ef-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea1ef-128">Property</span></span>|<span data-ttu-id="ea1ef-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ea1ef-129">Type</span></span>|<span data-ttu-id="ea1ef-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea1ef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea1ef-131">id</span><span class="sxs-lookup"><span data-stu-id="ea1ef-131">id</span></span>|<span data-ttu-id="ea1ef-132">String</span><span class="sxs-lookup"><span data-stu-id="ea1ef-132">String</span></span>|<span data-ttu-id="ea1ef-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ea1ef-133">Key of the entity.</span></span> <span data-ttu-id="ea1ef-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea1ef-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea1ef-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea1ef-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ea1ef-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea1ef-136">DateTimeOffset</span></span>|<span data-ttu-id="ea1ef-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-137">DateTime the object was last modified.</span></span> <span data-ttu-id="ea1ef-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea1ef-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea1ef-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea1ef-139">createdDateTime</span></span>|<span data-ttu-id="ea1ef-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea1ef-140">DateTimeOffset</span></span>|<span data-ttu-id="ea1ef-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-141">DateTime the object was created.</span></span> <span data-ttu-id="ea1ef-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea1ef-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea1ef-143">description</span><span class="sxs-lookup"><span data-stu-id="ea1ef-143">description</span></span>|<span data-ttu-id="ea1ef-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea1ef-144">String</span></span>|<span data-ttu-id="ea1ef-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ea1ef-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ea1ef-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea1ef-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea1ef-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ea1ef-147">displayName</span></span>|<span data-ttu-id="ea1ef-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea1ef-148">String</span></span>|<span data-ttu-id="ea1ef-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ea1ef-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ea1ef-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea1ef-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea1ef-151">Version</span><span class="sxs-lookup"><span data-stu-id="ea1ef-151">version</span></span>|<span data-ttu-id="ea1ef-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ea1ef-152">Int32</span></span>|<span data-ttu-id="ea1ef-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-153">Version of the device configuration.</span></span> <span data-ttu-id="ea1ef-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea1ef-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea1ef-155">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="ea1ef-155">assetTagTemplate</span></span>|<span data-ttu-id="ea1ef-156">String</span><span class="sxs-lookup"><span data-stu-id="ea1ef-156">String</span></span>|<span data-ttu-id="ea1ef-157">Bestandskennzeicheninformationen zum Gerät. Sie werden im Anmeldefenster und im Sperrbildschirm angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-157">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="ea1ef-158">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="ea1ef-158">lockScreenFootnote</span></span>|<span data-ttu-id="ea1ef-159">String</span><span class="sxs-lookup"><span data-stu-id="ea1ef-159">String</span></span>|<span data-ttu-id="ea1ef-160">Fußnote, die im Anmeldefenster und im Sperrbildschirm angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-160">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="ea1ef-161">Verfügbar ab iOS 9.3.1.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-161">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="ea1ef-162">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="ea1ef-162">homeScreenDockIcons</span></span>|<span data-ttu-id="ea1ef-163">Collection von Objekten des Typs [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="ea1ef-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="ea1ef-164">Liste der Apps und Ordner, die im Home-Bildschirm-Dock angezeigt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-164">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="ea1ef-165">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-165">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ea1ef-166">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="ea1ef-166">homeScreenPages</span></span>|<span data-ttu-id="ea1ef-167">Collection von Objekten des Typs [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="ea1ef-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="ea1ef-168">Liste der Seiten auf dem Home-Bildschirm.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-168">A list of pages on the Home Screen.</span></span> <span data-ttu-id="ea1ef-169">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-169">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ea1ef-170">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="ea1ef-170">notificationSettings</span></span>|<span data-ttu-id="ea1ef-171">Collection von Objekten des Typs [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ea1ef-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="ea1ef-172">Benachrichtigungseinstellungen für jede Bundle-ID. Gilt nur für Geräte im Betreuungsmodus (iOS 9.3 und höher).</span><span class="sxs-lookup"><span data-stu-id="ea1ef-172">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="ea1ef-173">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-173">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ea1ef-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea1ef-174">Response</span></span>
<span data-ttu-id="ea1ef-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-175">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea1ef-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea1ef-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea1ef-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea1ef-177">Request</span></span>
<span data-ttu-id="ea1ef-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="ea1ef-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea1ef-179">Response</span></span>
<span data-ttu-id="ea1ef-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea1ef-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
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
  ]
}
```



