---
title: Auflisten von „deviceConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19199da330a12ff400ee4b5845b8fcc580c35083
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257211"
---
# <a name="list-deviceconfigurations"></a><span data-ttu-id="041ee-103">Auflisten von „deviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="041ee-103">List deviceConfigurations</span></span>

> <span data-ttu-id="041ee-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="041ee-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="041ee-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="041ee-105">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="041ee-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="041ee-106">Prerequisites</span></span>
<span data-ttu-id="041ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="041ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="041ee-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="041ee-109">Permission type</span></span>|<span data-ttu-id="041ee-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="041ee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="041ee-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="041ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="041ee-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="041ee-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="041ee-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="041ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="041ee-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="041ee-114">Not supported.</span></span>|
|<span data-ttu-id="041ee-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="041ee-115">Application</span></span>|<span data-ttu-id="041ee-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="041ee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="041ee-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="041ee-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="041ee-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="041ee-118">Request headers</span></span>
|<span data-ttu-id="041ee-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="041ee-119">Header</span></span>|<span data-ttu-id="041ee-120">Wert</span><span class="sxs-lookup"><span data-stu-id="041ee-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="041ee-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="041ee-121">Authorization</span></span>|<span data-ttu-id="041ee-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="041ee-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="041ee-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="041ee-123">Accept</span></span>|<span data-ttu-id="041ee-124">application/json</span><span class="sxs-lookup"><span data-stu-id="041ee-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="041ee-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="041ee-125">Request body</span></span>
<span data-ttu-id="041ee-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="041ee-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="041ee-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="041ee-127">Response</span></span>
<span data-ttu-id="041ee-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="041ee-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="041ee-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="041ee-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="041ee-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="041ee-130">Request</span></span>
<span data-ttu-id="041ee-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="041ee-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="041ee-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="041ee-132">Response</span></span>
<span data-ttu-id="041ee-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="041ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 390

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfiguration",
      "id": "34977265-7265-3497-6572-973465729734",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



