---
title: Erstellen von „windowsPhone81CustomConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65e9f8dfd631fed0fb8ae3d8cf5c232ec83ab4f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932420"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="0e6bf-103">Erstellen von „windowsPhone81CustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="0e6bf-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="0e6bf-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0e6bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e6bf-105">Diese Methode erstellt ein neues Objekt des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e6bf-105">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e6bf-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0e6bf-106">Prerequisites</span></span>
<span data-ttu-id="0e6bf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e6bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e6bf-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e6bf-109">Permission type</span></span>|<span data-ttu-id="0e6bf-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e6bf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e6bf-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e6bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e6bf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e6bf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e6bf-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e6bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e6bf-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e6bf-114">Not supported.</span></span>|
|<span data-ttu-id="0e6bf-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e6bf-115">Application</span></span>|<span data-ttu-id="0e6bf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e6bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e6bf-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e6bf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0e6bf-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e6bf-118">Request headers</span></span>
|<span data-ttu-id="0e6bf-119">Header</span><span class="sxs-lookup"><span data-stu-id="0e6bf-119">Header</span></span>|<span data-ttu-id="0e6bf-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0e6bf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e6bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e6bf-121">Authorization</span></span>|<span data-ttu-id="0e6bf-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0e6bf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e6bf-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0e6bf-123">Accept</span></span>|<span data-ttu-id="0e6bf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0e6bf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e6bf-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e6bf-125">Request body</span></span>
<span data-ttu-id="0e6bf-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsPhone81CustomConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="0e6bf-126">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="0e6bf-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsPhone81CustomConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="0e6bf-127">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="0e6bf-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e6bf-128">Property</span></span>|<span data-ttu-id="0e6bf-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0e6bf-129">Type</span></span>|<span data-ttu-id="0e6bf-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e6bf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e6bf-131">id</span><span class="sxs-lookup"><span data-stu-id="0e6bf-131">id</span></span>|<span data-ttu-id="0e6bf-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e6bf-132">String</span></span>|<span data-ttu-id="0e6bf-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0e6bf-133">Key of the entity.</span></span> <span data-ttu-id="0e6bf-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e6bf-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e6bf-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e6bf-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0e6bf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e6bf-136">DateTimeOffset</span></span>|<span data-ttu-id="0e6bf-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e6bf-137">DateTime the object was last modified.</span></span> <span data-ttu-id="0e6bf-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e6bf-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e6bf-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e6bf-139">createdDateTime</span></span>|<span data-ttu-id="0e6bf-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e6bf-140">DateTimeOffset</span></span>|<span data-ttu-id="0e6bf-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e6bf-141">DateTime the object was created.</span></span> <span data-ttu-id="0e6bf-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e6bf-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e6bf-143">description</span><span class="sxs-lookup"><span data-stu-id="0e6bf-143">description</span></span>|<span data-ttu-id="0e6bf-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e6bf-144">String</span></span>|<span data-ttu-id="0e6bf-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0e6bf-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0e6bf-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e6bf-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e6bf-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0e6bf-147">displayName</span></span>|<span data-ttu-id="0e6bf-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e6bf-148">String</span></span>|<span data-ttu-id="0e6bf-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0e6bf-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0e6bf-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e6bf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e6bf-151">Version</span><span class="sxs-lookup"><span data-stu-id="0e6bf-151">version</span></span>|<span data-ttu-id="0e6bf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0e6bf-152">Int32</span></span>|<span data-ttu-id="0e6bf-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0e6bf-153">Version of the device configuration.</span></span> <span data-ttu-id="0e6bf-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e6bf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e6bf-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="0e6bf-155">omaSettings</span></span>|<span data-ttu-id="0e6bf-156">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e6bf-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="0e6bf-157">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="0e6bf-157">OMA settings.</span></span> <span data-ttu-id="0e6bf-158">Diese Sammlung kann bis zu 1000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="0e6bf-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0e6bf-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e6bf-159">Response</span></span>
<span data-ttu-id="0e6bf-160">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0e6bf-160">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e6bf-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e6bf-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e6bf-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e6bf-162">Request</span></span>
<span data-ttu-id="0e6bf-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e6bf-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="0e6bf-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e6bf-164">Response</span></span>
<span data-ttu-id="0e6bf-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e6bf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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



