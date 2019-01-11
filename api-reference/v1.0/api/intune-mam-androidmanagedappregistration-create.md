---
title: Erstellen von „androidManagedAppRegistration“
description: Diese Methode erstellt ein neues Objekt des Typs androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 84fc753a055e64549b0042d24acedf83827271df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841553"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="22888-103">Erstellen von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="22888-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="22888-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="22888-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22888-105">Diese Methode erstellt ein neues Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-105">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22888-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="22888-106">Prerequisites</span></span>
<span data-ttu-id="22888-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22888-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22888-109">Permission type</span></span>|<span data-ttu-id="22888-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22888-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22888-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22888-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22888-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22888-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22888-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22888-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22888-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22888-114">Not supported.</span></span>|
|<span data-ttu-id="22888-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22888-115">Application</span></span>|<span data-ttu-id="22888-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22888-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22888-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22888-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="22888-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22888-118">Request headers</span></span>
|<span data-ttu-id="22888-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="22888-119">Header</span></span>|<span data-ttu-id="22888-120">Wert</span><span class="sxs-lookup"><span data-stu-id="22888-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22888-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="22888-121">Authorization</span></span>|<span data-ttu-id="22888-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="22888-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22888-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="22888-123">Accept</span></span>|<span data-ttu-id="22888-124">application/json</span><span class="sxs-lookup"><span data-stu-id="22888-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22888-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22888-125">Request body</span></span>
<span data-ttu-id="22888-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidManagedAppRegistration“ an.</span><span class="sxs-lookup"><span data-stu-id="22888-126">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="22888-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidManagedAppRegistration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="22888-127">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="22888-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="22888-128">Property</span></span>|<span data-ttu-id="22888-129">Typ</span><span class="sxs-lookup"><span data-stu-id="22888-129">Type</span></span>|<span data-ttu-id="22888-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22888-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22888-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22888-131">createdDateTime</span></span>|<span data-ttu-id="22888-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22888-132">DateTimeOffset</span></span>|<span data-ttu-id="22888-133">Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-133">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="22888-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="22888-134">lastSyncDateTime</span></span>|<span data-ttu-id="22888-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22888-135">DateTimeOffset</span></span>|<span data-ttu-id="22888-136">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst.</span><span class="sxs-lookup"><span data-stu-id="22888-136">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="22888-137">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-137">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="22888-138">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="22888-138">applicationVersion</span></span>|<span data-ttu-id="22888-139">String</span><span class="sxs-lookup"><span data-stu-id="22888-139">String</span></span>|<span data-ttu-id="22888-140">App-Version. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-140">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="22888-141">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="22888-141">managementSdkVersion</span></span>|<span data-ttu-id="22888-142">String</span><span class="sxs-lookup"><span data-stu-id="22888-142">String</span></span>|<span data-ttu-id="22888-143">Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-143">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="22888-144">platformVersion</span><span class="sxs-lookup"><span data-stu-id="22888-144">platformVersion</span></span>|<span data-ttu-id="22888-145">String</span><span class="sxs-lookup"><span data-stu-id="22888-145">String</span></span>|<span data-ttu-id="22888-146">Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-146">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="22888-147">deviceType</span><span class="sxs-lookup"><span data-stu-id="22888-147">deviceType</span></span>|<span data-ttu-id="22888-148">String</span><span class="sxs-lookup"><span data-stu-id="22888-148">String</span></span>|<span data-ttu-id="22888-149">Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-149">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="22888-150">deviceTag</span><span class="sxs-lookup"><span data-stu-id="22888-150">deviceTag</span></span>|<span data-ttu-id="22888-151">String</span><span class="sxs-lookup"><span data-stu-id="22888-151">String</span></span>|<span data-ttu-id="22888-152">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="22888-152">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="22888-153">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="22888-153">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="22888-154">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-154">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="22888-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="22888-155">deviceName</span></span>|<span data-ttu-id="22888-156">String</span><span class="sxs-lookup"><span data-stu-id="22888-156">String</span></span>|<span data-ttu-id="22888-157">Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-157">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="22888-158">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="22888-158">flaggedReasons</span></span>|<span data-ttu-id="22888-159">[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="22888-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="22888-160">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="22888-160">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="22888-161">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="22888-161">E.g.</span></span> <span data-ttu-id="22888-162">die App auf Stamm Gerät Inherited verlaufende [ManagedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-162">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="22888-163">Mögliche Werte sind: `none` und `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="22888-163">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="22888-164">userId</span><span class="sxs-lookup"><span data-stu-id="22888-164">userId</span></span>|<span data-ttu-id="22888-165">String</span><span class="sxs-lookup"><span data-stu-id="22888-165">String</span></span>|<span data-ttu-id="22888-166">Benutzer-ID, zu der die App-Registrierung gehört.</span><span class="sxs-lookup"><span data-stu-id="22888-166">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="22888-167">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="22888-168">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="22888-168">appIdentifier</span></span>|[<span data-ttu-id="22888-169">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="22888-169">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="22888-170">Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-170">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="22888-171">id</span><span class="sxs-lookup"><span data-stu-id="22888-171">id</span></span>|<span data-ttu-id="22888-172">String</span><span class="sxs-lookup"><span data-stu-id="22888-172">String</span></span>|<span data-ttu-id="22888-173">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="22888-173">Key of the entity.</span></span> <span data-ttu-id="22888-174">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-174">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="22888-175">Version</span><span class="sxs-lookup"><span data-stu-id="22888-175">version</span></span>|<span data-ttu-id="22888-176">String</span><span class="sxs-lookup"><span data-stu-id="22888-176">String</span></span>|<span data-ttu-id="22888-177">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="22888-177">Version of the entity.</span></span> <span data-ttu-id="22888-178">Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="22888-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="22888-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="22888-179">Response</span></span>
<span data-ttu-id="22888-180">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="22888-180">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22888-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22888-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="22888-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22888-182">Request</span></span>
<span data-ttu-id="22888-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22888-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22888-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="22888-184">Response</span></span>
<span data-ttu-id="22888-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22888-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



