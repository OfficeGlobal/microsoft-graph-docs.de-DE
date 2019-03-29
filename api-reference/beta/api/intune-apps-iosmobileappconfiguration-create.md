---
title: iosMobileAppConfiguration erstellen
description: Erstellen eines neuen iosMobileAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd0b63b2d3682f080ae920b51f1515c56fbdb3c5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964283"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="f9f74-103">iosMobileAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="f9f74-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="f9f74-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9f74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9f74-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f9f74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9f74-106">Erstellen eines neuen [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f9f74-106">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9f74-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f9f74-107">Prerequisites</span></span>
<span data-ttu-id="f9f74-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9f74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9f74-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9f74-110">Permission type</span></span>|<span data-ttu-id="f9f74-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9f74-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9f74-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9f74-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9f74-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9f74-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9f74-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9f74-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9f74-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9f74-115">Not supported.</span></span>|
|<span data-ttu-id="f9f74-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9f74-116">Application</span></span>|<span data-ttu-id="f9f74-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9f74-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9f74-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9f74-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f9f74-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9f74-119">Request headers</span></span>
|<span data-ttu-id="f9f74-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f9f74-120">Header</span></span>|<span data-ttu-id="f9f74-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f9f74-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9f74-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9f74-122">Authorization</span></span>|<span data-ttu-id="f9f74-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f9f74-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9f74-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f9f74-124">Accept</span></span>|<span data-ttu-id="f9f74-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9f74-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9f74-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9f74-126">Request body</span></span>
<span data-ttu-id="f9f74-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs iosMobileAppConfiguration an.</span><span class="sxs-lookup"><span data-stu-id="f9f74-127">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="f9f74-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs iosMobileAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="f9f74-128">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="f9f74-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9f74-129">Property</span></span>|<span data-ttu-id="f9f74-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f9f74-130">Type</span></span>|<span data-ttu-id="f9f74-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9f74-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9f74-132">id</span><span class="sxs-lookup"><span data-stu-id="f9f74-132">id</span></span>|<span data-ttu-id="f9f74-133">String</span><span class="sxs-lookup"><span data-stu-id="f9f74-133">String</span></span>|<span data-ttu-id="f9f74-134">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="f9f74-134">Key of the entity.</span></span> <span data-ttu-id="f9f74-135">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f74-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f9f74-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="f9f74-136">targetedMobileApps</span></span>|<span data-ttu-id="f9f74-137">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f9f74-137">String collection</span></span>|<span data-ttu-id="f9f74-138">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="f9f74-138">the associated app.</span></span> <span data-ttu-id="f9f74-139">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f74-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f9f74-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="f9f74-140">roleScopeTagIds</span></span>|<span data-ttu-id="f9f74-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f9f74-141">String collection</span></span>|<span data-ttu-id="f9f74-142">Liste der Bereichs Tags für diese APP-Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="f9f74-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="f9f74-143">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f74-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f9f74-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f74-144">createdDateTime</span></span>|<span data-ttu-id="f9f74-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f74-145">DateTimeOffset</span></span>|<span data-ttu-id="f9f74-146">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f9f74-146">DateTime the object was created.</span></span> <span data-ttu-id="f9f74-147">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f74-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f9f74-148">description</span><span class="sxs-lookup"><span data-stu-id="f9f74-148">description</span></span>|<span data-ttu-id="f9f74-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9f74-149">String</span></span>|<span data-ttu-id="f9f74-150">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f9f74-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f9f74-151">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f74-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f9f74-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f74-152">lastModifiedDateTime</span></span>|<span data-ttu-id="f9f74-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f74-153">DateTimeOffset</span></span>|<span data-ttu-id="f9f74-154">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f9f74-154">DateTime the object was last modified.</span></span> <span data-ttu-id="f9f74-155">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f74-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f9f74-156">displayName</span><span class="sxs-lookup"><span data-stu-id="f9f74-156">displayName</span></span>|<span data-ttu-id="f9f74-157">String</span><span class="sxs-lookup"><span data-stu-id="f9f74-157">String</span></span>|<span data-ttu-id="f9f74-158">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f9f74-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f9f74-159">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f74-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f9f74-160">version</span><span class="sxs-lookup"><span data-stu-id="f9f74-160">version</span></span>|<span data-ttu-id="f9f74-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f9f74-161">Int32</span></span>|<span data-ttu-id="f9f74-162">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f9f74-162">Version of the device configuration.</span></span> <span data-ttu-id="f9f74-163">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f74-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f9f74-164">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="f9f74-164">encodedSettingXml</span></span>|<span data-ttu-id="f9f74-165">Binary</span><span class="sxs-lookup"><span data-stu-id="f9f74-165">Binary</span></span>|<span data-ttu-id="f9f74-166">Base64-binärcodierte MDM-App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="f9f74-166">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="f9f74-167">Einstellungen</span><span class="sxs-lookup"><span data-stu-id="f9f74-167">settings</span></span>|<span data-ttu-id="f9f74-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f9f74-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="f9f74-169">App-Konfigurationseinstellungselemente</span><span class="sxs-lookup"><span data-stu-id="f9f74-169">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="f9f74-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9f74-170">Response</span></span>
<span data-ttu-id="f9f74-171">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f9f74-171">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9f74-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9f74-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9f74-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9f74-173">Request</span></span>
<span data-ttu-id="f9f74-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9f74-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9f74-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9f74-175">Response</span></span>
<span data-ttu-id="f9f74-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9f74-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




