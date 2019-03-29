---
title: AndroidManagedStoreAppConfigurationSchema abrufen
description: Lesen von Eigenschaften und Beziehungen des androidManagedStoreAppConfigurationSchema-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d072c59decb189b375c4bf83349e93a89260dd13
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966957"
---
# <a name="get-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="f8993-103">AndroidManagedStoreAppConfigurationSchema abrufen</span><span class="sxs-lookup"><span data-stu-id="f8993-103">Get androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="f8993-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8993-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8993-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f8993-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8993-106">Lesen von Eigenschaften und Beziehungen des [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f8993-106">Read properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8993-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f8993-107">Prerequisites</span></span>
<span data-ttu-id="f8993-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8993-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8993-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8993-110">Permission type</span></span>|<span data-ttu-id="f8993-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8993-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8993-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8993-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8993-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8993-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f8993-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8993-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8993-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8993-115">Not supported.</span></span>|
|<span data-ttu-id="f8993-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8993-116">Application</span></span>|<span data-ttu-id="f8993-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8993-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8993-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8993-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8993-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f8993-119">Optional query parameters</span></span>
<span data-ttu-id="f8993-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f8993-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8993-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8993-121">Request headers</span></span>
|<span data-ttu-id="f8993-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f8993-122">Header</span></span>|<span data-ttu-id="f8993-123">Wert</span><span class="sxs-lookup"><span data-stu-id="f8993-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8993-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8993-124">Authorization</span></span>|<span data-ttu-id="f8993-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f8993-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8993-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f8993-126">Accept</span></span>|<span data-ttu-id="f8993-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f8993-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8993-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8993-128">Request body</span></span>
<span data-ttu-id="f8993-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f8993-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8993-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8993-130">Response</span></span>
<span data-ttu-id="f8993-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f8993-131">If successful, this method returns a `200 OK` response code and [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8993-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8993-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8993-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8993-133">Request</span></span>
<span data-ttu-id="f8993-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8993-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="f8993-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8993-135">Response</span></span>
<span data-ttu-id="f8993-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8993-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 923

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
    "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
    "exampleJson": "ZXhhbXBsZUpzb24=",
    "schemaItems": [
      {
        "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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




