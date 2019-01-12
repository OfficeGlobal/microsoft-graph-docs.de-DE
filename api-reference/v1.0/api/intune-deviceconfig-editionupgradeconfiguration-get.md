---
title: Abrufen von „editionUpgradeConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8701fc9420d4e659ddd138cae37ff4eb66483032
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953813"
---
# <a name="get-editionupgradeconfiguration"></a><span data-ttu-id="6818a-103">Abrufen von „editionUpgradeConfiguration“</span><span class="sxs-lookup"><span data-stu-id="6818a-103">Get editionUpgradeConfiguration</span></span>

> <span data-ttu-id="6818a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6818a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6818a-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6818a-105">Read properties and relationships of the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6818a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6818a-106">Prerequisites</span></span>
<span data-ttu-id="6818a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6818a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6818a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6818a-109">Permission type</span></span>|<span data-ttu-id="6818a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6818a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6818a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6818a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6818a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6818a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6818a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6818a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6818a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6818a-114">Not supported.</span></span>|
|<span data-ttu-id="6818a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6818a-115">Application</span></span>|<span data-ttu-id="6818a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6818a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6818a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6818a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6818a-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6818a-118">Optional query parameters</span></span>
<span data-ttu-id="6818a-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6818a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6818a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6818a-120">Request headers</span></span>
|<span data-ttu-id="6818a-121">Header</span><span class="sxs-lookup"><span data-stu-id="6818a-121">Header</span></span>|<span data-ttu-id="6818a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6818a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6818a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6818a-123">Authorization</span></span>|<span data-ttu-id="6818a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6818a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6818a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6818a-125">Accept</span></span>|<span data-ttu-id="6818a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6818a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6818a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6818a-127">Request body</span></span>
<span data-ttu-id="6818a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6818a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6818a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6818a-129">Response</span></span>
<span data-ttu-id="6818a-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6818a-130">If successful, this method returns a `200 OK` response code and [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6818a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6818a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6818a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6818a-132">Request</span></span>
<span data-ttu-id="6818a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6818a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6818a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6818a-134">Response</span></span>
<span data-ttu-id="6818a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6818a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 524

{
  "value": {
    "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
    "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "licenseType": "licenseFile",
    "targetEdition": "windows10EnterpriseN",
    "license": "License value",
    "productKey": "Product Key value"
  }
}
```



