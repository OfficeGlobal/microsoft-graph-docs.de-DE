---
title: WindowsManagementAppHealthStates aufListen
description: AufListen von Eigenschaften und Beziehungen der windowsManagementAppHealthState-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fc503791ba525c7a49f263931aef632079e088d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980068"
---
# <a name="list-windowsmanagementapphealthstates"></a><span data-ttu-id="c1845-103">WindowsManagementAppHealthStates aufListen</span><span class="sxs-lookup"><span data-stu-id="c1845-103">List windowsManagementAppHealthStates</span></span>

> <span data-ttu-id="c1845-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1845-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1845-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c1845-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1845-106">AufListen von Eigenschaften und Beziehungen der [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="c1845-106">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1845-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1845-107">Prerequisites</span></span>
<span data-ttu-id="c1845-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1845-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1845-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1845-110">Permission type</span></span>|<span data-ttu-id="c1845-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1845-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1845-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1845-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1845-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1845-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c1845-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1845-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1845-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1845-115">Not supported.</span></span>|
|<span data-ttu-id="c1845-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1845-116">Application</span></span>|<span data-ttu-id="c1845-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1845-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1845-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1845-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="c1845-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1845-119">Request headers</span></span>
|<span data-ttu-id="c1845-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c1845-120">Header</span></span>|<span data-ttu-id="c1845-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c1845-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1845-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1845-122">Authorization</span></span>|<span data-ttu-id="c1845-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1845-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1845-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c1845-124">Accept</span></span>|<span data-ttu-id="c1845-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1845-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1845-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1845-126">Request body</span></span>
<span data-ttu-id="c1845-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c1845-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1845-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1845-128">Response</span></span>
<span data-ttu-id="c1845-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c1845-129">If successful, this method returns a `200 OK` response code and a collection of [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1845-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1845-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1845-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1845-131">Request</span></span>
<span data-ttu-id="c1845-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1845-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
```

### <a name="response"></a><span data-ttu-id="c1845-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1845-133">Response</span></span>
<span data-ttu-id="c1845-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1845-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
      "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
      "healthState": "healthy",
      "installedVersion": "Installed Version value",
      "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
      "deviceName": "Device Name value",
      "deviceOSVersion": "Device OSVersion value"
    }
  ]
}
```




