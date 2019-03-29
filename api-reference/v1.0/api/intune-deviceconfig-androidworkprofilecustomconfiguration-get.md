---
title: AndroidWorkProfileCustomConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des androidWorkProfileCustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5fece69c0d287c8f8bdc8aa4a5121153c4cf3b1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965837"
---
# <a name="get-androidworkprofilecustomconfiguration"></a><span data-ttu-id="0d003-103">AndroidWorkProfileCustomConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="0d003-103">Get androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="0d003-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0d003-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d003-105">Lesen von Eigenschaften und Beziehungen des [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d003-105">Read properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d003-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0d003-106">Prerequisites</span></span>
<span data-ttu-id="0d003-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d003-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d003-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d003-109">Permission type</span></span>|<span data-ttu-id="0d003-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d003-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d003-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d003-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d003-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d003-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0d003-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d003-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d003-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d003-114">Not supported.</span></span>|
|<span data-ttu-id="0d003-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d003-115">Application</span></span>|<span data-ttu-id="0d003-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d003-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d003-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d003-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d003-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0d003-118">Optional query parameters</span></span>
<span data-ttu-id="0d003-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0d003-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d003-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d003-120">Request headers</span></span>
|<span data-ttu-id="0d003-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0d003-121">Header</span></span>|<span data-ttu-id="0d003-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0d003-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d003-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d003-123">Authorization</span></span>|<span data-ttu-id="0d003-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0d003-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d003-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0d003-125">Accept</span></span>|<span data-ttu-id="0d003-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d003-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d003-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d003-127">Request body</span></span>
<span data-ttu-id="0d003-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0d003-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d003-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d003-129">Response</span></span>
<span data-ttu-id="0d003-130">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0d003-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d003-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d003-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d003-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d003-132">Request</span></span>
<span data-ttu-id="0d003-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d003-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0d003-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d003-134">Response</span></span>
<span data-ttu-id="0d003-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d003-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 636

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
    "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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



