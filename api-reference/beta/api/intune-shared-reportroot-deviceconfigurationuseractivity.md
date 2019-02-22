---
title: Funktion „deviceConfigurationUserActivity“
description: Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c92de4aeb052d62333e0947f08f755a5e05f4d7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166986"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="4b601-103">Funktion „deviceConfigurationUserActivity“</span><span class="sxs-lookup"><span data-stu-id="4b601-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="4b601-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="4b601-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4b601-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b601-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b601-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4b601-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b601-107">Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="4b601-107">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b601-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4b601-108">Prerequisites</span></span>
<span data-ttu-id="4b601-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b601-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="4b601-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b601-111">Permission type</span></span>|<span data-ttu-id="4b601-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b601-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b601-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b601-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4b601-114">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="4b601-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4b601-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b601-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4b601-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b601-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b601-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b601-117">Not supported.</span></span>|
|<span data-ttu-id="4b601-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b601-118">Application</span></span>|<span data-ttu-id="4b601-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b601-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b601-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b601-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="4b601-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b601-121">Request headers</span></span>
|<span data-ttu-id="4b601-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4b601-122">Header</span></span>|<span data-ttu-id="4b601-123">Wert</span><span class="sxs-lookup"><span data-stu-id="4b601-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b601-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b601-124">Authorization</span></span>|<span data-ttu-id="4b601-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4b601-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b601-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4b601-126">Accept</span></span>|<span data-ttu-id="4b601-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4b601-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b601-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b601-128">Request body</span></span>
<span data-ttu-id="4b601-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4b601-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b601-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b601-130">Response</span></span>
<span data-ttu-id="4b601-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4b601-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b601-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b601-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b601-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b601-133">Request</span></span>
<span data-ttu-id="4b601-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b601-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="4b601-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b601-135">Response</span></span>
<span data-ttu-id="4b601-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b601-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



