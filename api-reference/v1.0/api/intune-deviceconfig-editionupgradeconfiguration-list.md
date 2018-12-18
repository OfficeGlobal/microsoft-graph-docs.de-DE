---
title: Auflisten von „editionUpgradeConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs editionUpgradeConfiguration auf.
author: tfitzmac
ms.openlocfilehash: e3dc33fbecf05f65eac49adf50c747ce5545ed3c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355090"
---
# <a name="list-editionupgradeconfigurations"></a><span data-ttu-id="39447-103">Auflisten von „editionUpgradeConfiguration“</span><span class="sxs-lookup"><span data-stu-id="39447-103">List editionUpgradeConfigurations</span></span>

> <span data-ttu-id="39447-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="39447-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39447-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="39447-105">List properties and relationships of the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39447-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="39447-106">Prerequisites</span></span>
<span data-ttu-id="39447-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39447-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39447-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39447-109">Permission type</span></span>|<span data-ttu-id="39447-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39447-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39447-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39447-111">Delegated (work or school account)</span></span>|<span data-ttu-id="39447-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="39447-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="39447-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39447-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39447-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39447-114">Not supported.</span></span>|
|<span data-ttu-id="39447-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39447-115">Application</span></span>|<span data-ttu-id="39447-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39447-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39447-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39447-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="39447-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39447-118">Request headers</span></span>
|<span data-ttu-id="39447-119">Header</span><span class="sxs-lookup"><span data-stu-id="39447-119">Header</span></span>|<span data-ttu-id="39447-120">Wert</span><span class="sxs-lookup"><span data-stu-id="39447-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39447-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="39447-121">Authorization</span></span>|<span data-ttu-id="39447-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="39447-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39447-123">Accept</span><span class="sxs-lookup"><span data-stu-id="39447-123">Accept</span></span>|<span data-ttu-id="39447-124">application/json</span><span class="sxs-lookup"><span data-stu-id="39447-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39447-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39447-125">Request body</span></span>
<span data-ttu-id="39447-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="39447-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39447-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="39447-127">Response</span></span>
<span data-ttu-id="39447-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="39447-128">If successful, this method returns a `200 OK` response code and a collection of [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39447-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39447-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="39447-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39447-130">Request</span></span>
<span data-ttu-id="39447-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39447-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="39447-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="39447-132">Response</span></span>
<span data-ttu-id="39447-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39447-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "value": [
    {
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
  ]
}
```



