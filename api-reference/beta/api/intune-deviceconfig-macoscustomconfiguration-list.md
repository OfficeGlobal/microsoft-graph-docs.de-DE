---
title: Auflisten von „macOSCustomConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs macOSCustomConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69abf859aaf1935b19573d878da34f98289f21f3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146424"
---
# <a name="list-macoscustomconfigurations"></a><span data-ttu-id="db13b-103">Auflisten von „macOSCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="db13b-103">List macOSCustomConfigurations</span></span>

> <span data-ttu-id="db13b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="db13b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db13b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="db13b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db13b-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="db13b-106">List properties and relationships of the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db13b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="db13b-107">Prerequisites</span></span>
<span data-ttu-id="db13b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="db13b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="db13b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db13b-110">Permission type</span></span>|<span data-ttu-id="db13b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="db13b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db13b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db13b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db13b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="db13b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="db13b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="db13b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db13b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db13b-115">Not supported.</span></span>|
|<span data-ttu-id="db13b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db13b-116">Application</span></span>|<span data-ttu-id="db13b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db13b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db13b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db13b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="db13b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db13b-119">Request headers</span></span>
|<span data-ttu-id="db13b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="db13b-120">Header</span></span>|<span data-ttu-id="db13b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="db13b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db13b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db13b-122">Authorization</span></span>|<span data-ttu-id="db13b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="db13b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db13b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="db13b-124">Accept</span></span>|<span data-ttu-id="db13b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db13b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db13b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db13b-126">Request body</span></span>
<span data-ttu-id="db13b-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="db13b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db13b-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="db13b-128">Response</span></span>
<span data-ttu-id="db13b-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="db13b-129">If successful, this method returns a `200 OK` response code and a collection of [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db13b-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db13b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="db13b-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="db13b-131">Request</span></span>
<span data-ttu-id="db13b-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="db13b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="db13b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="db13b-133">Response</span></span>
<span data-ttu-id="db13b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db13b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 634

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
      "id": "a253835d-835d-a253-5d83-53a25d8353a2",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "payloadName": "Payload Name value",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA=="
    }
  ]
}
```




