---
title: Abrufen von „deviceConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 146e659e26e2d146e1160908ad24b32d419b4cb1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956779"
---
# <a name="get-deviceconfiguration"></a><span data-ttu-id="0421c-103">Abrufen von „deviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="0421c-103">Get deviceConfiguration</span></span>

> <span data-ttu-id="0421c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0421c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0421c-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0421c-105">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0421c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0421c-106">Prerequisites</span></span>
<span data-ttu-id="0421c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0421c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0421c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0421c-109">Permission type</span></span>|<span data-ttu-id="0421c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0421c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0421c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0421c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0421c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0421c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0421c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0421c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0421c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0421c-114">Not supported.</span></span>|
|<span data-ttu-id="0421c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0421c-115">Application</span></span>|<span data-ttu-id="0421c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0421c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0421c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0421c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0421c-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0421c-118">Optional query parameters</span></span>
<span data-ttu-id="0421c-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0421c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0421c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0421c-120">Request headers</span></span>
|<span data-ttu-id="0421c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0421c-121">Header</span></span>|<span data-ttu-id="0421c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0421c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0421c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0421c-123">Authorization</span></span>|<span data-ttu-id="0421c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0421c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0421c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0421c-125">Accept</span></span>|<span data-ttu-id="0421c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0421c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0421c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0421c-127">Request body</span></span>
<span data-ttu-id="0421c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0421c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0421c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0421c-129">Response</span></span>
<span data-ttu-id="0421c-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0421c-130">If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0421c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0421c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0421c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0421c-132">Request</span></span>
<span data-ttu-id="0421c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0421c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0421c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0421c-134">Response</span></span>
<span data-ttu-id="0421c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0421c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



