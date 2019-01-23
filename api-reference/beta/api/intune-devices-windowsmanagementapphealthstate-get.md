---
title: Abrufen von windowsManagementAppHealthState
description: Lesen Sie Eigenschaften und Beziehungen des WindowsManagementAppHealthState-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fad8c0404bd253c9418b6c7cad517b07bd66fd3c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408474"
---
# <a name="get-windowsmanagementapphealthstate"></a><span data-ttu-id="55b42-103">Abrufen von windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="55b42-103">Get windowsManagementAppHealthState</span></span>

> <span data-ttu-id="55b42-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="55b42-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="55b42-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="55b42-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55b42-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="55b42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55b42-107">Lesen Sie Eigenschaften und Beziehungen des [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="55b42-107">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55b42-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="55b42-108">Prerequisites</span></span>
<span data-ttu-id="55b42-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="55b42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="55b42-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="55b42-111">Permission type</span></span>|<span data-ttu-id="55b42-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="55b42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55b42-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="55b42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55b42-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="55b42-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="55b42-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="55b42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55b42-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55b42-116">Not supported.</span></span>|
|<span data-ttu-id="55b42-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="55b42-117">Application</span></span>|<span data-ttu-id="55b42-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55b42-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55b42-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="55b42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55b42-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="55b42-120">Optional query parameters</span></span>
<span data-ttu-id="55b42-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="55b42-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55b42-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="55b42-122">Request headers</span></span>
|<span data-ttu-id="55b42-123">Header</span><span class="sxs-lookup"><span data-stu-id="55b42-123">Header</span></span>|<span data-ttu-id="55b42-124">Wert</span><span class="sxs-lookup"><span data-stu-id="55b42-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55b42-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="55b42-125">Authorization</span></span>|<span data-ttu-id="55b42-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="55b42-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55b42-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="55b42-127">Accept</span></span>|<span data-ttu-id="55b42-128">application/json</span><span class="sxs-lookup"><span data-stu-id="55b42-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55b42-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="55b42-129">Request body</span></span>
<span data-ttu-id="55b42-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="55b42-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55b42-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="55b42-131">Response</span></span>
<span data-ttu-id="55b42-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="55b42-132">If successful, this method returns a `200 OK` response code and [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55b42-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="55b42-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="55b42-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="55b42-134">Request</span></span>
<span data-ttu-id="55b42-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="55b42-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

### <a name="response"></a><span data-ttu-id="55b42-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="55b42-136">Response</span></span>
<span data-ttu-id="55b42-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="55b42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 382

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
    "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
    "healthState": "healthy",
    "installedVersion": "Installed Version value",
    "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
    "deviceName": "Device Name value",
    "deviceOSVersion": "Device OSVersion value"
  }
}
```




