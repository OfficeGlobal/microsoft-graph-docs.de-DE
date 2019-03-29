---
title: AndroidForWorkMobileAppConfiguration erstellen
description: Erstellen eines neuen androidForWorkMobileAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 15a8fb8d1b1485eae922bf302dd76fcc786a6fd3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958648"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="58241-103">AndroidForWorkMobileAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="58241-103">Create androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="58241-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58241-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58241-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="58241-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58241-106">Erstellen eines neuen [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="58241-106">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58241-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58241-107">Prerequisites</span></span>
<span data-ttu-id="58241-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58241-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58241-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58241-110">Permission type</span></span>|<span data-ttu-id="58241-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58241-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58241-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58241-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58241-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58241-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="58241-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58241-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58241-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58241-115">Not supported.</span></span>|
|<span data-ttu-id="58241-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58241-116">Application</span></span>|<span data-ttu-id="58241-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58241-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58241-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58241-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="58241-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58241-119">Request headers</span></span>
|<span data-ttu-id="58241-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="58241-120">Header</span></span>|<span data-ttu-id="58241-121">Wert</span><span class="sxs-lookup"><span data-stu-id="58241-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58241-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58241-122">Authorization</span></span>|<span data-ttu-id="58241-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="58241-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58241-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="58241-124">Accept</span></span>|<span data-ttu-id="58241-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58241-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58241-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58241-126">Request body</span></span>
<span data-ttu-id="58241-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidForWorkMobileAppConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="58241-127">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="58241-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidForWorkMobileAppConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="58241-128">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="58241-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58241-129">Property</span></span>|<span data-ttu-id="58241-130">Typ</span><span class="sxs-lookup"><span data-stu-id="58241-130">Type</span></span>|<span data-ttu-id="58241-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58241-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58241-132">id</span><span class="sxs-lookup"><span data-stu-id="58241-132">id</span></span>|<span data-ttu-id="58241-133">String</span><span class="sxs-lookup"><span data-stu-id="58241-133">String</span></span>|<span data-ttu-id="58241-134">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="58241-134">Key of the entity.</span></span> <span data-ttu-id="58241-135">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58241-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="58241-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="58241-136">targetedMobileApps</span></span>|<span data-ttu-id="58241-137">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="58241-137">String collection</span></span>|<span data-ttu-id="58241-138">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="58241-138">the associated app.</span></span> <span data-ttu-id="58241-139">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58241-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="58241-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="58241-140">roleScopeTagIds</span></span>|<span data-ttu-id="58241-141">String collection</span><span class="sxs-lookup"><span data-stu-id="58241-141">String collection</span></span>|<span data-ttu-id="58241-142">Liste der Bereichs Tags für diese APP-Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="58241-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="58241-143">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58241-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="58241-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58241-144">createdDateTime</span></span>|<span data-ttu-id="58241-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58241-145">DateTimeOffset</span></span>|<span data-ttu-id="58241-146">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="58241-146">DateTime the object was created.</span></span> <span data-ttu-id="58241-147">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58241-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="58241-148">description</span><span class="sxs-lookup"><span data-stu-id="58241-148">description</span></span>|<span data-ttu-id="58241-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58241-149">String</span></span>|<span data-ttu-id="58241-150">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="58241-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="58241-151">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58241-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="58241-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58241-152">lastModifiedDateTime</span></span>|<span data-ttu-id="58241-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58241-153">DateTimeOffset</span></span>|<span data-ttu-id="58241-154">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="58241-154">DateTime the object was last modified.</span></span> <span data-ttu-id="58241-155">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58241-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="58241-156">displayName</span><span class="sxs-lookup"><span data-stu-id="58241-156">displayName</span></span>|<span data-ttu-id="58241-157">String</span><span class="sxs-lookup"><span data-stu-id="58241-157">String</span></span>|<span data-ttu-id="58241-158">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="58241-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="58241-159">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58241-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="58241-160">version</span><span class="sxs-lookup"><span data-stu-id="58241-160">version</span></span>|<span data-ttu-id="58241-161">Int32</span><span class="sxs-lookup"><span data-stu-id="58241-161">Int32</span></span>|<span data-ttu-id="58241-162">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="58241-162">Version of the device configuration.</span></span> <span data-ttu-id="58241-163">Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58241-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="58241-164">packageId</span><span class="sxs-lookup"><span data-stu-id="58241-164">packageId</span></span>|<span data-ttu-id="58241-165">String</span><span class="sxs-lookup"><span data-stu-id="58241-165">String</span></span>|<span data-ttu-id="58241-166">Android for Work-App-Konfigurationspaket-ID.</span><span class="sxs-lookup"><span data-stu-id="58241-166">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="58241-167">payloadJson</span><span class="sxs-lookup"><span data-stu-id="58241-167">payloadJson</span></span>|<span data-ttu-id="58241-168">String</span><span class="sxs-lookup"><span data-stu-id="58241-168">String</span></span>|<span data-ttu-id="58241-169">Android for Work-App-Konfiguration JSON-Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="58241-169">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="58241-170">permissionActions</span><span class="sxs-lookup"><span data-stu-id="58241-170">permissionActions</span></span>|<span data-ttu-id="58241-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="58241-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="58241-172">Liste der Android-App-Berechtigungen und entsprechende Berechtigungs Aktionen.</span><span class="sxs-lookup"><span data-stu-id="58241-172">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="58241-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="58241-173">Response</span></span>
<span data-ttu-id="58241-174">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="58241-174">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58241-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58241-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="58241-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58241-176">Request</span></span>
<span data-ttu-id="58241-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58241-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
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

### <a name="response"></a><span data-ttu-id="58241-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="58241-178">Response</span></span>
<span data-ttu-id="58241-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58241-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




