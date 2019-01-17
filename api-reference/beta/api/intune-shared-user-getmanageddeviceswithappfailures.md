---
title: GetManagedDevicesWithAppFailures-Funktion
description: Ruft die Liste der Geräte mit fehlerhaften apps
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 18b1a4275d623cf3d35d38db1d183bdd344e7cfe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918749"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="cf3d9-103">GetManagedDevicesWithAppFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="cf3d9-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="cf3d9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cf3d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf3d9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cf3d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf3d9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cf3d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf3d9-107">Ruft die Liste der Geräte mit fehlerhaften apps</span><span class="sxs-lookup"><span data-stu-id="cf3d9-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf3d9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cf3d9-108">Prerequisites</span></span>
<span data-ttu-id="cf3d9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf3d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf3d9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf3d9-111">Permission type</span></span>|<span data-ttu-id="cf3d9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf3d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf3d9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf3d9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cf3d9-114">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="cf3d9-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="cf3d9-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf3d9-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cf3d9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf3d9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf3d9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf3d9-117">Not supported.</span></span>|
|<span data-ttu-id="cf3d9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf3d9-118">Application</span></span>|<span data-ttu-id="cf3d9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf3d9-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf3d9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf3d9-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="cf3d9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf3d9-121">Request headers</span></span>
|<span data-ttu-id="cf3d9-122">Header</span><span class="sxs-lookup"><span data-stu-id="cf3d9-122">Header</span></span>|<span data-ttu-id="cf3d9-123">Wert</span><span class="sxs-lookup"><span data-stu-id="cf3d9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf3d9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf3d9-124">Authorization</span></span>|<span data-ttu-id="cf3d9-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cf3d9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf3d9-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cf3d9-126">Accept</span></span>|<span data-ttu-id="cf3d9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cf3d9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf3d9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf3d9-128">Request body</span></span>
<span data-ttu-id="cf3d9-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cf3d9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf3d9-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf3d9-130">Response</span></span>
<span data-ttu-id="cf3d9-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cf3d9-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf3d9-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf3d9-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf3d9-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf3d9-133">Request</span></span>
<span data-ttu-id="cf3d9-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf3d9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="cf3d9-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf3d9-135">Response</span></span>
<span data-ttu-id="cf3d9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf3d9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 74

{
  "value": [
    "Get Managed Devices With App Failures value"
  ]
}
```





