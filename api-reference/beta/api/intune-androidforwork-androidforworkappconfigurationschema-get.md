---
title: Abrufen von „androidForWorkAppConfigurationSchema“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs androidForWorkAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4028244c487aaecbb9ab53a18800ee7769239f6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977345"
---
# <a name="get-androidforworkappconfigurationschema"></a><span data-ttu-id="a1aca-103">Abrufen von „androidForWorkAppConfigurationSchema“</span><span class="sxs-lookup"><span data-stu-id="a1aca-103">Get androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="a1aca-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1aca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1aca-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a1aca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1aca-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="a1aca-106">Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1aca-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a1aca-107">Prerequisites</span></span>
<span data-ttu-id="a1aca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1aca-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1aca-110">Permission type</span></span>|<span data-ttu-id="a1aca-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1aca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1aca-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1aca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1aca-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1aca-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a1aca-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1aca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1aca-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1aca-115">Not supported.</span></span>|
|<span data-ttu-id="a1aca-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1aca-116">Application</span></span>|<span data-ttu-id="a1aca-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1aca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1aca-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1aca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1aca-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a1aca-119">Optional query parameters</span></span>
<span data-ttu-id="a1aca-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a1aca-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1aca-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1aca-121">Request headers</span></span>
|<span data-ttu-id="a1aca-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a1aca-122">Header</span></span>|<span data-ttu-id="a1aca-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a1aca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1aca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1aca-124">Authorization</span></span>|<span data-ttu-id="a1aca-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a1aca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1aca-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a1aca-126">Accept</span></span>|<span data-ttu-id="a1aca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a1aca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1aca-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1aca-128">Request body</span></span>
<span data-ttu-id="a1aca-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a1aca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1aca-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1aca-130">Response</span></span>
<span data-ttu-id="a1aca-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a1aca-131">If successful, this method returns a `200 OK` response code and [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1aca-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1aca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1aca-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1aca-133">Request</span></span>
<span data-ttu-id="a1aca-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a1aca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="a1aca-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1aca-135">Response</span></span>
<span data-ttu-id="a1aca-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1aca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 913

{
  "value": {
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
}
```




