---
title: Auflisten von „iosManagedAppRegistration“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs iosManagedAppRegistration auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 258becf30b23b02d84318523515c5b7c6d07a13d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419128"
---
# <a name="list-iosmanagedappregistrations"></a><span data-ttu-id="64f15-103">Auflisten von „iosManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="64f15-103">List iosManagedAppRegistrations</span></span>

> <span data-ttu-id="64f15-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="64f15-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="64f15-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64f15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64f15-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="64f15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64f15-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="64f15-107">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64f15-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="64f15-108">Prerequisites</span></span>
<span data-ttu-id="64f15-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="64f15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="64f15-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64f15-111">Permission type</span></span>|<span data-ttu-id="64f15-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64f15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64f15-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64f15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64f15-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64f15-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="64f15-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64f15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64f15-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64f15-116">Not supported.</span></span>|
|<span data-ttu-id="64f15-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64f15-117">Application</span></span>|<span data-ttu-id="64f15-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64f15-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64f15-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64f15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="64f15-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64f15-120">Request headers</span></span>
|<span data-ttu-id="64f15-121">Header</span><span class="sxs-lookup"><span data-stu-id="64f15-121">Header</span></span>|<span data-ttu-id="64f15-122">Wert</span><span class="sxs-lookup"><span data-stu-id="64f15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64f15-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="64f15-123">Authorization</span></span>|<span data-ttu-id="64f15-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="64f15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64f15-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="64f15-125">Accept</span></span>|<span data-ttu-id="64f15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64f15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64f15-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64f15-127">Request body</span></span>
<span data-ttu-id="64f15-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="64f15-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64f15-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="64f15-129">Response</span></span>
<span data-ttu-id="64f15-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="64f15-130">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64f15-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64f15-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="64f15-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64f15-132">Request</span></span>
<span data-ttu-id="64f15-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64f15-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="64f15-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="64f15-134">Response</span></span>
<span data-ttu-id="64f15-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64f15-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1060

{
  "value": [
    {
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
  ]
}
```




