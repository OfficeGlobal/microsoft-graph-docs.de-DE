---
title: Funktion „deviceConfigurationUserActivity“
description: Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration
author: tfitzmac
ms.openlocfilehash: 3cf73f5b8df21d7675ceeeed1b11bd1705e19c1c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305495"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="427a1-103">Funktion „deviceConfigurationUserActivity“</span><span class="sxs-lookup"><span data-stu-id="427a1-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="427a1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="427a1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="427a1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="427a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="427a1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="427a1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="427a1-107">Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="427a1-107">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="427a1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="427a1-108">Prerequisites</span></span>
<span data-ttu-id="427a1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="427a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="427a1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="427a1-111">Permission type</span></span>|<span data-ttu-id="427a1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="427a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="427a1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="427a1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="427a1-114">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="427a1-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="427a1-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="427a1-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="427a1-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="427a1-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="427a1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="427a1-117">Not supported.</span></span>|
|<span data-ttu-id="427a1-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="427a1-118">Application</span></span>|<span data-ttu-id="427a1-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="427a1-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="427a1-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="427a1-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="427a1-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="427a1-121">Request headers</span></span>
|<span data-ttu-id="427a1-122">Header</span><span class="sxs-lookup"><span data-stu-id="427a1-122">Header</span></span>|<span data-ttu-id="427a1-123">Wert</span><span class="sxs-lookup"><span data-stu-id="427a1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="427a1-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="427a1-124">Authorization</span></span>|<span data-ttu-id="427a1-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="427a1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="427a1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="427a1-126">Accept</span></span>|<span data-ttu-id="427a1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="427a1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="427a1-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="427a1-128">Request body</span></span>
<span data-ttu-id="427a1-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="427a1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="427a1-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="427a1-130">Response</span></span>
<span data-ttu-id="427a1-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="427a1-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="427a1-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="427a1-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="427a1-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="427a1-133">Request</span></span>
<span data-ttu-id="427a1-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="427a1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="427a1-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="427a1-135">Response</span></span>
<span data-ttu-id="427a1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="427a1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



