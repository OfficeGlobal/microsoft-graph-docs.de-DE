---
title: AndroidForWorkMobileAppConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidForWorkMobileAppConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aa42c7109d769142113fe6837b3d7db312856e3e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398261"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="f632f-103">AndroidForWorkMobileAppConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f632f-103">Update androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="f632f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f632f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f632f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f632f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f632f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f632f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f632f-107">Aktualisieren Sie die Eigenschaften eines [AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f632f-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f632f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f632f-108">Prerequisites</span></span>
<span data-ttu-id="f632f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f632f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f632f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f632f-111">Permission type</span></span>|<span data-ttu-id="f632f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f632f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f632f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f632f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f632f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f632f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f632f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f632f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f632f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f632f-116">Not supported.</span></span>|
|<span data-ttu-id="f632f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f632f-117">Application</span></span>|<span data-ttu-id="f632f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f632f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f632f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f632f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f632f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f632f-120">Request headers</span></span>
|<span data-ttu-id="f632f-121">Header</span><span class="sxs-lookup"><span data-stu-id="f632f-121">Header</span></span>|<span data-ttu-id="f632f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f632f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f632f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f632f-123">Authorization</span></span>|<span data-ttu-id="f632f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f632f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f632f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f632f-125">Accept</span></span>|<span data-ttu-id="f632f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f632f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f632f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f632f-127">Request body</span></span>
<span data-ttu-id="f632f-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f632f-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="f632f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="f632f-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="f632f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f632f-130">Property</span></span>|<span data-ttu-id="f632f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f632f-131">Type</span></span>|<span data-ttu-id="f632f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f632f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f632f-133">id</span><span class="sxs-lookup"><span data-stu-id="f632f-133">id</span></span>|<span data-ttu-id="f632f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f632f-134">String</span></span>|<span data-ttu-id="f632f-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="f632f-135">Key of the entity.</span></span> <span data-ttu-id="f632f-136">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f632f-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f632f-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="f632f-137">targetedMobileApps</span></span>|<span data-ttu-id="f632f-138">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f632f-138">String collection</span></span>|<span data-ttu-id="f632f-139">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="f632f-139">the associated app.</span></span> <span data-ttu-id="f632f-140">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f632f-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f632f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f632f-141">roleScopeTagIds</span></span>|<span data-ttu-id="f632f-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="f632f-142">String collection</span></span>|<span data-ttu-id="f632f-143">Liste der Bereich Tags für diese App Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="f632f-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="f632f-144">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f632f-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f632f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f632f-145">createdDateTime</span></span>|<span data-ttu-id="f632f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f632f-146">DateTimeOffset</span></span>|<span data-ttu-id="f632f-147">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f632f-147">DateTime the object was created.</span></span> <span data-ttu-id="f632f-148">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f632f-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f632f-149">description</span><span class="sxs-lookup"><span data-stu-id="f632f-149">description</span></span>|<span data-ttu-id="f632f-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f632f-150">String</span></span>|<span data-ttu-id="f632f-151">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f632f-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f632f-152">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f632f-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f632f-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f632f-153">lastModifiedDateTime</span></span>|<span data-ttu-id="f632f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f632f-154">DateTimeOffset</span></span>|<span data-ttu-id="f632f-155">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f632f-155">DateTime the object was last modified.</span></span> <span data-ttu-id="f632f-156">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f632f-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f632f-157">displayName</span><span class="sxs-lookup"><span data-stu-id="f632f-157">displayName</span></span>|<span data-ttu-id="f632f-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f632f-158">String</span></span>|<span data-ttu-id="f632f-159">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f632f-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f632f-160">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f632f-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f632f-161">version</span><span class="sxs-lookup"><span data-stu-id="f632f-161">version</span></span>|<span data-ttu-id="f632f-162">Int32</span><span class="sxs-lookup"><span data-stu-id="f632f-162">Int32</span></span>|<span data-ttu-id="f632f-163">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f632f-163">Version of the device configuration.</span></span> <span data-ttu-id="f632f-164">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f632f-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="f632f-165">packageId</span><span class="sxs-lookup"><span data-stu-id="f632f-165">packageId</span></span>|<span data-ttu-id="f632f-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f632f-166">String</span></span>|<span data-ttu-id="f632f-167">Für die Arbeit Android-app Konfiguration-Paket-Id.</span><span class="sxs-lookup"><span data-stu-id="f632f-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="f632f-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="f632f-168">payloadJson</span></span>|<span data-ttu-id="f632f-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f632f-169">String</span></span>|<span data-ttu-id="f632f-170">Android für Arbeit app Konfiguration JSON-Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="f632f-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="f632f-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="f632f-171">permissionActions</span></span>|<span data-ttu-id="f632f-172">[AndroidPermissionAction](../resources/intune-apps-androidpermissionaction.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f632f-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="f632f-173">Liste der Android-app-Berechtigungen und die entsprechenden Berechtigung Aktionen.</span><span class="sxs-lookup"><span data-stu-id="f632f-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="f632f-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="f632f-174">Response</span></span>
<span data-ttu-id="f632f-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f632f-175">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f632f-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f632f-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="f632f-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f632f-177">Request</span></span>
<span data-ttu-id="f632f-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f632f-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="f632f-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="f632f-179">Response</span></span>
<span data-ttu-id="f632f-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f632f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




