---
title: Abrufen von „managedAppRegistration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9597a651813d341642637cdb7650a205be6c4c53
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959586"
---
# <a name="get-managedappregistration"></a><span data-ttu-id="a3fde-103">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="a3fde-103">Get managedAppRegistration</span></span>

> <span data-ttu-id="a3fde-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a3fde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3fde-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a3fde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3fde-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3fde-106">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3fde-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a3fde-107">Prerequisites</span></span>
<span data-ttu-id="a3fde-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3fde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3fde-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a3fde-110">Permission type</span></span>|<span data-ttu-id="a3fde-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a3fde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3fde-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a3fde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3fde-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3fde-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a3fde-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a3fde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3fde-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3fde-115">Not supported.</span></span>|
|<span data-ttu-id="a3fde-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a3fde-116">Application</span></span>|<span data-ttu-id="a3fde-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3fde-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3fde-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3fde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3fde-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a3fde-119">Optional query parameters</span></span>
<span data-ttu-id="a3fde-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a3fde-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3fde-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a3fde-121">Request headers</span></span>
|<span data-ttu-id="a3fde-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a3fde-122">Header</span></span>|<span data-ttu-id="a3fde-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a3fde-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3fde-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3fde-124">Authorization</span></span>|<span data-ttu-id="a3fde-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a3fde-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3fde-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a3fde-126">Accept</span></span>|<span data-ttu-id="a3fde-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a3fde-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3fde-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a3fde-128">Request body</span></span>
<span data-ttu-id="a3fde-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a3fde-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3fde-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3fde-130">Response</span></span>
<span data-ttu-id="a3fde-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a3fde-131">If successful, this method returns a `200 OK` response code and [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3fde-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a3fde-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3fde-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3fde-133">Request</span></span>
<span data-ttu-id="a3fde-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a3fde-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="a3fde-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3fde-135">Response</span></span>
<span data-ttu-id="a3fde-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3fde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 956

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppRegistration",
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
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "id": "5496aa60-aa60-5496-60aa-965460aa9654",
    "version": "Version value"
  }
}
```




