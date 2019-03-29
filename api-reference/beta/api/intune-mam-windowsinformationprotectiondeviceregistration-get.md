---
title: WindowsInformationProtectionDeviceRegistration abrufen
description: Lesen von Eigenschaften und Beziehungen des windowsInformationProtectionDeviceRegistration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eaf5b789226a1dbdbc3a563278314ada8c472ac6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982798"
---
# <a name="get-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="741b2-103">WindowsInformationProtectionDeviceRegistration abrufen</span><span class="sxs-lookup"><span data-stu-id="741b2-103">Get windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="741b2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="741b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="741b2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="741b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="741b2-106">Lesen von Eigenschaften und Beziehungen des [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="741b2-106">Read properties and relationships of the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="741b2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="741b2-107">Prerequisites</span></span>
<span data-ttu-id="741b2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="741b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="741b2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="741b2-110">Permission type</span></span>|<span data-ttu-id="741b2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="741b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="741b2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="741b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="741b2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="741b2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="741b2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="741b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="741b2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="741b2-115">Not supported.</span></span>|
|<span data-ttu-id="741b2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="741b2-116">Application</span></span>|<span data-ttu-id="741b2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="741b2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="741b2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="741b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="741b2-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="741b2-119">Optional query parameters</span></span>
<span data-ttu-id="741b2-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="741b2-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="741b2-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="741b2-121">Request headers</span></span>
|<span data-ttu-id="741b2-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="741b2-122">Header</span></span>|<span data-ttu-id="741b2-123">Wert</span><span class="sxs-lookup"><span data-stu-id="741b2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="741b2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="741b2-124">Authorization</span></span>|<span data-ttu-id="741b2-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="741b2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="741b2-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="741b2-126">Accept</span></span>|<span data-ttu-id="741b2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="741b2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="741b2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="741b2-128">Request body</span></span>
<span data-ttu-id="741b2-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="741b2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="741b2-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="741b2-130">Response</span></span>
<span data-ttu-id="741b2-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="741b2-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="741b2-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="741b2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="741b2-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="741b2-133">Request</span></span>
<span data-ttu-id="741b2-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="741b2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

### <a name="response"></a><span data-ttu-id="741b2-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="741b2-135">Response</span></span>
<span data-ttu-id="741b2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="741b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
    "id": "dd72e2c8-e2c8-dd72-c8e2-72ddc8e272dd",
    "userId": "User Id value",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceName": "Device Name value",
    "deviceType": "Device Type value",
    "deviceMacAddress": "Device Mac Address value",
    "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
  }
}
```




