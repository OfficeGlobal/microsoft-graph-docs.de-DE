---
title: GetManagedDevicesWithAppFailures-Funktion
description: Ruft die Liste der Geräte mit fehlerhaften apps
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cafda91617bfd183606877bfda352370f2364c9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890069"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="bdae0-103">GetManagedDevicesWithAppFailures-Funktion</span><span class="sxs-lookup"><span data-stu-id="bdae0-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="bdae0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bdae0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdae0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bdae0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdae0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bdae0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdae0-107">Ruft die Liste der Geräte mit fehlerhaften apps</span><span class="sxs-lookup"><span data-stu-id="bdae0-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bdae0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bdae0-108">Prerequisites</span></span>
<span data-ttu-id="bdae0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdae0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdae0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bdae0-111">Permission type</span></span>|<span data-ttu-id="bdae0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bdae0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdae0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bdae0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bdae0-114">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="bdae0-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="bdae0-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdae0-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bdae0-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bdae0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdae0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bdae0-117">Not supported.</span></span>|
|<span data-ttu-id="bdae0-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bdae0-118">Application</span></span>|<span data-ttu-id="bdae0-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bdae0-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdae0-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdae0-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="bdae0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bdae0-121">Request headers</span></span>
|<span data-ttu-id="bdae0-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bdae0-122">Header</span></span>|<span data-ttu-id="bdae0-123">Wert</span><span class="sxs-lookup"><span data-stu-id="bdae0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdae0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdae0-124">Authorization</span></span>|<span data-ttu-id="bdae0-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bdae0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdae0-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bdae0-126">Accept</span></span>|<span data-ttu-id="bdae0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bdae0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdae0-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bdae0-128">Request body</span></span>
<span data-ttu-id="bdae0-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bdae0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdae0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdae0-130">Response</span></span>
<span data-ttu-id="bdae0-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bdae0-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdae0-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bdae0-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="bdae0-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdae0-133">Request</span></span>
<span data-ttu-id="bdae0-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bdae0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="bdae0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdae0-135">Response</span></span>
<span data-ttu-id="bdae0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bdae0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





