---
title: ManagedDeviceEnrollmentFailureTrends-Funktion
description: Metadaten für die Registrierung Trends Fehlerbericht
author: tfitzmac
ms.openlocfilehash: 873169eb3532b149de337ff21afe4fb8c3f67fe1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316331"
---
# <a name="manageddeviceenrollmentfailuretrends-function"></a><span data-ttu-id="c12e7-103">ManagedDeviceEnrollmentFailureTrends-Funktion</span><span class="sxs-lookup"><span data-stu-id="c12e7-103">managedDeviceEnrollmentFailureTrends function</span></span>

> <span data-ttu-id="c12e7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c12e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c12e7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c12e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c12e7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c12e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c12e7-107">Metadaten für die Registrierung Trends Fehlerbericht</span><span class="sxs-lookup"><span data-stu-id="c12e7-107">Metadata for the enrollment failure trends report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c12e7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c12e7-108">Prerequisites</span></span>
<span data-ttu-id="c12e7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c12e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c12e7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c12e7-111">Permission type</span></span>|<span data-ttu-id="c12e7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c12e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c12e7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c12e7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c12e7-114">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="c12e7-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c12e7-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c12e7-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c12e7-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c12e7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c12e7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c12e7-117">Not supported.</span></span>|
|<span data-ttu-id="c12e7-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c12e7-118">Application</span></span>|<span data-ttu-id="c12e7-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c12e7-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c12e7-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c12e7-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureTrends
```

## <a name="request-headers"></a><span data-ttu-id="c12e7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c12e7-121">Request headers</span></span>
|<span data-ttu-id="c12e7-122">Header</span><span class="sxs-lookup"><span data-stu-id="c12e7-122">Header</span></span>|<span data-ttu-id="c12e7-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c12e7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c12e7-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c12e7-124">Authorization</span></span>|<span data-ttu-id="c12e7-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c12e7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c12e7-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c12e7-126">Accept</span></span>|<span data-ttu-id="c12e7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c12e7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c12e7-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c12e7-128">Request body</span></span>
<span data-ttu-id="c12e7-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c12e7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c12e7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c12e7-130">Response</span></span>
<span data-ttu-id="c12e7-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c12e7-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c12e7-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c12e7-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="c12e7-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c12e7-133">Request</span></span>
<span data-ttu-id="c12e7-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c12e7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureTrends
```

### <a name="response"></a><span data-ttu-id="c12e7-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c12e7-135">Response</span></span>
<span data-ttu-id="c12e7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c12e7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



