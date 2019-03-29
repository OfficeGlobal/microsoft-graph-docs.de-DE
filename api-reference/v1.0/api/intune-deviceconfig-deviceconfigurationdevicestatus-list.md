---
title: Auflisten von „deviceConfigurationDeviceStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationDeviceStatus auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0699363257d4733db017aafce251ba531bb321ad
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970415"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="b8b5c-103">Auflisten von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="b8b5c-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="b8b5c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b8b5c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8b5c-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="b8b5c-105">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8b5c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b8b5c-106">Prerequisites</span></span>
<span data-ttu-id="b8b5c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8b5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8b5c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8b5c-109">Permission type</span></span>|<span data-ttu-id="b8b5c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8b5c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8b5c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8b5c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8b5c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8b5c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b8b5c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8b5c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8b5c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8b5c-114">Not supported.</span></span>|
|<span data-ttu-id="b8b5c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8b5c-115">Application</span></span>|<span data-ttu-id="b8b5c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8b5c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8b5c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8b5c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b8b5c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8b5c-118">Request headers</span></span>
|<span data-ttu-id="b8b5c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b8b5c-119">Header</span></span>|<span data-ttu-id="b8b5c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b8b5c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8b5c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8b5c-121">Authorization</span></span>|<span data-ttu-id="b8b5c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b8b5c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8b5c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b8b5c-123">Accept</span></span>|<span data-ttu-id="b8b5c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b8b5c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8b5c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8b5c-125">Request body</span></span>
<span data-ttu-id="b8b5c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b8b5c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8b5c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8b5c-127">Response</span></span>
<span data-ttu-id="b8b5c-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b8b5c-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8b5c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8b5c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8b5c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8b5c-130">Request</span></span>
<span data-ttu-id="b8b5c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8b5c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="b8b5c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8b5c-132">Response</span></span>
<span data-ttu-id="b8b5c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8b5c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
      "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



