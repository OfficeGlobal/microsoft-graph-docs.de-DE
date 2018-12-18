---
title: GetManagedDevicesWithAppFailures-Funktion
description: Ruft die Liste der Geräte mit fehlerhaften apps
author: tfitzmac
ms.openlocfilehash: 147ee26644c3e2c425f70434516e13b03407891b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352955"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="d8f9c-103">GetManagedDevicesWithAppFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="d8f9c-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="d8f9c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d8f9c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8f9c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8f9c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8f9c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d8f9c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8f9c-107">Ruft die Liste der Geräte mit fehlerhaften apps</span><span class="sxs-lookup"><span data-stu-id="d8f9c-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8f9c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d8f9c-108">Prerequisites</span></span>
<span data-ttu-id="d8f9c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8f9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8f9c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d8f9c-111">Permission type</span></span>|<span data-ttu-id="d8f9c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d8f9c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8f9c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d8f9c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d8f9c-114">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="d8f9c-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d8f9c-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8f9c-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d8f9c-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d8f9c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8f9c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d8f9c-117">Not supported.</span></span>|
|<span data-ttu-id="d8f9c-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d8f9c-118">Application</span></span>|<span data-ttu-id="d8f9c-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d8f9c-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8f9c-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8f9c-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="d8f9c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d8f9c-121">Request headers</span></span>
|<span data-ttu-id="d8f9c-122">Header</span><span class="sxs-lookup"><span data-stu-id="d8f9c-122">Header</span></span>|<span data-ttu-id="d8f9c-123">Wert</span><span class="sxs-lookup"><span data-stu-id="d8f9c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8f9c-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d8f9c-124">Authorization</span></span>|<span data-ttu-id="d8f9c-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d8f9c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8f9c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d8f9c-126">Accept</span></span>|<span data-ttu-id="d8f9c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d8f9c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8f9c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d8f9c-128">Request body</span></span>
<span data-ttu-id="d8f9c-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d8f9c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8f9c-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="d8f9c-130">Response</span></span>
<span data-ttu-id="d8f9c-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d8f9c-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8f9c-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d8f9c-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8f9c-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8f9c-133">Request</span></span>
<span data-ttu-id="d8f9c-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d8f9c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="d8f9c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="d8f9c-135">Response</span></span>
<span data-ttu-id="d8f9c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d8f9c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





