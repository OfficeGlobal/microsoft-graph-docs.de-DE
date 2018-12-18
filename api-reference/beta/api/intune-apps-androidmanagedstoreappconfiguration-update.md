---
title: AndroidManagedStoreAppConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidManagedStoreAppConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: a2643ac3f7ea23b500315a06505f5bb378ee0d58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341258"
---
# <a name="update-androidmanagedstoreappconfiguration"></a><span data-ttu-id="04717-103">AndroidManagedStoreAppConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="04717-103">Update androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="04717-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="04717-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04717-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04717-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04717-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="04717-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04717-107">Aktualisieren Sie die Eigenschaften eines [AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="04717-107">Update the properties of a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04717-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="04717-108">Prerequisites</span></span>
<span data-ttu-id="04717-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04717-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04717-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04717-111">Permission type</span></span>|<span data-ttu-id="04717-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04717-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04717-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04717-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04717-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04717-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04717-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04717-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04717-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04717-116">Not supported.</span></span>|
|<span data-ttu-id="04717-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04717-117">Application</span></span>|<span data-ttu-id="04717-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04717-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04717-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04717-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="04717-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04717-120">Request headers</span></span>
|<span data-ttu-id="04717-121">Header</span><span class="sxs-lookup"><span data-stu-id="04717-121">Header</span></span>|<span data-ttu-id="04717-122">Wert</span><span class="sxs-lookup"><span data-stu-id="04717-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04717-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="04717-123">Authorization</span></span>|<span data-ttu-id="04717-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="04717-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04717-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04717-125">Accept</span></span>|<span data-ttu-id="04717-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04717-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04717-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04717-127">Request body</span></span>
<span data-ttu-id="04717-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="04717-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

<span data-ttu-id="04717-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="04717-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span></span>

|<span data-ttu-id="04717-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04717-130">Property</span></span>|<span data-ttu-id="04717-131">Typ</span><span class="sxs-lookup"><span data-stu-id="04717-131">Type</span></span>|<span data-ttu-id="04717-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04717-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04717-133">id</span><span class="sxs-lookup"><span data-stu-id="04717-133">id</span></span>|<span data-ttu-id="04717-134">String</span><span class="sxs-lookup"><span data-stu-id="04717-134">String</span></span>|<span data-ttu-id="04717-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="04717-135">Key of the entity.</span></span> <span data-ttu-id="04717-136">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04717-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="04717-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="04717-137">targetedMobileApps</span></span>|<span data-ttu-id="04717-138">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="04717-138">String collection</span></span>|<span data-ttu-id="04717-139">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="04717-139">the associated app.</span></span> <span data-ttu-id="04717-140">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04717-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="04717-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="04717-141">roleScopeTagIds</span></span>|<span data-ttu-id="04717-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="04717-142">String collection</span></span>|<span data-ttu-id="04717-143">Liste der Bereich Tags für diese App Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="04717-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="04717-144">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04717-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="04717-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04717-145">createdDateTime</span></span>|<span data-ttu-id="04717-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04717-146">DateTimeOffset</span></span>|<span data-ttu-id="04717-147">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="04717-147">DateTime the object was created.</span></span> <span data-ttu-id="04717-148">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04717-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="04717-149">description</span><span class="sxs-lookup"><span data-stu-id="04717-149">description</span></span>|<span data-ttu-id="04717-150">String</span><span class="sxs-lookup"><span data-stu-id="04717-150">String</span></span>|<span data-ttu-id="04717-151">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="04717-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="04717-152">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04717-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="04717-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04717-153">lastModifiedDateTime</span></span>|<span data-ttu-id="04717-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04717-154">DateTimeOffset</span></span>|<span data-ttu-id="04717-155">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="04717-155">DateTime the object was last modified.</span></span> <span data-ttu-id="04717-156">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04717-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="04717-157">displayName</span><span class="sxs-lookup"><span data-stu-id="04717-157">displayName</span></span>|<span data-ttu-id="04717-158">String</span><span class="sxs-lookup"><span data-stu-id="04717-158">String</span></span>|<span data-ttu-id="04717-159">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="04717-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="04717-160">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04717-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="04717-161">version</span><span class="sxs-lookup"><span data-stu-id="04717-161">version</span></span>|<span data-ttu-id="04717-162">Int32</span><span class="sxs-lookup"><span data-stu-id="04717-162">Int32</span></span>|<span data-ttu-id="04717-163">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="04717-163">Version of the device configuration.</span></span> <span data-ttu-id="04717-164">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04717-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="04717-165">packageId</span><span class="sxs-lookup"><span data-stu-id="04717-165">packageId</span></span>|<span data-ttu-id="04717-166">String</span><span class="sxs-lookup"><span data-stu-id="04717-166">String</span></span>|<span data-ttu-id="04717-167">Android Enterprise app Konfiguration Paket-Id.</span><span class="sxs-lookup"><span data-stu-id="04717-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="04717-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="04717-168">payloadJson</span></span>|<span data-ttu-id="04717-169">String</span><span class="sxs-lookup"><span data-stu-id="04717-169">String</span></span>|<span data-ttu-id="04717-170">Android Enterprise app Konfiguration JSON Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="04717-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="04717-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="04717-171">permissionActions</span></span>|<span data-ttu-id="04717-172">[AndroidPermissionAction](../resources/intune-apps-androidpermissionaction.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="04717-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="04717-173">Liste der Android-app-Berechtigungen und die entsprechenden Berechtigung Aktionen.</span><span class="sxs-lookup"><span data-stu-id="04717-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="04717-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="04717-174">Response</span></span>
<span data-ttu-id="04717-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="04717-175">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04717-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04717-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="04717-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04717-177">Request</span></span>
<span data-ttu-id="04717-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04717-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 549

{
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="04717-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="04717-179">Response</span></span>
<span data-ttu-id="04717-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04717-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





