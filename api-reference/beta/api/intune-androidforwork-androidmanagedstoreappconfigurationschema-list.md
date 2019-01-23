---
title: Liste androidManagedStoreAppConfigurationSchemas
description: Listeneigenschaften und Beziehungen der AndroidManagedStoreAppConfigurationSchema-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c655795b05dba448508001585d5ef2baa24e7da3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401782"
---
# <a name="list-androidmanagedstoreappconfigurationschemas"></a><span data-ttu-id="8c8fe-103">Liste androidManagedStoreAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="8c8fe-103">List androidManagedStoreAppConfigurationSchemas</span></span>

> <span data-ttu-id="8c8fe-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8c8fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8c8fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c8fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c8fe-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8c8fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c8fe-107">Listeneigenschaften und Beziehungen der [AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="8c8fe-107">List properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c8fe-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8c8fe-108">Prerequisites</span></span>
<span data-ttu-id="8c8fe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8c8fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8c8fe-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c8fe-111">Permission type</span></span>|<span data-ttu-id="8c8fe-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c8fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c8fe-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c8fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c8fe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c8fe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8c8fe-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c8fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c8fe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c8fe-116">Not supported.</span></span>|
|<span data-ttu-id="8c8fe-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c8fe-117">Application</span></span>|<span data-ttu-id="8c8fe-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c8fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c8fe-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c8fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="8c8fe-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c8fe-120">Request headers</span></span>
|<span data-ttu-id="8c8fe-121">Header</span><span class="sxs-lookup"><span data-stu-id="8c8fe-121">Header</span></span>|<span data-ttu-id="8c8fe-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8c8fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c8fe-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8c8fe-123">Authorization</span></span>|<span data-ttu-id="8c8fe-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8c8fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c8fe-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8c8fe-125">Accept</span></span>|<span data-ttu-id="8c8fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c8fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c8fe-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c8fe-127">Request body</span></span>
<span data-ttu-id="8c8fe-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8c8fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c8fe-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c8fe-129">Response</span></span>
<span data-ttu-id="8c8fe-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="8c8fe-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c8fe-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c8fe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c8fe-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c8fe-132">Request</span></span>
<span data-ttu-id="8c8fe-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c8fe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="8c8fe-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c8fe-134">Response</span></span>
<span data-ttu-id="8c8fe-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c8fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 987

{
  "value": [
    {
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
  ]
}
```




