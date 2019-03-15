---
title: Erstellen von „androidManagedAppRegistration“
description: Diese Methode erstellt ein neues Objekt des Typs androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c05ba7fa13577134b148c8af836e3ba453a1e40
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571459"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="04db7-103">Erstellen von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="04db7-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="04db7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04db7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04db7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="04db7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04db7-106">Diese Methode erstellt ein neues Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-106">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04db7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="04db7-107">Prerequisites</span></span>
<span data-ttu-id="04db7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="04db7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04db7-110">Permission type</span></span>|<span data-ttu-id="04db7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04db7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04db7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04db7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04db7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04db7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04db7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04db7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04db7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04db7-115">Not supported.</span></span>|
|<span data-ttu-id="04db7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04db7-116">Application</span></span>|<span data-ttu-id="04db7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04db7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04db7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04db7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="04db7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04db7-119">Request headers</span></span>
|<span data-ttu-id="04db7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="04db7-120">Header</span></span>|<span data-ttu-id="04db7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="04db7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04db7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04db7-122">Authorization</span></span>|<span data-ttu-id="04db7-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="04db7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04db7-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="04db7-124">Accept</span></span>|<span data-ttu-id="04db7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04db7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04db7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04db7-126">Request body</span></span>
<span data-ttu-id="04db7-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidManagedAppRegistration“ an.</span><span class="sxs-lookup"><span data-stu-id="04db7-127">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="04db7-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidManagedAppRegistration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="04db7-128">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="04db7-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04db7-129">Property</span></span>|<span data-ttu-id="04db7-130">Typ</span><span class="sxs-lookup"><span data-stu-id="04db7-130">Type</span></span>|<span data-ttu-id="04db7-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04db7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04db7-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04db7-132">createdDateTime</span></span>|<span data-ttu-id="04db7-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04db7-133">DateTimeOffset</span></span>|<span data-ttu-id="04db7-134">Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-134">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="04db7-135">lastSyncDateTime</span></span>|<span data-ttu-id="04db7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04db7-136">DateTimeOffset</span></span>|<span data-ttu-id="04db7-137">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst.</span><span class="sxs-lookup"><span data-stu-id="04db7-137">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="04db7-138">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-138">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-139">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="04db7-139">applicationVersion</span></span>|<span data-ttu-id="04db7-140">String</span><span class="sxs-lookup"><span data-stu-id="04db7-140">String</span></span>|<span data-ttu-id="04db7-141">App-Version. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-141">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-142">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="04db7-142">managementSdkVersion</span></span>|<span data-ttu-id="04db7-143">String</span><span class="sxs-lookup"><span data-stu-id="04db7-143">String</span></span>|<span data-ttu-id="04db7-144">Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-144">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-145">platformVersion</span><span class="sxs-lookup"><span data-stu-id="04db7-145">platformVersion</span></span>|<span data-ttu-id="04db7-146">String</span><span class="sxs-lookup"><span data-stu-id="04db7-146">String</span></span>|<span data-ttu-id="04db7-147">Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-147">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-148">deviceType</span><span class="sxs-lookup"><span data-stu-id="04db7-148">deviceType</span></span>|<span data-ttu-id="04db7-149">String</span><span class="sxs-lookup"><span data-stu-id="04db7-149">String</span></span>|<span data-ttu-id="04db7-150">Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-150">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-151">deviceTag</span><span class="sxs-lookup"><span data-stu-id="04db7-151">deviceTag</span></span>|<span data-ttu-id="04db7-152">String</span><span class="sxs-lookup"><span data-stu-id="04db7-152">String</span></span>|<span data-ttu-id="04db7-153">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="04db7-153">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="04db7-154">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="04db7-154">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="04db7-155">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-155">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="04db7-156">deviceName</span></span>|<span data-ttu-id="04db7-157">String</span><span class="sxs-lookup"><span data-stu-id="04db7-157">String</span></span>|<span data-ttu-id="04db7-158">Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-158">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-159">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="04db7-159">managedDeviceId</span></span>|<span data-ttu-id="04db7-160">String</span><span class="sxs-lookup"><span data-stu-id="04db7-160">String</span></span>|<span data-ttu-id="04db7-161">Die ID des verwalteten Geräts des Hostgeräts.</span><span class="sxs-lookup"><span data-stu-id="04db7-161">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="04db7-162">Der Wert kann auch dann leer sein, wenn das Host Gerät verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="04db7-162">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="04db7-163">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-163">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-164">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="04db7-164">azureADDeviceId</span></span>|<span data-ttu-id="04db7-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04db7-165">String</span></span>|<span data-ttu-id="04db7-166">Die Azure Active Directory-Geräte-ID des Hostgeräts.</span><span class="sxs-lookup"><span data-stu-id="04db7-166">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="04db7-167">Der Wert kann auch dann leer sein, wenn das Host Gerät Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="04db7-167">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="04db7-168">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-169">deviceModel</span><span class="sxs-lookup"><span data-stu-id="04db7-169">deviceModel</span></span>|<span data-ttu-id="04db7-170">String</span><span class="sxs-lookup"><span data-stu-id="04db7-170">String</span></span>|<span data-ttu-id="04db7-171">Das Gerätemodell für die aktuelle App-Registrierung, geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="04db7-171">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-172">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="04db7-172">deviceManufacturer</span></span>|<span data-ttu-id="04db7-173">String</span><span class="sxs-lookup"><span data-stu-id="04db7-173">String</span></span>|<span data-ttu-id="04db7-174">Der Gerätehersteller für die aktuelle App-Registrierung, geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="04db7-174">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-175">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="04db7-175">flaggedReasons</span></span>|<span data-ttu-id="04db7-176">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="04db7-176">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="04db7-177">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="04db7-177">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="04db7-178">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="04db7-178">E.g.</span></span> <span data-ttu-id="04db7-179">APP, die auf einem von [ManagedAppRegistration](../resources/intune-mam-managedappregistration.md)geerbten Stammgerät läuft.</span><span class="sxs-lookup"><span data-stu-id="04db7-179">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="04db7-180">Mögliche Werte sind: `none`, `rootedDevice`, `androidBootloaderUnlocked` und `androidFactoryRomModified`.</span><span class="sxs-lookup"><span data-stu-id="04db7-180">Possible values are: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span></span>|
|<span data-ttu-id="04db7-181">userId</span><span class="sxs-lookup"><span data-stu-id="04db7-181">userId</span></span>|<span data-ttu-id="04db7-182">String</span><span class="sxs-lookup"><span data-stu-id="04db7-182">String</span></span>|<span data-ttu-id="04db7-183">Benutzer-ID, zu der die App-Registrierung gehört.</span><span class="sxs-lookup"><span data-stu-id="04db7-183">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="04db7-184">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-184">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-185">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="04db7-185">appIdentifier</span></span>|[<span data-ttu-id="04db7-186">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="04db7-186">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="04db7-187">Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-187">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-188">id</span><span class="sxs-lookup"><span data-stu-id="04db7-188">id</span></span>|<span data-ttu-id="04db7-189">String</span><span class="sxs-lookup"><span data-stu-id="04db7-189">String</span></span>|<span data-ttu-id="04db7-190">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="04db7-190">Key of the entity.</span></span> <span data-ttu-id="04db7-191">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-191">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-192">version</span><span class="sxs-lookup"><span data-stu-id="04db7-192">version</span></span>|<span data-ttu-id="04db7-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04db7-193">String</span></span>|<span data-ttu-id="04db7-194">Version der Entität.</span><span class="sxs-lookup"><span data-stu-id="04db7-194">Version of the entity.</span></span> <span data-ttu-id="04db7-195">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="04db7-195">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="04db7-196">patchVersion</span><span class="sxs-lookup"><span data-stu-id="04db7-196">patchVersion</span></span>|<span data-ttu-id="04db7-197">String</span><span class="sxs-lookup"><span data-stu-id="04db7-197">String</span></span>|<span data-ttu-id="04db7-198">Die Patchversion für die aktuelle Android-App-Registrierung</span><span class="sxs-lookup"><span data-stu-id="04db7-198">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="04db7-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="04db7-199">Response</span></span>
<span data-ttu-id="04db7-200">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="04db7-200">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04db7-201">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04db7-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="04db7-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04db7-202">Request</span></span>
<span data-ttu-id="04db7-203">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04db7-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04db7-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="04db7-204">Response</span></span>
<span data-ttu-id="04db7-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04db7-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




