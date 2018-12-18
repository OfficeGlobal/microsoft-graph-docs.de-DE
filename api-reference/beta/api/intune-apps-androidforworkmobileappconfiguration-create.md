---
title: Erstellen von androidForWorkMobileAppConfiguration
description: Erstellen eines neuen AndroidForWorkMobileAppConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 25f6f82c04ddd1f2d451a5e16769f48d3e48799c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308834"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="480f8-103">Erstellen von androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="480f8-103">Create androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="480f8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="480f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="480f8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="480f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="480f8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="480f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="480f8-107">Erstellen eines neuen [AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="480f8-107">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="480f8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="480f8-108">Prerequisites</span></span>
<span data-ttu-id="480f8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="480f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="480f8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="480f8-111">Permission type</span></span>|<span data-ttu-id="480f8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="480f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="480f8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="480f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="480f8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="480f8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="480f8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="480f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="480f8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="480f8-116">Not supported.</span></span>|
|<span data-ttu-id="480f8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="480f8-117">Application</span></span>|<span data-ttu-id="480f8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="480f8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="480f8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="480f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="480f8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="480f8-120">Request headers</span></span>
|<span data-ttu-id="480f8-121">Header</span><span class="sxs-lookup"><span data-stu-id="480f8-121">Header</span></span>|<span data-ttu-id="480f8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="480f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="480f8-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="480f8-123">Authorization</span></span>|<span data-ttu-id="480f8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="480f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="480f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="480f8-125">Accept</span></span>|<span data-ttu-id="480f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="480f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="480f8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="480f8-127">Request body</span></span>
<span data-ttu-id="480f8-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidForWorkMobileAppConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="480f8-128">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="480f8-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidForWorkMobileAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="480f8-129">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="480f8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="480f8-130">Property</span></span>|<span data-ttu-id="480f8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="480f8-131">Type</span></span>|<span data-ttu-id="480f8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="480f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="480f8-133">id</span><span class="sxs-lookup"><span data-stu-id="480f8-133">id</span></span>|<span data-ttu-id="480f8-134">String</span><span class="sxs-lookup"><span data-stu-id="480f8-134">String</span></span>|<span data-ttu-id="480f8-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="480f8-135">Key of the entity.</span></span> <span data-ttu-id="480f8-136">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="480f8-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="480f8-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="480f8-137">targetedMobileApps</span></span>|<span data-ttu-id="480f8-138">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="480f8-138">String collection</span></span>|<span data-ttu-id="480f8-139">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="480f8-139">the associated app.</span></span> <span data-ttu-id="480f8-140">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="480f8-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="480f8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="480f8-141">roleScopeTagIds</span></span>|<span data-ttu-id="480f8-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="480f8-142">String collection</span></span>|<span data-ttu-id="480f8-143">Liste der Bereich Tags für diese App Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="480f8-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="480f8-144">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="480f8-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="480f8-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="480f8-145">createdDateTime</span></span>|<span data-ttu-id="480f8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="480f8-146">DateTimeOffset</span></span>|<span data-ttu-id="480f8-147">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="480f8-147">DateTime the object was created.</span></span> <span data-ttu-id="480f8-148">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="480f8-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="480f8-149">description</span><span class="sxs-lookup"><span data-stu-id="480f8-149">description</span></span>|<span data-ttu-id="480f8-150">String</span><span class="sxs-lookup"><span data-stu-id="480f8-150">String</span></span>|<span data-ttu-id="480f8-151">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="480f8-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="480f8-152">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="480f8-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="480f8-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="480f8-153">lastModifiedDateTime</span></span>|<span data-ttu-id="480f8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="480f8-154">DateTimeOffset</span></span>|<span data-ttu-id="480f8-155">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="480f8-155">DateTime the object was last modified.</span></span> <span data-ttu-id="480f8-156">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="480f8-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="480f8-157">displayName</span><span class="sxs-lookup"><span data-stu-id="480f8-157">displayName</span></span>|<span data-ttu-id="480f8-158">String</span><span class="sxs-lookup"><span data-stu-id="480f8-158">String</span></span>|<span data-ttu-id="480f8-159">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="480f8-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="480f8-160">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="480f8-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="480f8-161">version</span><span class="sxs-lookup"><span data-stu-id="480f8-161">version</span></span>|<span data-ttu-id="480f8-162">Int32</span><span class="sxs-lookup"><span data-stu-id="480f8-162">Int32</span></span>|<span data-ttu-id="480f8-163">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="480f8-163">Version of the device configuration.</span></span> <span data-ttu-id="480f8-164">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="480f8-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="480f8-165">packageId</span><span class="sxs-lookup"><span data-stu-id="480f8-165">packageId</span></span>|<span data-ttu-id="480f8-166">String</span><span class="sxs-lookup"><span data-stu-id="480f8-166">String</span></span>|<span data-ttu-id="480f8-167">Für die Arbeit Android-app Konfiguration-Paket-Id.</span><span class="sxs-lookup"><span data-stu-id="480f8-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="480f8-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="480f8-168">payloadJson</span></span>|<span data-ttu-id="480f8-169">String</span><span class="sxs-lookup"><span data-stu-id="480f8-169">String</span></span>|<span data-ttu-id="480f8-170">Android für Arbeit app Konfiguration JSON-Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="480f8-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="480f8-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="480f8-171">permissionActions</span></span>|<span data-ttu-id="480f8-172">[AndroidPermissionAction](../resources/intune-apps-androidpermissionaction.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="480f8-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="480f8-173">Liste der Android-app-Berechtigungen und die entsprechenden Berechtigung Aktionen.</span><span class="sxs-lookup"><span data-stu-id="480f8-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="480f8-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="480f8-174">Response</span></span>
<span data-ttu-id="480f8-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="480f8-175">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="480f8-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="480f8-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="480f8-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="480f8-177">Request</span></span>
<span data-ttu-id="480f8-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="480f8-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 624

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="480f8-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="480f8-179">Response</span></span>
<span data-ttu-id="480f8-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="480f8-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 732

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
  "id": "6204ae6d-ae6d-6204-6dae-04626dae0462",
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





