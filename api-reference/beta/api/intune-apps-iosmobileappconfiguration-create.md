---
title: iosMobileAppConfiguration erstellen
description: Erstellen eines neuen iosMobileAppConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fd3b9b94d94f78db0db69d5b6e69d269ba0e7bcc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418939"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="77075-103">iosMobileAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="77075-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="77075-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="77075-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="77075-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77075-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77075-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77075-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77075-107">Erstellen eines neuen [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="77075-107">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77075-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77075-108">Prerequisites</span></span>
<span data-ttu-id="77075-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="77075-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="77075-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77075-111">Permission type</span></span>|<span data-ttu-id="77075-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77075-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77075-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77075-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77075-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77075-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="77075-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77075-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77075-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77075-116">Not supported.</span></span>|
|<span data-ttu-id="77075-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77075-117">Application</span></span>|<span data-ttu-id="77075-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77075-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77075-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77075-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="77075-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77075-120">Request headers</span></span>
|<span data-ttu-id="77075-121">Header</span><span class="sxs-lookup"><span data-stu-id="77075-121">Header</span></span>|<span data-ttu-id="77075-122">Wert</span><span class="sxs-lookup"><span data-stu-id="77075-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77075-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="77075-123">Authorization</span></span>|<span data-ttu-id="77075-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="77075-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77075-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="77075-125">Accept</span></span>|<span data-ttu-id="77075-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77075-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77075-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77075-127">Request body</span></span>
<span data-ttu-id="77075-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs iosMobileAppConfiguration an.</span><span class="sxs-lookup"><span data-stu-id="77075-128">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="77075-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs iosMobileAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="77075-129">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="77075-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77075-130">Property</span></span>|<span data-ttu-id="77075-131">Typ</span><span class="sxs-lookup"><span data-stu-id="77075-131">Type</span></span>|<span data-ttu-id="77075-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77075-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77075-133">id</span><span class="sxs-lookup"><span data-stu-id="77075-133">id</span></span>|<span data-ttu-id="77075-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77075-134">String</span></span>|<span data-ttu-id="77075-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="77075-135">Key of the entity.</span></span> <span data-ttu-id="77075-136">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77075-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="77075-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="77075-137">targetedMobileApps</span></span>|<span data-ttu-id="77075-138">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="77075-138">String collection</span></span>|<span data-ttu-id="77075-139">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="77075-139">the associated app.</span></span> <span data-ttu-id="77075-140">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77075-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="77075-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="77075-141">roleScopeTagIds</span></span>|<span data-ttu-id="77075-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="77075-142">String collection</span></span>|<span data-ttu-id="77075-143">Liste der Bereich Tags für diese App Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="77075-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="77075-144">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77075-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="77075-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77075-145">createdDateTime</span></span>|<span data-ttu-id="77075-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77075-146">DateTimeOffset</span></span>|<span data-ttu-id="77075-147">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="77075-147">DateTime the object was created.</span></span> <span data-ttu-id="77075-148">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77075-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="77075-149">description</span><span class="sxs-lookup"><span data-stu-id="77075-149">description</span></span>|<span data-ttu-id="77075-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77075-150">String</span></span>|<span data-ttu-id="77075-151">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="77075-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="77075-152">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77075-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="77075-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77075-153">lastModifiedDateTime</span></span>|<span data-ttu-id="77075-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77075-154">DateTimeOffset</span></span>|<span data-ttu-id="77075-155">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="77075-155">DateTime the object was last modified.</span></span> <span data-ttu-id="77075-156">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77075-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="77075-157">displayName</span><span class="sxs-lookup"><span data-stu-id="77075-157">displayName</span></span>|<span data-ttu-id="77075-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77075-158">String</span></span>|<span data-ttu-id="77075-159">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="77075-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="77075-160">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77075-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="77075-161">version</span><span class="sxs-lookup"><span data-stu-id="77075-161">version</span></span>|<span data-ttu-id="77075-162">Int32</span><span class="sxs-lookup"><span data-stu-id="77075-162">Int32</span></span>|<span data-ttu-id="77075-163">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="77075-163">Version of the device configuration.</span></span> <span data-ttu-id="77075-164">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77075-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="77075-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="77075-165">encodedSettingXml</span></span>|<span data-ttu-id="77075-166">Binary</span><span class="sxs-lookup"><span data-stu-id="77075-166">Binary</span></span>|<span data-ttu-id="77075-167">Base64-binärcodierte MDM-App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="77075-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="77075-168">Einstellungen</span><span class="sxs-lookup"><span data-stu-id="77075-168">settings</span></span>|<span data-ttu-id="77075-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="77075-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="77075-170">App-Konfigurationseinstellungselemente</span><span class="sxs-lookup"><span data-stu-id="77075-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="77075-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="77075-171">Response</span></span>
<span data-ttu-id="77075-172">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="77075-172">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77075-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77075-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="77075-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77075-174">Request</span></span>
<span data-ttu-id="77075-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77075-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 596

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="77075-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="77075-176">Response</span></span>
<span data-ttu-id="77075-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77075-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 768

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```




