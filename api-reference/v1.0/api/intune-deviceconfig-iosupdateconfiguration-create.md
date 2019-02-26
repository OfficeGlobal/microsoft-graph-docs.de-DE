---
title: iosUpdateConfiguration erstellen
description: Erstellen eines neuen iosUpdateConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1aa18553c42faa75dfc392f84eb137ce03e216e3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258387"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="48185-103">iosUpdateConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="48185-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="48185-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="48185-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48185-105">Erstellen eines neuen [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="48185-105">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48185-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="48185-106">Prerequisites</span></span>
<span data-ttu-id="48185-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="48185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48185-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48185-109">Permission type</span></span>|<span data-ttu-id="48185-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48185-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48185-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48185-111">Delegated (work or school account)</span></span>|<span data-ttu-id="48185-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48185-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48185-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48185-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48185-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48185-114">Not supported.</span></span>|
|<span data-ttu-id="48185-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48185-115">Application</span></span>|<span data-ttu-id="48185-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48185-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48185-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48185-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="48185-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48185-118">Request headers</span></span>
|<span data-ttu-id="48185-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="48185-119">Header</span></span>|<span data-ttu-id="48185-120">Wert</span><span class="sxs-lookup"><span data-stu-id="48185-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48185-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="48185-121">Authorization</span></span>|<span data-ttu-id="48185-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="48185-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48185-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="48185-123">Accept</span></span>|<span data-ttu-id="48185-124">application/json</span><span class="sxs-lookup"><span data-stu-id="48185-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48185-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48185-125">Request body</span></span>
<span data-ttu-id="48185-126">Geben Sie im Anforderungstext eine JSON-Darstellung des iosUpdateConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="48185-126">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="48185-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des iosUpdateConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="48185-127">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="48185-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="48185-128">Property</span></span>|<span data-ttu-id="48185-129">Typ</span><span class="sxs-lookup"><span data-stu-id="48185-129">Type</span></span>|<span data-ttu-id="48185-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48185-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48185-131">id</span><span class="sxs-lookup"><span data-stu-id="48185-131">id</span></span>|<span data-ttu-id="48185-132">string</span><span class="sxs-lookup"><span data-stu-id="48185-132">String</span></span>|<span data-ttu-id="48185-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="48185-133">Key of the entity.</span></span> <span data-ttu-id="48185-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48185-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48185-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48185-135">lastModifiedDateTime</span></span>|<span data-ttu-id="48185-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48185-136">DateTimeOffset</span></span>|<span data-ttu-id="48185-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="48185-137">DateTime the object was last modified.</span></span> <span data-ttu-id="48185-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48185-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48185-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48185-139">createdDateTime</span></span>|<span data-ttu-id="48185-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48185-140">DateTimeOffset</span></span>|<span data-ttu-id="48185-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="48185-141">DateTime the object was created.</span></span> <span data-ttu-id="48185-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48185-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48185-143">description</span><span class="sxs-lookup"><span data-stu-id="48185-143">description</span></span>|<span data-ttu-id="48185-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48185-144">String</span></span>|<span data-ttu-id="48185-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="48185-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="48185-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48185-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48185-147">displayName</span><span class="sxs-lookup"><span data-stu-id="48185-147">displayName</span></span>|<span data-ttu-id="48185-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48185-148">String</span></span>|<span data-ttu-id="48185-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="48185-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="48185-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48185-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48185-151">Version</span><span class="sxs-lookup"><span data-stu-id="48185-151">version</span></span>|<span data-ttu-id="48185-152">Int32</span><span class="sxs-lookup"><span data-stu-id="48185-152">Int32</span></span>|<span data-ttu-id="48185-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="48185-153">Version of the device configuration.</span></span> <span data-ttu-id="48185-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48185-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48185-155">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="48185-155">activeHoursStart</span></span>|<span data-ttu-id="48185-156">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="48185-156">TimeOfDay</span></span>|<span data-ttu-id="48185-157">Beginn der aktiven Stunden (Als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Updates installiert werden sollen.)</span><span class="sxs-lookup"><span data-stu-id="48185-157">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="48185-158">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="48185-158">activeHoursEnd</span></span>|<span data-ttu-id="48185-159">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="48185-159">TimeOfDay</span></span>|<span data-ttu-id="48185-160">Ende der aktiven Stunden (Als aktive Stunden wird das Zeitfenster bezeichnet, in dem keine Updates installiert werden sollen.)</span><span class="sxs-lookup"><span data-stu-id="48185-160">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="48185-161">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="48185-161">scheduledInstallDays</span></span>|<span data-ttu-id="48185-162">[DayOfWeek](../resources/intune-deviceconfig-dayofweek.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="48185-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="48185-163">Tage in der Woche, für die aktive Stunden konfiguriert sind.</span><span class="sxs-lookup"><span data-stu-id="48185-163">Days in week for which active hours are configured.</span></span> <span data-ttu-id="48185-164">Diese Sammlung darf maximal 7 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="48185-164">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="48185-165">Mögliche Werte sind: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday` und `saturday`.</span><span class="sxs-lookup"><span data-stu-id="48185-165">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="48185-166">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="48185-166">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="48185-167">Int32</span><span class="sxs-lookup"><span data-stu-id="48185-167">Int32</span></span>|<span data-ttu-id="48185-168">UTC-Zeitversatz in Minuten</span><span class="sxs-lookup"><span data-stu-id="48185-168">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="48185-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="48185-169">Response</span></span>
<span data-ttu-id="48185-170">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48185-170">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48185-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48185-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="48185-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48185-172">Request</span></span>
<span data-ttu-id="48185-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48185-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```

### <a name="response"></a><span data-ttu-id="48185-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="48185-174">Response</span></span>
<span data-ttu-id="48185-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48185-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```



