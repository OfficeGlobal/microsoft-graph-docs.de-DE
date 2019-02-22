---
title: AndroidManagedStoreAppConfiguration erstellen
description: Erstellen eines neuen androidManagedStoreAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f83097929793df891a17ceb1de5c08892fa32c9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169461"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="503b3-103">AndroidManagedStoreAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="503b3-103">Create androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="503b3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="503b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="503b3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="503b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="503b3-106">Erstellen eines neuen [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="503b3-106">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="503b3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="503b3-107">Prerequisites</span></span>
<span data-ttu-id="503b3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="503b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="503b3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="503b3-110">Permission type</span></span>|<span data-ttu-id="503b3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="503b3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="503b3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="503b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="503b3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="503b3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="503b3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="503b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="503b3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="503b3-115">Not supported.</span></span>|
|<span data-ttu-id="503b3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="503b3-116">Application</span></span>|<span data-ttu-id="503b3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="503b3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="503b3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="503b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="503b3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="503b3-119">Request headers</span></span>
|<span data-ttu-id="503b3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="503b3-120">Header</span></span>|<span data-ttu-id="503b3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="503b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="503b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="503b3-122">Authorization</span></span>|<span data-ttu-id="503b3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="503b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="503b3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="503b3-124">Accept</span></span>|<span data-ttu-id="503b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="503b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="503b3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="503b3-126">Request body</span></span>
<span data-ttu-id="503b3-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidManagedStoreAppConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="503b3-127">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="503b3-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidManagedStoreAppConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="503b3-128">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="503b3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="503b3-129">Property</span></span>|<span data-ttu-id="503b3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="503b3-130">Type</span></span>|<span data-ttu-id="503b3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="503b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="503b3-132">id</span><span class="sxs-lookup"><span data-stu-id="503b3-132">id</span></span>|<span data-ttu-id="503b3-133">string</span><span class="sxs-lookup"><span data-stu-id="503b3-133">String</span></span>|<span data-ttu-id="503b3-134">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="503b3-134">Key of the entity.</span></span> <span data-ttu-id="503b3-135">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="503b3-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="503b3-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="503b3-136">targetedMobileApps</span></span>|<span data-ttu-id="503b3-137">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="503b3-137">String collection</span></span>|<span data-ttu-id="503b3-138">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="503b3-138">the associated app.</span></span> <span data-ttu-id="503b3-139">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="503b3-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="503b3-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="503b3-140">roleScopeTagIds</span></span>|<span data-ttu-id="503b3-141">String collection</span><span class="sxs-lookup"><span data-stu-id="503b3-141">String collection</span></span>|<span data-ttu-id="503b3-142">Liste der Bereichs Tags für diese APP-Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="503b3-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="503b3-143">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="503b3-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="503b3-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="503b3-144">createdDateTime</span></span>|<span data-ttu-id="503b3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="503b3-145">DateTimeOffset</span></span>|<span data-ttu-id="503b3-146">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="503b3-146">DateTime the object was created.</span></span> <span data-ttu-id="503b3-147">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="503b3-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="503b3-148">description</span><span class="sxs-lookup"><span data-stu-id="503b3-148">description</span></span>|<span data-ttu-id="503b3-149">String</span><span class="sxs-lookup"><span data-stu-id="503b3-149">String</span></span>|<span data-ttu-id="503b3-150">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="503b3-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="503b3-151">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="503b3-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="503b3-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="503b3-152">lastModifiedDateTime</span></span>|<span data-ttu-id="503b3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="503b3-153">DateTimeOffset</span></span>|<span data-ttu-id="503b3-154">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="503b3-154">DateTime the object was last modified.</span></span> <span data-ttu-id="503b3-155">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="503b3-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="503b3-156">displayName</span><span class="sxs-lookup"><span data-stu-id="503b3-156">displayName</span></span>|<span data-ttu-id="503b3-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="503b3-157">String</span></span>|<span data-ttu-id="503b3-158">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="503b3-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="503b3-159">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="503b3-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="503b3-160">version</span><span class="sxs-lookup"><span data-stu-id="503b3-160">version</span></span>|<span data-ttu-id="503b3-161">Int32</span><span class="sxs-lookup"><span data-stu-id="503b3-161">Int32</span></span>|<span data-ttu-id="503b3-162">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="503b3-162">Version of the device configuration.</span></span> <span data-ttu-id="503b3-163">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="503b3-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="503b3-164">packageId</span><span class="sxs-lookup"><span data-stu-id="503b3-164">packageId</span></span>|<span data-ttu-id="503b3-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="503b3-165">String</span></span>|<span data-ttu-id="503b3-166">Android Enterprise App-Konfigurationspaket-ID.</span><span class="sxs-lookup"><span data-stu-id="503b3-166">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="503b3-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="503b3-167">payloadJson</span></span>|<span data-ttu-id="503b3-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="503b3-168">String</span></span>|<span data-ttu-id="503b3-169">JSON-Nutzlast der Android Enterprise-App-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="503b3-169">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="503b3-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="503b3-170">permissionActions</span></span>|<span data-ttu-id="503b3-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="503b3-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="503b3-172">Liste der Android-App-Berechtigungen und entsprechende Berechtigungs Aktionen.</span><span class="sxs-lookup"><span data-stu-id="503b3-172">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="503b3-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="503b3-173">Response</span></span>
<span data-ttu-id="503b3-174">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="503b3-174">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="503b3-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="503b3-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="503b3-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="503b3-176">Request</span></span>
<span data-ttu-id="503b3-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="503b3-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 559

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="503b3-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="503b3-178">Response</span></span>
<span data-ttu-id="503b3-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="503b3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 731

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
  ]
}
```




