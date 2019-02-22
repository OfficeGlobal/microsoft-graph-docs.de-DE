---
title: Abrufen von „iosManagedAppRegistration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs iosManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c950c78e60f87110f335f432a5a1b88c4e166067
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170413"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="135e1-103">Abrufen von „iosManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="135e1-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="135e1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="135e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="135e1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="135e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="135e1-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="135e1-106">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="135e1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="135e1-107">Prerequisites</span></span>
<span data-ttu-id="135e1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="135e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="135e1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="135e1-110">Permission type</span></span>|<span data-ttu-id="135e1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="135e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="135e1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="135e1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="135e1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="135e1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="135e1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="135e1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="135e1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="135e1-115">Not supported.</span></span>|
|<span data-ttu-id="135e1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="135e1-116">Application</span></span>|<span data-ttu-id="135e1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="135e1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="135e1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="135e1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="135e1-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="135e1-119">Optional query parameters</span></span>
<span data-ttu-id="135e1-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="135e1-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="135e1-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="135e1-121">Request headers</span></span>
|<span data-ttu-id="135e1-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="135e1-122">Header</span></span>|<span data-ttu-id="135e1-123">Wert</span><span class="sxs-lookup"><span data-stu-id="135e1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="135e1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="135e1-124">Authorization</span></span>|<span data-ttu-id="135e1-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="135e1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="135e1-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="135e1-126">Accept</span></span>|<span data-ttu-id="135e1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="135e1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="135e1-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="135e1-128">Request body</span></span>
<span data-ttu-id="135e1-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="135e1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="135e1-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="135e1-130">Response</span></span>
<span data-ttu-id="135e1-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="135e1-131">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="135e1-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="135e1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="135e1-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="135e1-133">Request</span></span>
<span data-ttu-id="135e1-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="135e1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="135e1-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="135e1-135">Response</span></span>
<span data-ttu-id="135e1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="135e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1000

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
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
      "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
      "bundleId": "Bundle Id value"
    },
    "id": "47632c19-2c19-4763-192c-6347192c6347",
    "version": "Version value"
  }
}
```




