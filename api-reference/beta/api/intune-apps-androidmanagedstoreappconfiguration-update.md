---
title: AndroidManagedStoreAppConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidManagedStoreAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e14992fd5f7698f28fb376ecb9cf8355918dfbf4
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572138"
---
# <a name="update-androidmanagedstoreappconfiguration"></a><span data-ttu-id="ad09f-103">AndroidManagedStoreAppConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ad09f-103">Update androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="ad09f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ad09f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad09f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ad09f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad09f-106">Aktualisieren der Eigenschaften eines [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ad09f-106">Update the properties of a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad09f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ad09f-107">Prerequisites</span></span>
<span data-ttu-id="ad09f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ad09f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ad09f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ad09f-110">Permission type</span></span>|<span data-ttu-id="ad09f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ad09f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad09f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ad09f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad09f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad09f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad09f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ad09f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad09f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ad09f-115">Not supported.</span></span>|
|<span data-ttu-id="ad09f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ad09f-116">Application</span></span>|<span data-ttu-id="ad09f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ad09f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad09f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad09f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ad09f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ad09f-119">Request headers</span></span>
|<span data-ttu-id="ad09f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ad09f-120">Header</span></span>|<span data-ttu-id="ad09f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ad09f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad09f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad09f-122">Authorization</span></span>|<span data-ttu-id="ad09f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ad09f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad09f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ad09f-124">Accept</span></span>|<span data-ttu-id="ad09f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad09f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad09f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ad09f-126">Request body</span></span>
<span data-ttu-id="ad09f-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ad09f-127">In the request body, supply a JSON representation for the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

<span data-ttu-id="ad09f-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ad09f-128">The following table shows the properties that are required when you create the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span></span>

|<span data-ttu-id="ad09f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad09f-129">Property</span></span>|<span data-ttu-id="ad09f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ad09f-130">Type</span></span>|<span data-ttu-id="ad09f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad09f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad09f-132">id</span><span class="sxs-lookup"><span data-stu-id="ad09f-132">id</span></span>|<span data-ttu-id="ad09f-133">String</span><span class="sxs-lookup"><span data-stu-id="ad09f-133">String</span></span>|<span data-ttu-id="ad09f-134">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="ad09f-134">Key of the entity.</span></span> <span data-ttu-id="ad09f-135">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad09f-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad09f-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ad09f-136">targetedMobileApps</span></span>|<span data-ttu-id="ad09f-137">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ad09f-137">String collection</span></span>|<span data-ttu-id="ad09f-138">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="ad09f-138">the associated app.</span></span> <span data-ttu-id="ad09f-139">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad09f-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad09f-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="ad09f-140">roleScopeTagIds</span></span>|<span data-ttu-id="ad09f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ad09f-141">String collection</span></span>|<span data-ttu-id="ad09f-142">Liste der Bereichs Tags für diese APP-Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="ad09f-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="ad09f-143">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad09f-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad09f-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad09f-144">createdDateTime</span></span>|<span data-ttu-id="ad09f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad09f-145">DateTimeOffset</span></span>|<span data-ttu-id="ad09f-146">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ad09f-146">DateTime the object was created.</span></span> <span data-ttu-id="ad09f-147">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad09f-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad09f-148">description</span><span class="sxs-lookup"><span data-stu-id="ad09f-148">description</span></span>|<span data-ttu-id="ad09f-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ad09f-149">String</span></span>|<span data-ttu-id="ad09f-150">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ad09f-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ad09f-151">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad09f-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad09f-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad09f-152">lastModifiedDateTime</span></span>|<span data-ttu-id="ad09f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad09f-153">DateTimeOffset</span></span>|<span data-ttu-id="ad09f-154">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ad09f-154">DateTime the object was last modified.</span></span> <span data-ttu-id="ad09f-155">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad09f-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad09f-156">displayName</span><span class="sxs-lookup"><span data-stu-id="ad09f-156">displayName</span></span>|<span data-ttu-id="ad09f-157">String</span><span class="sxs-lookup"><span data-stu-id="ad09f-157">String</span></span>|<span data-ttu-id="ad09f-158">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ad09f-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ad09f-159">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad09f-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad09f-160">version</span><span class="sxs-lookup"><span data-stu-id="ad09f-160">version</span></span>|<span data-ttu-id="ad09f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="ad09f-161">Int32</span></span>|<span data-ttu-id="ad09f-162">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ad09f-162">Version of the device configuration.</span></span> <span data-ttu-id="ad09f-163">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad09f-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad09f-164">packageId</span><span class="sxs-lookup"><span data-stu-id="ad09f-164">packageId</span></span>|<span data-ttu-id="ad09f-165">String</span><span class="sxs-lookup"><span data-stu-id="ad09f-165">String</span></span>|<span data-ttu-id="ad09f-166">Android Enterprise App-Konfigurationspaket-ID.</span><span class="sxs-lookup"><span data-stu-id="ad09f-166">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="ad09f-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="ad09f-167">payloadJson</span></span>|<span data-ttu-id="ad09f-168">String</span><span class="sxs-lookup"><span data-stu-id="ad09f-168">String</span></span>|<span data-ttu-id="ad09f-169">JSON-Nutzlast der Android Enterprise-App-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="ad09f-169">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="ad09f-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="ad09f-170">permissionActions</span></span>|<span data-ttu-id="ad09f-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="ad09f-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="ad09f-172">Liste der Android-App-Berechtigungen und entsprechende Berechtigungs Aktionen.</span><span class="sxs-lookup"><span data-stu-id="ad09f-172">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="ad09f-173">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="ad09f-173">appSupportsOemConfig</span></span>|<span data-ttu-id="ad09f-174">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ad09f-174">Boolean</span></span>|<span data-ttu-id="ad09f-175">Gibt an, ob diese AppConfig eine OEMConfig-Richtlinie ist.</span><span class="sxs-lookup"><span data-stu-id="ad09f-175">Whether or not this AppConfig is an OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="ad09f-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad09f-176">Response</span></span>
<span data-ttu-id="ad09f-177">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ad09f-177">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad09f-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ad09f-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad09f-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad09f-179">Request</span></span>
<span data-ttu-id="ad09f-180">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ad09f-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 592

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ],
  "appSupportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="ad09f-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad09f-181">Response</span></span>
<span data-ttu-id="ad09f-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ad09f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 764

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "id": "919a9335-9335-919a-3593-9a9135939a91",
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
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ],
  "appSupportsOemConfig": true
}
```




