---
title: Erstellen von „androidManagedAppRegistration“
description: Diese Methode erstellt ein neues Objekt des Typs androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e9fccc978437652dc06c2d8003016b514ff214c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252728"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="f2abb-103">Erstellen von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="f2abb-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="f2abb-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f2abb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2abb-105">Diese Methode erstellt ein neues Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-105">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2abb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f2abb-106">Prerequisites</span></span>
<span data-ttu-id="f2abb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f2abb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2abb-109">Permission type</span></span>|<span data-ttu-id="f2abb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2abb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2abb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2abb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2abb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2abb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2abb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2abb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2abb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2abb-114">Not supported.</span></span>|
|<span data-ttu-id="f2abb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2abb-115">Application</span></span>|<span data-ttu-id="f2abb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2abb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2abb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2abb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="f2abb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2abb-118">Request headers</span></span>
|<span data-ttu-id="f2abb-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f2abb-119">Header</span></span>|<span data-ttu-id="f2abb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f2abb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2abb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2abb-121">Authorization</span></span>|<span data-ttu-id="f2abb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f2abb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2abb-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f2abb-123">Accept</span></span>|<span data-ttu-id="f2abb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f2abb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2abb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2abb-125">Request body</span></span>
<span data-ttu-id="f2abb-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidManagedAppRegistration“ an.</span><span class="sxs-lookup"><span data-stu-id="f2abb-126">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="f2abb-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidManagedAppRegistration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="f2abb-127">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="f2abb-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f2abb-128">Property</span></span>|<span data-ttu-id="f2abb-129">Typ</span><span class="sxs-lookup"><span data-stu-id="f2abb-129">Type</span></span>|<span data-ttu-id="f2abb-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2abb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2abb-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2abb-131">createdDateTime</span></span>|<span data-ttu-id="f2abb-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2abb-132">DateTimeOffset</span></span>|<span data-ttu-id="f2abb-133">Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-133">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f2abb-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f2abb-134">lastSyncDateTime</span></span>|<span data-ttu-id="f2abb-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2abb-135">DateTimeOffset</span></span>|<span data-ttu-id="f2abb-136">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst.</span><span class="sxs-lookup"><span data-stu-id="f2abb-136">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="f2abb-137">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-137">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f2abb-138">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="f2abb-138">applicationVersion</span></span>|<span data-ttu-id="f2abb-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f2abb-139">String</span></span>|<span data-ttu-id="f2abb-140">App-Version. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-140">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f2abb-141">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="f2abb-141">managementSdkVersion</span></span>|<span data-ttu-id="f2abb-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f2abb-142">String</span></span>|<span data-ttu-id="f2abb-143">Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-143">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f2abb-144">platformVersion</span><span class="sxs-lookup"><span data-stu-id="f2abb-144">platformVersion</span></span>|<span data-ttu-id="f2abb-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f2abb-145">String</span></span>|<span data-ttu-id="f2abb-146">Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-146">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f2abb-147">deviceType</span><span class="sxs-lookup"><span data-stu-id="f2abb-147">deviceType</span></span>|<span data-ttu-id="f2abb-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f2abb-148">String</span></span>|<span data-ttu-id="f2abb-149">Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-149">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f2abb-150">deviceTag</span><span class="sxs-lookup"><span data-stu-id="f2abb-150">deviceTag</span></span>|<span data-ttu-id="f2abb-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f2abb-151">String</span></span>|<span data-ttu-id="f2abb-152">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="f2abb-152">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="f2abb-153">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="f2abb-153">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="f2abb-154">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-154">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f2abb-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="f2abb-155">deviceName</span></span>|<span data-ttu-id="f2abb-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f2abb-156">String</span></span>|<span data-ttu-id="f2abb-157">Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-157">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f2abb-158">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="f2abb-158">flaggedReasons</span></span>|<span data-ttu-id="f2abb-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="f2abb-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="f2abb-160">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="f2abb-160">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="f2abb-161">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="f2abb-161">E.g.</span></span> <span data-ttu-id="f2abb-162">APP, die auf einem von [ManagedAppRegistration](../resources/intune-mam-managedappregistration.md)geerbten Stammgerät läuft.</span><span class="sxs-lookup"><span data-stu-id="f2abb-162">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="f2abb-163">Mögliche Werte sind: `none` und `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="f2abb-163">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="f2abb-164">userId</span><span class="sxs-lookup"><span data-stu-id="f2abb-164">userId</span></span>|<span data-ttu-id="f2abb-165">String</span><span class="sxs-lookup"><span data-stu-id="f2abb-165">String</span></span>|<span data-ttu-id="f2abb-166">Benutzer-ID, zu der die App-Registrierung gehört.</span><span class="sxs-lookup"><span data-stu-id="f2abb-166">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="f2abb-167">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f2abb-168">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2abb-168">appIdentifier</span></span>|[<span data-ttu-id="f2abb-169">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2abb-169">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="f2abb-170">Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-170">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f2abb-171">id</span><span class="sxs-lookup"><span data-stu-id="f2abb-171">id</span></span>|<span data-ttu-id="f2abb-172">string</span><span class="sxs-lookup"><span data-stu-id="f2abb-172">String</span></span>|<span data-ttu-id="f2abb-173">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f2abb-173">Key of the entity.</span></span> <span data-ttu-id="f2abb-174">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-174">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f2abb-175">Version</span><span class="sxs-lookup"><span data-stu-id="f2abb-175">version</span></span>|<span data-ttu-id="f2abb-176">String</span><span class="sxs-lookup"><span data-stu-id="f2abb-176">String</span></span>|<span data-ttu-id="f2abb-177">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="f2abb-177">Version of the entity.</span></span> <span data-ttu-id="f2abb-178">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f2abb-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f2abb-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2abb-179">Response</span></span>
<span data-ttu-id="f2abb-180">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f2abb-180">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2abb-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2abb-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2abb-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2abb-182">Request</span></span>
<span data-ttu-id="f2abb-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f2abb-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="f2abb-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2abb-184">Response</span></span>
<span data-ttu-id="f2abb-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2abb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

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
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```



