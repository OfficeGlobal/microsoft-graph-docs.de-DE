---
title: windowsPhone81CustomConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des windowsPhone81CustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ea82c3964562d491f71a6961b1c4dcd9ad301f0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261257"
---
# <a name="get-windowsphone81customconfiguration"></a><span data-ttu-id="d90fb-103">windowsPhone81CustomConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="d90fb-103">Get windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="d90fb-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d90fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d90fb-105">Lesen von Eigenschaften und Beziehungen des [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d90fb-105">Read properties and relationships of the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d90fb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d90fb-106">Prerequisites</span></span>
<span data-ttu-id="d90fb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d90fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d90fb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d90fb-109">Permission type</span></span>|<span data-ttu-id="d90fb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d90fb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d90fb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d90fb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d90fb-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d90fb-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d90fb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d90fb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d90fb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d90fb-114">Not supported.</span></span>|
|<span data-ttu-id="d90fb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d90fb-115">Application</span></span>|<span data-ttu-id="d90fb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d90fb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d90fb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d90fb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d90fb-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d90fb-118">Optional query parameters</span></span>
<span data-ttu-id="d90fb-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d90fb-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d90fb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d90fb-120">Request headers</span></span>
|<span data-ttu-id="d90fb-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d90fb-121">Header</span></span>|<span data-ttu-id="d90fb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d90fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d90fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d90fb-123">Authorization</span></span>|<span data-ttu-id="d90fb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d90fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d90fb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d90fb-125">Accept</span></span>|<span data-ttu-id="d90fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d90fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d90fb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d90fb-127">Request body</span></span>
<span data-ttu-id="d90fb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d90fb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d90fb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d90fb-129">Response</span></span>
<span data-ttu-id="d90fb-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d90fb-130">If successful, this method returns a `200 OK` response code and [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d90fb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d90fb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d90fb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d90fb-132">Request</span></span>
<span data-ttu-id="d90fb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d90fb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d90fb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d90fb-134">Response</span></span>
<span data-ttu-id="d90fb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d90fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
    "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSettingInteger",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "value": 5
      }
    ]
  }
}
```



