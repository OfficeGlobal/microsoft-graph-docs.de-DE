---
title: AndroidWorkProfileCustomConfiguration erstellen
description: Erstellen eines neuen androidWorkProfileCustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e3c82610760cd1213373d4284160b3673e46961
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961140"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="33f66-103">AndroidWorkProfileCustomConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="33f66-103">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="33f66-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="33f66-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33f66-105">Erstellen eines neuen [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="33f66-105">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33f66-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="33f66-106">Prerequisites</span></span>
<span data-ttu-id="33f66-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33f66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33f66-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33f66-109">Permission type</span></span>|<span data-ttu-id="33f66-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33f66-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33f66-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33f66-111">Delegated (work or school account)</span></span>|<span data-ttu-id="33f66-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33f66-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33f66-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33f66-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33f66-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33f66-114">Not supported.</span></span>|
|<span data-ttu-id="33f66-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33f66-115">Application</span></span>|<span data-ttu-id="33f66-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33f66-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33f66-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33f66-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="33f66-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33f66-118">Request headers</span></span>
|<span data-ttu-id="33f66-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="33f66-119">Header</span></span>|<span data-ttu-id="33f66-120">Wert</span><span class="sxs-lookup"><span data-stu-id="33f66-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33f66-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="33f66-121">Authorization</span></span>|<span data-ttu-id="33f66-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="33f66-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33f66-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="33f66-123">Accept</span></span>|<span data-ttu-id="33f66-124">application/json</span><span class="sxs-lookup"><span data-stu-id="33f66-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33f66-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33f66-125">Request body</span></span>
<span data-ttu-id="33f66-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidWorkProfileCustomConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="33f66-126">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="33f66-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidWorkProfileCustomConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="33f66-127">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="33f66-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33f66-128">Property</span></span>|<span data-ttu-id="33f66-129">Typ</span><span class="sxs-lookup"><span data-stu-id="33f66-129">Type</span></span>|<span data-ttu-id="33f66-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33f66-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33f66-131">id</span><span class="sxs-lookup"><span data-stu-id="33f66-131">id</span></span>|<span data-ttu-id="33f66-132">String</span><span class="sxs-lookup"><span data-stu-id="33f66-132">String</span></span>|<span data-ttu-id="33f66-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="33f66-133">Key of the entity.</span></span> <span data-ttu-id="33f66-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33f66-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33f66-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33f66-135">lastModifiedDateTime</span></span>|<span data-ttu-id="33f66-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33f66-136">DateTimeOffset</span></span>|<span data-ttu-id="33f66-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33f66-137">DateTime the object was last modified.</span></span> <span data-ttu-id="33f66-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33f66-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33f66-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33f66-139">createdDateTime</span></span>|<span data-ttu-id="33f66-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33f66-140">DateTimeOffset</span></span>|<span data-ttu-id="33f66-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33f66-141">DateTime the object was created.</span></span> <span data-ttu-id="33f66-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33f66-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33f66-143">description</span><span class="sxs-lookup"><span data-stu-id="33f66-143">description</span></span>|<span data-ttu-id="33f66-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33f66-144">String</span></span>|<span data-ttu-id="33f66-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33f66-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33f66-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33f66-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33f66-147">displayName</span><span class="sxs-lookup"><span data-stu-id="33f66-147">displayName</span></span>|<span data-ttu-id="33f66-148">String</span><span class="sxs-lookup"><span data-stu-id="33f66-148">String</span></span>|<span data-ttu-id="33f66-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33f66-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33f66-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33f66-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33f66-151">Version</span><span class="sxs-lookup"><span data-stu-id="33f66-151">version</span></span>|<span data-ttu-id="33f66-152">Int32</span><span class="sxs-lookup"><span data-stu-id="33f66-152">Int32</span></span>|<span data-ttu-id="33f66-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="33f66-153">Version of the device configuration.</span></span> <span data-ttu-id="33f66-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33f66-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33f66-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="33f66-155">omaSettings</span></span>|<span data-ttu-id="33f66-156">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="33f66-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="33f66-157">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="33f66-157">OMA settings.</span></span> <span data-ttu-id="33f66-158">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="33f66-158">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="33f66-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="33f66-159">Response</span></span>
<span data-ttu-id="33f66-160">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="33f66-160">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33f66-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33f66-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="33f66-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33f66-162">Request</span></span>
<span data-ttu-id="33f66-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33f66-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="33f66-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="33f66-164">Response</span></span>
<span data-ttu-id="33f66-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33f66-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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



