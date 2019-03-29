---
title: deviceConfigurationUserStatus abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationUserStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d2e7ba1a4459bc8d33e38bea3e83902ba9d5551
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980621"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="ea607-103">deviceConfigurationUserStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="ea607-103">Get deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="ea607-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ea607-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea607-105">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea607-105">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea607-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ea607-106">Prerequisites</span></span>
<span data-ttu-id="ea607-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea607-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea607-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea607-109">Permission type</span></span>|<span data-ttu-id="ea607-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea607-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea607-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea607-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ea607-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea607-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ea607-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea607-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea607-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea607-114">Not supported.</span></span>|
|<span data-ttu-id="ea607-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea607-115">Application</span></span>|<span data-ttu-id="ea607-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea607-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea607-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea607-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea607-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ea607-118">Optional query parameters</span></span>
<span data-ttu-id="ea607-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ea607-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea607-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea607-120">Request headers</span></span>
|<span data-ttu-id="ea607-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ea607-121">Header</span></span>|<span data-ttu-id="ea607-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ea607-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea607-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea607-123">Authorization</span></span>|<span data-ttu-id="ea607-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ea607-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea607-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ea607-125">Accept</span></span>|<span data-ttu-id="ea607-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea607-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea607-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea607-127">Request body</span></span>
<span data-ttu-id="ea607-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ea607-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea607-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea607-129">Response</span></span>
<span data-ttu-id="ea607-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea607-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea607-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea607-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea607-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea607-132">Request</span></span>
<span data-ttu-id="ea607-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea607-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="ea607-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea607-134">Response</span></span>
<span data-ttu-id="ea607-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea607-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
    "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



