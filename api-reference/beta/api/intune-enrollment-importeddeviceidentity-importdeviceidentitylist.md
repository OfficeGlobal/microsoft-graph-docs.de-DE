---
title: importDeviceIdentityList-Aktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 644c5cb2d4c710b796015bf4d1fd005b6b78727d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973271"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="02a16-103">importDeviceIdentityList-Aktion</span><span class="sxs-lookup"><span data-stu-id="02a16-103">importDeviceIdentityList action</span></span>

> <span data-ttu-id="02a16-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02a16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02a16-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="02a16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02a16-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="02a16-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02a16-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="02a16-107">Prerequisites</span></span>
<span data-ttu-id="02a16-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02a16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a16-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02a16-110">Permission type</span></span>|<span data-ttu-id="02a16-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02a16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02a16-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02a16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02a16-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a16-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="02a16-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02a16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02a16-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02a16-115">Not supported.</span></span>|
|<span data-ttu-id="02a16-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02a16-116">Application</span></span>|<span data-ttu-id="02a16-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02a16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02a16-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02a16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="02a16-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02a16-119">Request headers</span></span>
|<span data-ttu-id="02a16-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="02a16-120">Header</span></span>|<span data-ttu-id="02a16-121">Wert</span><span class="sxs-lookup"><span data-stu-id="02a16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02a16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="02a16-122">Authorization</span></span>|<span data-ttu-id="02a16-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="02a16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02a16-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="02a16-124">Accept</span></span>|<span data-ttu-id="02a16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02a16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02a16-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02a16-126">Request body</span></span>
<span data-ttu-id="02a16-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="02a16-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="02a16-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="02a16-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="02a16-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02a16-129">Property</span></span>|<span data-ttu-id="02a16-130">Typ</span><span class="sxs-lookup"><span data-stu-id="02a16-130">Type</span></span>|<span data-ttu-id="02a16-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02a16-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02a16-132">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="02a16-132">importedDeviceIdentities</span></span>|<span data-ttu-id="02a16-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="02a16-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="02a16-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="02a16-134">Not yet documented</span></span>|
|<span data-ttu-id="02a16-135">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="02a16-135">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="02a16-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="02a16-136">Boolean</span></span>|<span data-ttu-id="02a16-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="02a16-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="02a16-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="02a16-138">Response</span></span>
<span data-ttu-id="02a16-139">Bei erfolgreicher Ausführung gibt die Aktion den `200 OK` Antwortcode und eine [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="02a16-139">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02a16-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02a16-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="02a16-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02a16-141">Request</span></span>
<span data-ttu-id="02a16-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02a16-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/importDeviceIdentityList

Content-type: application/json
Content-length: 642

{
  "importedDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="02a16-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="02a16-143">Response</span></span>
<span data-ttu-id="02a16-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02a16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```




