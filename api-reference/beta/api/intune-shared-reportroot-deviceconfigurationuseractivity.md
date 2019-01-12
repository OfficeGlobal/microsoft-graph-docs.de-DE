---
title: Funktion „deviceConfigurationUserActivity“
description: Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3467b25da219bed76b2875f16d532a3d8b0269dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914311"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="803eb-103">Funktion „deviceConfigurationUserActivity“</span><span class="sxs-lookup"><span data-stu-id="803eb-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="803eb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="803eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="803eb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="803eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="803eb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="803eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="803eb-107">Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="803eb-107">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="803eb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="803eb-108">Prerequisites</span></span>
<span data-ttu-id="803eb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="803eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="803eb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="803eb-111">Permission type</span></span>|<span data-ttu-id="803eb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="803eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="803eb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="803eb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="803eb-114">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="803eb-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="803eb-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="803eb-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="803eb-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="803eb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="803eb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="803eb-117">Not supported.</span></span>|
|<span data-ttu-id="803eb-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="803eb-118">Application</span></span>|<span data-ttu-id="803eb-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="803eb-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="803eb-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="803eb-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="803eb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="803eb-121">Request headers</span></span>
|<span data-ttu-id="803eb-122">Header</span><span class="sxs-lookup"><span data-stu-id="803eb-122">Header</span></span>|<span data-ttu-id="803eb-123">Wert</span><span class="sxs-lookup"><span data-stu-id="803eb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="803eb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="803eb-124">Authorization</span></span>|<span data-ttu-id="803eb-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="803eb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="803eb-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="803eb-126">Accept</span></span>|<span data-ttu-id="803eb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="803eb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="803eb-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="803eb-128">Request body</span></span>
<span data-ttu-id="803eb-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="803eb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="803eb-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="803eb-130">Response</span></span>
<span data-ttu-id="803eb-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="803eb-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="803eb-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="803eb-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="803eb-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="803eb-133">Request</span></span>
<span data-ttu-id="803eb-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="803eb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="803eb-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="803eb-135">Response</span></span>
<span data-ttu-id="803eb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="803eb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



