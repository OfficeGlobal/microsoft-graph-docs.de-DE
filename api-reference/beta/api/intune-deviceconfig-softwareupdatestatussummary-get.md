---
title: Abrufen von „softwareUpdateStatusSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs softwareUpdateStatusSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5e05d7b237d9964fba8b8fe7a7c4f32f59473ede
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406598"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="f7ccb-103">Abrufen von „softwareUpdateStatusSummary“</span><span class="sxs-lookup"><span data-stu-id="f7ccb-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="f7ccb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f7ccb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f7ccb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7ccb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7ccb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f7ccb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7ccb-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="f7ccb-107">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7ccb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f7ccb-108">Prerequisites</span></span>
<span data-ttu-id="f7ccb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f7ccb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f7ccb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7ccb-111">Permission type</span></span>|<span data-ttu-id="f7ccb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7ccb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7ccb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7ccb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7ccb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7ccb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f7ccb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7ccb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7ccb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7ccb-116">Not supported.</span></span>|
|<span data-ttu-id="f7ccb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7ccb-117">Application</span></span>|<span data-ttu-id="f7ccb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7ccb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7ccb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7ccb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7ccb-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f7ccb-120">Optional query parameters</span></span>
<span data-ttu-id="f7ccb-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f7ccb-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7ccb-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7ccb-122">Request headers</span></span>
|<span data-ttu-id="f7ccb-123">Header</span><span class="sxs-lookup"><span data-stu-id="f7ccb-123">Header</span></span>|<span data-ttu-id="f7ccb-124">Wert</span><span class="sxs-lookup"><span data-stu-id="f7ccb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7ccb-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f7ccb-125">Authorization</span></span>|<span data-ttu-id="f7ccb-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f7ccb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7ccb-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f7ccb-127">Accept</span></span>|<span data-ttu-id="f7ccb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f7ccb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7ccb-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7ccb-129">Request body</span></span>
<span data-ttu-id="f7ccb-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f7ccb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7ccb-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7ccb-131">Response</span></span>
<span data-ttu-id="f7ccb-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f7ccb-132">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7ccb-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7ccb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7ccb-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7ccb-134">Request</span></span>
<span data-ttu-id="f7ccb-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f7ccb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="f7ccb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7ccb-136">Response</span></span>
<span data-ttu-id="f7ccb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7ccb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": {
    "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
    "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
    "displayName": "Display Name value",
    "compliantDeviceCount": 4,
    "nonCompliantDeviceCount": 7,
    "remediatedDeviceCount": 5,
    "errorDeviceCount": 0,
    "unknownDeviceCount": 2,
    "conflictDeviceCount": 3,
    "notApplicableDeviceCount": 8,
    "compliantUserCount": 2,
    "nonCompliantUserCount": 5,
    "remediatedUserCount": 3,
    "errorUserCount": 14,
    "unknownUserCount": 0,
    "conflictUserCount": 1,
    "notApplicableUserCount": 6
  }
}
```




