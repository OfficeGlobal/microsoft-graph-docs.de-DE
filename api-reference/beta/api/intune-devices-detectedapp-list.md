---
title: Auflisten von „detectedApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs detectedApp auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7b042a954aaae4871d88ba4d07f97a97e4684924
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414655"
---
# <a name="list-detectedapps"></a><span data-ttu-id="0f399-103">Auflisten von „detectedApp“</span><span class="sxs-lookup"><span data-stu-id="0f399-103">List detectedApps</span></span>

> <span data-ttu-id="0f399-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0f399-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f399-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f399-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f399-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f399-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f399-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [detectedApp](../resources/intune-devices-detectedapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="0f399-107">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f399-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0f399-108">Prerequisites</span></span>
<span data-ttu-id="0f399-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f399-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0f399-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f399-111">Permission type</span></span>|<span data-ttu-id="0f399-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f399-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f399-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f399-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f399-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f399-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0f399-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f399-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f399-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f399-116">Not supported.</span></span>|
|<span data-ttu-id="0f399-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f399-117">Application</span></span>|<span data-ttu-id="0f399-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f399-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f399-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f399-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="0f399-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f399-120">Request headers</span></span>
|<span data-ttu-id="0f399-121">Header</span><span class="sxs-lookup"><span data-stu-id="0f399-121">Header</span></span>|<span data-ttu-id="0f399-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0f399-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f399-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0f399-123">Authorization</span></span>|<span data-ttu-id="0f399-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0f399-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f399-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0f399-125">Accept</span></span>|<span data-ttu-id="0f399-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f399-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f399-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f399-127">Request body</span></span>
<span data-ttu-id="0f399-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0f399-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f399-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f399-129">Response</span></span>
<span data-ttu-id="0f399-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [detectedApp](../resources/intune-devices-detectedapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0f399-130">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f399-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f399-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f399-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f399-132">Request</span></span>
<span data-ttu-id="0f399-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f399-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="0f399-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f399-134">Response</span></span>
<span data-ttu-id="0f399-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f399-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.detectedApp",
      "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
      "displayName": "Display Name value",
      "version": "Version value",
      "sizeInByte": 10,
      "deviceCount": 11
    }
  ]
}
```




