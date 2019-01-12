---
title: Erstellen von androidForWorkMobileAppConfiguration
description: Erstellen eines neuen AndroidForWorkMobileAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c512d35d8f37ed19b132641742942ca3c47aad2b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990613"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="b5116-103">Erstellen von androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5116-103">Create androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="b5116-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b5116-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5116-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5116-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5116-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b5116-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5116-107">Erstellen eines neuen [AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5116-107">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5116-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b5116-108">Prerequisites</span></span>
<span data-ttu-id="b5116-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5116-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5116-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5116-111">Permission type</span></span>|<span data-ttu-id="b5116-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5116-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5116-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5116-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5116-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5116-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b5116-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5116-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5116-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5116-116">Not supported.</span></span>|
|<span data-ttu-id="b5116-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5116-117">Application</span></span>|<span data-ttu-id="b5116-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5116-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5116-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5116-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b5116-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5116-120">Request headers</span></span>
|<span data-ttu-id="b5116-121">Header</span><span class="sxs-lookup"><span data-stu-id="b5116-121">Header</span></span>|<span data-ttu-id="b5116-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b5116-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5116-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5116-123">Authorization</span></span>|<span data-ttu-id="b5116-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5116-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5116-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b5116-125">Accept</span></span>|<span data-ttu-id="b5116-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5116-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5116-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5116-127">Request body</span></span>
<span data-ttu-id="b5116-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidForWorkMobileAppConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b5116-128">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="b5116-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidForWorkMobileAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="b5116-129">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="b5116-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5116-130">Property</span></span>|<span data-ttu-id="b5116-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b5116-131">Type</span></span>|<span data-ttu-id="b5116-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5116-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5116-133">id</span><span class="sxs-lookup"><span data-stu-id="b5116-133">id</span></span>|<span data-ttu-id="b5116-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5116-134">String</span></span>|<span data-ttu-id="b5116-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="b5116-135">Key of the entity.</span></span> <span data-ttu-id="b5116-136">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5116-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b5116-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b5116-137">targetedMobileApps</span></span>|<span data-ttu-id="b5116-138">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b5116-138">String collection</span></span>|<span data-ttu-id="b5116-139">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="b5116-139">the associated app.</span></span> <span data-ttu-id="b5116-140">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5116-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b5116-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b5116-141">roleScopeTagIds</span></span>|<span data-ttu-id="b5116-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b5116-142">String collection</span></span>|<span data-ttu-id="b5116-143">Liste der Bereich Tags für diese App Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="b5116-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="b5116-144">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5116-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b5116-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5116-145">createdDateTime</span></span>|<span data-ttu-id="b5116-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5116-146">DateTimeOffset</span></span>|<span data-ttu-id="b5116-147">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5116-147">DateTime the object was created.</span></span> <span data-ttu-id="b5116-148">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5116-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b5116-149">description</span><span class="sxs-lookup"><span data-stu-id="b5116-149">description</span></span>|<span data-ttu-id="b5116-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5116-150">String</span></span>|<span data-ttu-id="b5116-151">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b5116-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b5116-152">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5116-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b5116-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5116-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b5116-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5116-154">DateTimeOffset</span></span>|<span data-ttu-id="b5116-155">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5116-155">DateTime the object was last modified.</span></span> <span data-ttu-id="b5116-156">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5116-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b5116-157">displayName</span><span class="sxs-lookup"><span data-stu-id="b5116-157">displayName</span></span>|<span data-ttu-id="b5116-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5116-158">String</span></span>|<span data-ttu-id="b5116-159">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b5116-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b5116-160">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5116-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b5116-161">version</span><span class="sxs-lookup"><span data-stu-id="b5116-161">version</span></span>|<span data-ttu-id="b5116-162">Int32</span><span class="sxs-lookup"><span data-stu-id="b5116-162">Int32</span></span>|<span data-ttu-id="b5116-163">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b5116-163">Version of the device configuration.</span></span> <span data-ttu-id="b5116-164">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5116-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b5116-165">packageId</span><span class="sxs-lookup"><span data-stu-id="b5116-165">packageId</span></span>|<span data-ttu-id="b5116-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5116-166">String</span></span>|<span data-ttu-id="b5116-167">Für die Arbeit Android-app Konfiguration-Paket-Id.</span><span class="sxs-lookup"><span data-stu-id="b5116-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="b5116-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="b5116-168">payloadJson</span></span>|<span data-ttu-id="b5116-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5116-169">String</span></span>|<span data-ttu-id="b5116-170">Android für Arbeit app Konfiguration JSON-Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="b5116-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="b5116-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="b5116-171">permissionActions</span></span>|<span data-ttu-id="b5116-172">[AndroidPermissionAction](../resources/intune-apps-androidpermissionaction.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b5116-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="b5116-173">Liste der Android-app-Berechtigungen und die entsprechenden Berechtigung Aktionen.</span><span class="sxs-lookup"><span data-stu-id="b5116-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="b5116-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5116-174">Response</span></span>
<span data-ttu-id="b5116-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b5116-175">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5116-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5116-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5116-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5116-177">Request</span></span>
<span data-ttu-id="b5116-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5116-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b5116-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5116-179">Response</span></span>
<span data-ttu-id="b5116-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5116-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





