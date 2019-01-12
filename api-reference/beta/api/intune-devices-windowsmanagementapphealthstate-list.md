---
title: Liste windowsManagementAppHealthStates
description: Listeneigenschaften und Beziehungen der WindowsManagementAppHealthState-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d4c76297d41b63bd765c952a831df4cb201c245c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913562"
---
# <a name="list-windowsmanagementapphealthstates"></a><span data-ttu-id="51ec0-103">Liste windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="51ec0-103">List windowsManagementAppHealthStates</span></span>

> <span data-ttu-id="51ec0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="51ec0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51ec0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51ec0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51ec0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="51ec0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51ec0-107">Listeneigenschaften und Beziehungen der [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="51ec0-107">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51ec0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="51ec0-108">Prerequisites</span></span>
<span data-ttu-id="51ec0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51ec0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51ec0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51ec0-111">Permission type</span></span>|<span data-ttu-id="51ec0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51ec0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51ec0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51ec0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51ec0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="51ec0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="51ec0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51ec0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51ec0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51ec0-116">Not supported.</span></span>|
|<span data-ttu-id="51ec0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51ec0-117">Application</span></span>|<span data-ttu-id="51ec0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51ec0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51ec0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51ec0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="51ec0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51ec0-120">Request headers</span></span>
|<span data-ttu-id="51ec0-121">Header</span><span class="sxs-lookup"><span data-stu-id="51ec0-121">Header</span></span>|<span data-ttu-id="51ec0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="51ec0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51ec0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51ec0-123">Authorization</span></span>|<span data-ttu-id="51ec0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="51ec0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51ec0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="51ec0-125">Accept</span></span>|<span data-ttu-id="51ec0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51ec0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51ec0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51ec0-127">Request body</span></span>
<span data-ttu-id="51ec0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="51ec0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51ec0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="51ec0-129">Response</span></span>
<span data-ttu-id="51ec0-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="51ec0-130">If successful, this method returns a `200 OK` response code and a collection of [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51ec0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51ec0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="51ec0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51ec0-132">Request</span></span>
<span data-ttu-id="51ec0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51ec0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
```

### <a name="response"></a><span data-ttu-id="51ec0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="51ec0-134">Response</span></span>
<span data-ttu-id="51ec0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51ec0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





