---
title: Erstellen von androidManagedStoreAppConfiguration
description: Erstellen eines neuen AndroidManagedStoreAppConfiguration-Objekts.
ms.openlocfilehash: 2a9d9e7e9927f84999f018ce53dcad8c896554ba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060572"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="cf6cb-103">Erstellen von androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf6cb-103">Create androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="cf6cb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf6cb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf6cb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf6cb-107">Erstellen eines neuen [AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-107">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf6cb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cf6cb-108">Prerequisites</span></span>
<span data-ttu-id="cf6cb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf6cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf6cb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf6cb-111">Permission type</span></span>|<span data-ttu-id="cf6cb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf6cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf6cb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf6cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf6cb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf6cb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cf6cb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf6cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf6cb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf6cb-116">Not supported.</span></span>|
|<span data-ttu-id="cf6cb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf6cb-117">Application</span></span>|<span data-ttu-id="cf6cb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf6cb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf6cb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf6cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cf6cb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf6cb-120">Request headers</span></span>
|<span data-ttu-id="cf6cb-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cf6cb-121">Header</span></span>|<span data-ttu-id="cf6cb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cf6cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf6cb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf6cb-123">Authorization</span></span>|<span data-ttu-id="cf6cb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cf6cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf6cb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf6cb-125">Accept</span></span>|<span data-ttu-id="cf6cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf6cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf6cb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf6cb-127">Request body</span></span>
<span data-ttu-id="cf6cb-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidManagedStoreAppConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="cf6cb-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidManagedStoreAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="cf6cb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cf6cb-130">Property</span></span>|<span data-ttu-id="cf6cb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="cf6cb-131">Type</span></span>|<span data-ttu-id="cf6cb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf6cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf6cb-133">id</span><span class="sxs-lookup"><span data-stu-id="cf6cb-133">id</span></span>|<span data-ttu-id="cf6cb-134">String</span><span class="sxs-lookup"><span data-stu-id="cf6cb-134">String</span></span>|<span data-ttu-id="cf6cb-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-135">Key of the entity.</span></span> <span data-ttu-id="cf6cb-136">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf6cb-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cf6cb-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="cf6cb-137">targetedMobileApps</span></span>|<span data-ttu-id="cf6cb-138">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cf6cb-138">String collection</span></span>|<span data-ttu-id="cf6cb-139">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-139">the associated app.</span></span> <span data-ttu-id="cf6cb-140">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf6cb-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cf6cb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cf6cb-141">roleScopeTagIds</span></span>|<span data-ttu-id="cf6cb-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="cf6cb-142">String collection</span></span>|<span data-ttu-id="cf6cb-143">Liste der Bereich Tags für diese App Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="cf6cb-144">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf6cb-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cf6cb-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf6cb-145">createdDateTime</span></span>|<span data-ttu-id="cf6cb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf6cb-146">DateTimeOffset</span></span>|<span data-ttu-id="cf6cb-147">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-147">DateTime the object was created.</span></span> <span data-ttu-id="cf6cb-148">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf6cb-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cf6cb-149">description</span><span class="sxs-lookup"><span data-stu-id="cf6cb-149">description</span></span>|<span data-ttu-id="cf6cb-150">String</span><span class="sxs-lookup"><span data-stu-id="cf6cb-150">String</span></span>|<span data-ttu-id="cf6cb-151">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cf6cb-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cf6cb-152">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf6cb-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cf6cb-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf6cb-153">lastModifiedDateTime</span></span>|<span data-ttu-id="cf6cb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf6cb-154">DateTimeOffset</span></span>|<span data-ttu-id="cf6cb-155">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-155">DateTime the object was last modified.</span></span> <span data-ttu-id="cf6cb-156">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf6cb-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cf6cb-157">displayName</span><span class="sxs-lookup"><span data-stu-id="cf6cb-157">displayName</span></span>|<span data-ttu-id="cf6cb-158">String</span><span class="sxs-lookup"><span data-stu-id="cf6cb-158">String</span></span>|<span data-ttu-id="cf6cb-159">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cf6cb-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cf6cb-160">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf6cb-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cf6cb-161">version</span><span class="sxs-lookup"><span data-stu-id="cf6cb-161">version</span></span>|<span data-ttu-id="cf6cb-162">Int32</span><span class="sxs-lookup"><span data-stu-id="cf6cb-162">Int32</span></span>|<span data-ttu-id="cf6cb-163">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-163">Version of the device configuration.</span></span> <span data-ttu-id="cf6cb-164">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf6cb-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="cf6cb-165">packageId</span><span class="sxs-lookup"><span data-stu-id="cf6cb-165">packageId</span></span>|<span data-ttu-id="cf6cb-166">String</span><span class="sxs-lookup"><span data-stu-id="cf6cb-166">String</span></span>|<span data-ttu-id="cf6cb-167">Android Enterprise app Konfiguration Paket-Id.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="cf6cb-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="cf6cb-168">payloadJson</span></span>|<span data-ttu-id="cf6cb-169">String</span><span class="sxs-lookup"><span data-stu-id="cf6cb-169">String</span></span>|<span data-ttu-id="cf6cb-170">Android Enterprise app Konfiguration JSON Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="cf6cb-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="cf6cb-171">permissionActions</span></span>|<span data-ttu-id="cf6cb-172">[AndroidPermissionAction](../resources/intune-apps-androidpermissionaction.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="cf6cb-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="cf6cb-173">Liste der Android-app-Berechtigungen und die entsprechenden Berechtigung Aktionen.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="cf6cb-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf6cb-174">Response</span></span>
<span data-ttu-id="cf6cb-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-175">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf6cb-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf6cb-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf6cb-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf6cb-177">Request</span></span>
<span data-ttu-id="cf6cb-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 623

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="cf6cb-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf6cb-179">Response</span></span>
<span data-ttu-id="cf6cb-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf6cb-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





