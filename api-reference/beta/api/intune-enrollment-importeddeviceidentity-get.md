---
title: ImportedDeviceIdentity abrufen
description: Lesen von Eigenschaften und Beziehungen des importedDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8bac93ae04a5a8e7b2a0edb280a9c6ca79a09394
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141048"
---
# <a name="get-importeddeviceidentity"></a><span data-ttu-id="dd051-103">ImportedDeviceIdentity abrufen</span><span class="sxs-lookup"><span data-stu-id="dd051-103">Get importedDeviceIdentity</span></span>

> <span data-ttu-id="dd051-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd051-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd051-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dd051-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd051-106">Lesen von Eigenschaften und Beziehungen des [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd051-106">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd051-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dd051-107">Prerequisites</span></span>
<span data-ttu-id="dd051-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd051-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dd051-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd051-110">Permission type</span></span>|<span data-ttu-id="dd051-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd051-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd051-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd051-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd051-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd051-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dd051-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd051-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd051-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd051-115">Not supported.</span></span>|
|<span data-ttu-id="dd051-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd051-116">Application</span></span>|<span data-ttu-id="dd051-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd051-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd051-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd051-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd051-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="dd051-119">Optional query parameters</span></span>
<span data-ttu-id="dd051-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dd051-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd051-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd051-121">Request headers</span></span>
|<span data-ttu-id="dd051-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dd051-122">Header</span></span>|<span data-ttu-id="dd051-123">Wert</span><span class="sxs-lookup"><span data-stu-id="dd051-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd051-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd051-124">Authorization</span></span>|<span data-ttu-id="dd051-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dd051-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd051-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dd051-126">Accept</span></span>|<span data-ttu-id="dd051-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dd051-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd051-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd051-128">Request body</span></span>
<span data-ttu-id="dd051-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dd051-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd051-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd051-130">Response</span></span>
<span data-ttu-id="dd051-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dd051-131">If successful, this method returns a `200 OK` response code and [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd051-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd051-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd051-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd051-133">Request</span></span>
<span data-ttu-id="dd051-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd051-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="dd051-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd051-135">Response</span></span>
<span data-ttu-id="dd051-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd051-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "value": {
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
}
```




