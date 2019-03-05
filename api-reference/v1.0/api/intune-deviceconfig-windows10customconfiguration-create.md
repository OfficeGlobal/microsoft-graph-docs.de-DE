---
title: Erstellen von „windows10CustomConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windows10CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e8e99a6f6e5bac3e7d03263f2a4646fcc01ee71
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258751"
---
# <a name="create-windows10customconfiguration"></a><span data-ttu-id="857b8-103">Erstellen von „windows10CustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="857b8-103">Create windows10CustomConfiguration</span></span>

> <span data-ttu-id="857b8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="857b8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="857b8-105">Diese Methode erstellt ein neues Objekt des Typs [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="857b8-105">Create a new [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="857b8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="857b8-106">Prerequisites</span></span>
<span data-ttu-id="857b8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="857b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="857b8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="857b8-109">Permission type</span></span>|<span data-ttu-id="857b8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="857b8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="857b8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="857b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="857b8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="857b8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="857b8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="857b8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="857b8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="857b8-114">Not supported.</span></span>|
|<span data-ttu-id="857b8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="857b8-115">Application</span></span>|<span data-ttu-id="857b8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="857b8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="857b8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="857b8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="857b8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="857b8-118">Request headers</span></span>
|<span data-ttu-id="857b8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="857b8-119">Header</span></span>|<span data-ttu-id="857b8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="857b8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="857b8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="857b8-121">Authorization</span></span>|<span data-ttu-id="857b8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="857b8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="857b8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="857b8-123">Accept</span></span>|<span data-ttu-id="857b8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="857b8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="857b8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="857b8-125">Request body</span></span>
<span data-ttu-id="857b8-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10CustomConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="857b8-126">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="857b8-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10CustomConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="857b8-127">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="857b8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="857b8-128">Property</span></span>|<span data-ttu-id="857b8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="857b8-129">Type</span></span>|<span data-ttu-id="857b8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="857b8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="857b8-131">id</span><span class="sxs-lookup"><span data-stu-id="857b8-131">id</span></span>|<span data-ttu-id="857b8-132">string</span><span class="sxs-lookup"><span data-stu-id="857b8-132">String</span></span>|<span data-ttu-id="857b8-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="857b8-133">Key of the entity.</span></span> <span data-ttu-id="857b8-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="857b8-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="857b8-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="857b8-135">lastModifiedDateTime</span></span>|<span data-ttu-id="857b8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="857b8-136">DateTimeOffset</span></span>|<span data-ttu-id="857b8-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="857b8-137">DateTime the object was last modified.</span></span> <span data-ttu-id="857b8-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="857b8-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="857b8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="857b8-139">createdDateTime</span></span>|<span data-ttu-id="857b8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="857b8-140">DateTimeOffset</span></span>|<span data-ttu-id="857b8-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="857b8-141">DateTime the object was created.</span></span> <span data-ttu-id="857b8-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="857b8-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="857b8-143">description</span><span class="sxs-lookup"><span data-stu-id="857b8-143">description</span></span>|<span data-ttu-id="857b8-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="857b8-144">String</span></span>|<span data-ttu-id="857b8-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="857b8-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="857b8-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="857b8-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="857b8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="857b8-147">displayName</span></span>|<span data-ttu-id="857b8-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="857b8-148">String</span></span>|<span data-ttu-id="857b8-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="857b8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="857b8-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="857b8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="857b8-151">Version</span><span class="sxs-lookup"><span data-stu-id="857b8-151">version</span></span>|<span data-ttu-id="857b8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="857b8-152">Int32</span></span>|<span data-ttu-id="857b8-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="857b8-153">Version of the device configuration.</span></span> <span data-ttu-id="857b8-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="857b8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="857b8-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="857b8-155">omaSettings</span></span>|<span data-ttu-id="857b8-156">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="857b8-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="857b8-157">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="857b8-157">OMA settings.</span></span> <span data-ttu-id="857b8-158">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="857b8-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="857b8-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="857b8-159">Response</span></span>
<span data-ttu-id="857b8-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="857b8-160">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="857b8-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="857b8-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="857b8-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="857b8-162">Request</span></span>
<span data-ttu-id="857b8-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="857b8-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="857b8-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="857b8-164">Response</span></span>
<span data-ttu-id="857b8-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="857b8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```



