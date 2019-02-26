---
title: Abrufen von „deviceConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e32b8f7a87cf188c474150b85c29d9f56b7ac842
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254317"
---
# <a name="get-deviceconfiguration"></a><span data-ttu-id="dd85f-103">Abrufen von „deviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="dd85f-103">Get deviceConfiguration</span></span>

> <span data-ttu-id="dd85f-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dd85f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd85f-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd85f-105">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd85f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dd85f-106">Prerequisites</span></span>
<span data-ttu-id="dd85f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd85f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dd85f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd85f-109">Permission type</span></span>|<span data-ttu-id="dd85f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd85f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd85f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd85f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dd85f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd85f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dd85f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd85f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd85f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd85f-114">Not supported.</span></span>|
|<span data-ttu-id="dd85f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd85f-115">Application</span></span>|<span data-ttu-id="dd85f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd85f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd85f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd85f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd85f-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="dd85f-118">Optional query parameters</span></span>
<span data-ttu-id="dd85f-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dd85f-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd85f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd85f-120">Request headers</span></span>
|<span data-ttu-id="dd85f-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dd85f-121">Header</span></span>|<span data-ttu-id="dd85f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dd85f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd85f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd85f-123">Authorization</span></span>|<span data-ttu-id="dd85f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dd85f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd85f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dd85f-125">Accept</span></span>|<span data-ttu-id="dd85f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd85f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd85f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd85f-127">Request body</span></span>
<span data-ttu-id="dd85f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dd85f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd85f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd85f-129">Response</span></span>
<span data-ttu-id="dd85f-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dd85f-130">If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd85f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd85f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd85f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd85f-132">Request</span></span>
<span data-ttu-id="dd85f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd85f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="dd85f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd85f-134">Response</span></span>
<span data-ttu-id="dd85f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd85f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 362

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfiguration",
    "id": "34977265-7265-3497-6572-973465729734",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



