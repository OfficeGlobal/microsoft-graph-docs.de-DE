---
title: ManagedDeviceEnrollmentFailureTrends-Funktion
description: Metadaten für die Registrierung Trends Fehlerbericht
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e5d15c247c16e22748da0fe0db358adbe41035f9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411316"
---
# <a name="manageddeviceenrollmentfailuretrends-function"></a><span data-ttu-id="fc7c4-103">ManagedDeviceEnrollmentFailureTrends-Funktion</span><span class="sxs-lookup"><span data-stu-id="fc7c4-103">managedDeviceEnrollmentFailureTrends function</span></span>

> <span data-ttu-id="fc7c4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="fc7c4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fc7c4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc7c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc7c4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc7c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc7c4-107">Metadaten für die Registrierung Trends Fehlerbericht</span><span class="sxs-lookup"><span data-stu-id="fc7c4-107">Metadata for the enrollment failure trends report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc7c4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fc7c4-108">Prerequisites</span></span>
<span data-ttu-id="fc7c4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc7c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc7c4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc7c4-111">Permission type</span></span>|<span data-ttu-id="fc7c4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc7c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc7c4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc7c4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fc7c4-114">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="fc7c4-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fc7c4-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc7c4-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fc7c4-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc7c4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc7c4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc7c4-117">Not supported.</span></span>|
|<span data-ttu-id="fc7c4-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc7c4-118">Application</span></span>|<span data-ttu-id="fc7c4-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc7c4-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc7c4-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc7c4-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureTrends
```

## <a name="request-headers"></a><span data-ttu-id="fc7c4-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc7c4-121">Request headers</span></span>
|<span data-ttu-id="fc7c4-122">Header</span><span class="sxs-lookup"><span data-stu-id="fc7c4-122">Header</span></span>|<span data-ttu-id="fc7c4-123">Wert</span><span class="sxs-lookup"><span data-stu-id="fc7c4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc7c4-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fc7c4-124">Authorization</span></span>|<span data-ttu-id="fc7c4-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fc7c4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc7c4-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fc7c4-126">Accept</span></span>|<span data-ttu-id="fc7c4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fc7c4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc7c4-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc7c4-128">Request body</span></span>
<span data-ttu-id="fc7c4-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fc7c4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc7c4-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc7c4-130">Response</span></span>
<span data-ttu-id="fc7c4-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fc7c4-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc7c4-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc7c4-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc7c4-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc7c4-133">Request</span></span>
<span data-ttu-id="fc7c4-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fc7c4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureTrends
```

### <a name="response"></a><span data-ttu-id="fc7c4-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc7c4-135">Response</span></span>
<span data-ttu-id="fc7c4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc7c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



