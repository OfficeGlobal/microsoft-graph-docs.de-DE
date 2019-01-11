---
title: Auflisten von „androidForWorkAppConfigurationSchema“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs androidForWorkAppConfigurationSchema auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b8fc68b90da5144453066d3c46028fc2d916152f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813930"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="6cce8-103">Auflisten von „androidForWorkAppConfigurationSchema“</span><span class="sxs-lookup"><span data-stu-id="6cce8-103">List androidForWorkAppConfigurationSchemas</span></span>

> <span data-ttu-id="6cce8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6cce8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cce8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6cce8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6cce8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6cce8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cce8-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) auf.</span><span class="sxs-lookup"><span data-stu-id="6cce8-107">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6cce8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6cce8-108">Prerequisites</span></span>
<span data-ttu-id="6cce8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cce8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cce8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6cce8-111">Permission type</span></span>|<span data-ttu-id="6cce8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6cce8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cce8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6cce8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cce8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cce8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6cce8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6cce8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cce8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cce8-116">Not supported.</span></span>|
|<span data-ttu-id="6cce8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6cce8-117">Application</span></span>|<span data-ttu-id="6cce8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cce8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cce8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cce8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="6cce8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6cce8-120">Request headers</span></span>
|<span data-ttu-id="6cce8-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6cce8-121">Header</span></span>|<span data-ttu-id="6cce8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6cce8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cce8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cce8-123">Authorization</span></span>|<span data-ttu-id="6cce8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6cce8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cce8-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6cce8-125">Accept</span></span>|<span data-ttu-id="6cce8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cce8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cce8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6cce8-127">Request body</span></span>
<span data-ttu-id="6cce8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6cce8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cce8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cce8-129">Response</span></span>
<span data-ttu-id="6cce8-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6cce8-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cce8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6cce8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6cce8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cce8-132">Request</span></span>
<span data-ttu-id="6cce8-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6cce8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="6cce8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cce8-134">Response</span></span>
<span data-ttu-id="6cce8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6cce8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
      "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
      "exampleJson": "ZXhhbXBsZUpzb24=",
      "schemaItems": [
        {
          "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
          "schemaItemKey": "Schema Item Key value",
          "displayName": "Display Name value",
          "description": "Description value",
          "defaultBoolValue": true,
          "defaultIntValue": 15,
          "defaultStringValue": "Default String Value value",
          "defaultStringArrayValue": [
            "Default String Array Value value"
          ],
          "dataType": "integer",
          "selections": [
            {
              "@odata.type": "microsoft.graph.keyValuePair",
              "name": "Name value",
              "value": "Value value"
            }
          ]
        }
      ]
    }
  ]
}
```





