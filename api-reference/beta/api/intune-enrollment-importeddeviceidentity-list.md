---
title: ImportedDeviceIdentities aufListen
description: AufListen von Eigenschaften und Beziehungen der importedDeviceIdentity-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 995769e609ff1b999b65a074106d0ac5472e948d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988945"
---
# <a name="list-importeddeviceidentities"></a><span data-ttu-id="1bebb-103">ImportedDeviceIdentities aufListen</span><span class="sxs-lookup"><span data-stu-id="1bebb-103">List importedDeviceIdentities</span></span>

> <span data-ttu-id="1bebb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1bebb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bebb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1bebb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bebb-106">AufListen von Eigenschaften und Beziehungen der [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="1bebb-106">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bebb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1bebb-107">Prerequisites</span></span>
<span data-ttu-id="1bebb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bebb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bebb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1bebb-110">Permission type</span></span>|<span data-ttu-id="1bebb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1bebb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bebb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1bebb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1bebb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bebb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1bebb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1bebb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bebb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1bebb-115">Not supported.</span></span>|
|<span data-ttu-id="1bebb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1bebb-116">Application</span></span>|<span data-ttu-id="1bebb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1bebb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bebb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bebb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="1bebb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1bebb-119">Request headers</span></span>
|<span data-ttu-id="1bebb-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1bebb-120">Header</span></span>|<span data-ttu-id="1bebb-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1bebb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bebb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bebb-122">Authorization</span></span>|<span data-ttu-id="1bebb-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1bebb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bebb-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1bebb-124">Accept</span></span>|<span data-ttu-id="1bebb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1bebb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bebb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1bebb-126">Request body</span></span>
<span data-ttu-id="1bebb-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1bebb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bebb-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="1bebb-128">Response</span></span>
<span data-ttu-id="1bebb-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1bebb-129">If successful, this method returns a `200 OK` response code and a collection of [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bebb-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1bebb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bebb-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bebb-131">Request</span></span>
<span data-ttu-id="1bebb-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1bebb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="1bebb-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1bebb-133">Response</span></span>
<span data-ttu-id="1bebb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1bebb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "value": [
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
  ]
}
```




