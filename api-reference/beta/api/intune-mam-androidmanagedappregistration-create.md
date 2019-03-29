---
title: Erstellen von „androidManagedAppRegistration“
description: Diese Methode erstellt ein neues Objekt des Typs androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97ff5274358abd9ada2ee14e624e516a74b01d29
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962813"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="d87fe-103">Erstellen von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="d87fe-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="d87fe-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d87fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d87fe-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d87fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d87fe-106">Diese Methode erstellt ein neues Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-106">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d87fe-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d87fe-107">Prerequisites</span></span>
<span data-ttu-id="d87fe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d87fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d87fe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d87fe-110">Permission type</span></span>|<span data-ttu-id="d87fe-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d87fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d87fe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d87fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d87fe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d87fe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d87fe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d87fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d87fe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d87fe-115">Not supported.</span></span>|
|<span data-ttu-id="d87fe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d87fe-116">Application</span></span>|<span data-ttu-id="d87fe-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d87fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d87fe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d87fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="d87fe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d87fe-119">Request headers</span></span>
|<span data-ttu-id="d87fe-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d87fe-120">Header</span></span>|<span data-ttu-id="d87fe-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d87fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d87fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d87fe-122">Authorization</span></span>|<span data-ttu-id="d87fe-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d87fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d87fe-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d87fe-124">Accept</span></span>|<span data-ttu-id="d87fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d87fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d87fe-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d87fe-126">Request body</span></span>
<span data-ttu-id="d87fe-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidManagedAppRegistration“ an.</span><span class="sxs-lookup"><span data-stu-id="d87fe-127">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="d87fe-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidManagedAppRegistration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="d87fe-128">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="d87fe-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d87fe-129">Property</span></span>|<span data-ttu-id="d87fe-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d87fe-130">Type</span></span>|<span data-ttu-id="d87fe-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d87fe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d87fe-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d87fe-132">createdDateTime</span></span>|<span data-ttu-id="d87fe-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d87fe-133">DateTimeOffset</span></span>|<span data-ttu-id="d87fe-134">Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-134">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d87fe-135">lastSyncDateTime</span></span>|<span data-ttu-id="d87fe-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d87fe-136">DateTimeOffset</span></span>|<span data-ttu-id="d87fe-137">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst.</span><span class="sxs-lookup"><span data-stu-id="d87fe-137">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="d87fe-138">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-138">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-139">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="d87fe-139">applicationVersion</span></span>|<span data-ttu-id="d87fe-140">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-140">String</span></span>|<span data-ttu-id="d87fe-141">App-Version. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-141">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-142">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d87fe-142">managementSdkVersion</span></span>|<span data-ttu-id="d87fe-143">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-143">String</span></span>|<span data-ttu-id="d87fe-144">Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-144">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-145">platformVersion</span><span class="sxs-lookup"><span data-stu-id="d87fe-145">platformVersion</span></span>|<span data-ttu-id="d87fe-146">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-146">String</span></span>|<span data-ttu-id="d87fe-147">Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-147">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-148">deviceType</span><span class="sxs-lookup"><span data-stu-id="d87fe-148">deviceType</span></span>|<span data-ttu-id="d87fe-149">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-149">String</span></span>|<span data-ttu-id="d87fe-150">Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-150">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-151">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d87fe-151">deviceTag</span></span>|<span data-ttu-id="d87fe-152">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-152">String</span></span>|<span data-ttu-id="d87fe-153">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="d87fe-153">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="d87fe-154">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="d87fe-154">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="d87fe-155">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-155">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="d87fe-156">deviceName</span></span>|<span data-ttu-id="d87fe-157">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-157">String</span></span>|<span data-ttu-id="d87fe-158">Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-158">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-159">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d87fe-159">managedDeviceId</span></span>|<span data-ttu-id="d87fe-160">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-160">String</span></span>|<span data-ttu-id="d87fe-161">Die ID des verwalteten Geräts des Hostgeräts.</span><span class="sxs-lookup"><span data-stu-id="d87fe-161">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="d87fe-162">Der Wert kann auch dann leer sein, wenn das Host Gerät verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="d87fe-162">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="d87fe-163">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-163">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-164">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="d87fe-164">azureADDeviceId</span></span>|<span data-ttu-id="d87fe-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d87fe-165">String</span></span>|<span data-ttu-id="d87fe-166">Die Azure Active Directory-Geräte-ID des Hostgeräts.</span><span class="sxs-lookup"><span data-stu-id="d87fe-166">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="d87fe-167">Der Wert kann auch dann leer sein, wenn das Host Gerät Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="d87fe-167">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="d87fe-168">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-169">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d87fe-169">deviceModel</span></span>|<span data-ttu-id="d87fe-170">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-170">String</span></span>|<span data-ttu-id="d87fe-171">Das Gerätemodell für die aktuelle App-Registrierung, geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d87fe-171">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-172">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="d87fe-172">deviceManufacturer</span></span>|<span data-ttu-id="d87fe-173">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-173">String</span></span>|<span data-ttu-id="d87fe-174">Der Gerätehersteller für die aktuelle App-Registrierung, geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="d87fe-174">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-175">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="d87fe-175">flaggedReasons</span></span>|<span data-ttu-id="d87fe-176">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d87fe-176">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="d87fe-177">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="d87fe-177">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="d87fe-178">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="d87fe-178">E.g.</span></span> <span data-ttu-id="d87fe-179">APP, die auf einem von [ManagedAppRegistration](../resources/intune-mam-managedappregistration.md)geerbten Stammgerät läuft.</span><span class="sxs-lookup"><span data-stu-id="d87fe-179">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="d87fe-180">Mögliche Werte sind: `none`, `rootedDevice`, `androidBootloaderUnlocked` und `androidFactoryRomModified`.</span><span class="sxs-lookup"><span data-stu-id="d87fe-180">Possible values are: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span></span>|
|<span data-ttu-id="d87fe-181">userId</span><span class="sxs-lookup"><span data-stu-id="d87fe-181">userId</span></span>|<span data-ttu-id="d87fe-182">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-182">String</span></span>|<span data-ttu-id="d87fe-183">Benutzer-ID, zu der die App-Registrierung gehört.</span><span class="sxs-lookup"><span data-stu-id="d87fe-183">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="d87fe-184">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-184">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-185">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d87fe-185">appIdentifier</span></span>|[<span data-ttu-id="d87fe-186">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d87fe-186">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d87fe-187">Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-187">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-188">id</span><span class="sxs-lookup"><span data-stu-id="d87fe-188">id</span></span>|<span data-ttu-id="d87fe-189">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-189">String</span></span>|<span data-ttu-id="d87fe-190">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="d87fe-190">Key of the entity.</span></span> <span data-ttu-id="d87fe-191">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-191">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-192">version</span><span class="sxs-lookup"><span data-stu-id="d87fe-192">version</span></span>|<span data-ttu-id="d87fe-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d87fe-193">String</span></span>|<span data-ttu-id="d87fe-194">Version der Entität.</span><span class="sxs-lookup"><span data-stu-id="d87fe-194">Version of the entity.</span></span> <span data-ttu-id="d87fe-195">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d87fe-195">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="d87fe-196">patchVersion</span><span class="sxs-lookup"><span data-stu-id="d87fe-196">patchVersion</span></span>|<span data-ttu-id="d87fe-197">String</span><span class="sxs-lookup"><span data-stu-id="d87fe-197">String</span></span>|<span data-ttu-id="d87fe-198">Die Patchversion für die aktuelle Android-App-Registrierung</span><span class="sxs-lookup"><span data-stu-id="d87fe-198">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="d87fe-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="d87fe-199">Response</span></span>
<span data-ttu-id="d87fe-200">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d87fe-200">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d87fe-201">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d87fe-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="d87fe-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d87fe-202">Request</span></span>
<span data-ttu-id="d87fe-203">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d87fe-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 879

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```

### <a name="response"></a><span data-ttu-id="d87fe-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="d87fe-204">Response</span></span>
<span data-ttu-id="d87fe-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d87fe-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 987

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```




