---
title: Auflisten von „managedDeviceMobileAppConfigurationAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedDeviceMobileAppConfigurationAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cc477f0193f80bb6df1fdc6f42eabe8e7fce220
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957227"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="5d3b1-103">Auflisten von „managedDeviceMobileAppConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="5d3b1-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="5d3b1-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5d3b1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d3b1-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="5d3b1-105">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d3b1-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5d3b1-106">Prerequisites</span></span>
<span data-ttu-id="5d3b1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d3b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d3b1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d3b1-109">Permission type</span></span>|<span data-ttu-id="5d3b1-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d3b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d3b1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d3b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5d3b1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d3b1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5d3b1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d3b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d3b1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d3b1-114">Not supported.</span></span>|
|<span data-ttu-id="5d3b1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d3b1-115">Application</span></span>|<span data-ttu-id="5d3b1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d3b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d3b1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d3b1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5d3b1-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d3b1-118">Request headers</span></span>
|<span data-ttu-id="5d3b1-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5d3b1-119">Header</span></span>|<span data-ttu-id="5d3b1-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5d3b1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d3b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d3b1-121">Authorization</span></span>|<span data-ttu-id="5d3b1-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5d3b1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d3b1-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5d3b1-123">Accept</span></span>|<span data-ttu-id="5d3b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5d3b1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d3b1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d3b1-125">Request body</span></span>
<span data-ttu-id="5d3b1-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5d3b1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d3b1-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d3b1-127">Response</span></span>
<span data-ttu-id="5d3b1-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5d3b1-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d3b1-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d3b1-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d3b1-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d3b1-130">Request</span></span>
<span data-ttu-id="5d3b1-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d3b1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="5d3b1-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d3b1-132">Response</span></span>
<span data-ttu-id="5d3b1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d3b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



