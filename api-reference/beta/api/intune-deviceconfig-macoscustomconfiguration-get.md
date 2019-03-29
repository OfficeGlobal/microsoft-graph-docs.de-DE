---
title: Abrufen von „macOSCustomConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 145f244417f4ea6692b2f83c1f6ac4dde3b1fa23
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982231"
---
# <a name="get-macoscustomconfiguration"></a><span data-ttu-id="9e405-103">Abrufen von „macOSCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="9e405-103">Get macOSCustomConfiguration</span></span>

> <span data-ttu-id="9e405-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e405-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e405-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9e405-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e405-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e405-106">Read properties and relationships of the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e405-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9e405-107">Prerequisites</span></span>
<span data-ttu-id="9e405-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e405-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e405-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9e405-110">Permission type</span></span>|<span data-ttu-id="9e405-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9e405-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e405-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9e405-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e405-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e405-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9e405-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9e405-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e405-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e405-115">Not supported.</span></span>|
|<span data-ttu-id="9e405-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9e405-116">Application</span></span>|<span data-ttu-id="9e405-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e405-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e405-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e405-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e405-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9e405-119">Optional query parameters</span></span>
<span data-ttu-id="9e405-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9e405-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e405-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9e405-121">Request headers</span></span>
|<span data-ttu-id="9e405-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9e405-122">Header</span></span>|<span data-ttu-id="9e405-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9e405-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e405-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e405-124">Authorization</span></span>|<span data-ttu-id="9e405-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9e405-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e405-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9e405-126">Accept</span></span>|<span data-ttu-id="9e405-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9e405-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e405-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9e405-128">Request body</span></span>
<span data-ttu-id="9e405-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9e405-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e405-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e405-130">Response</span></span>
<span data-ttu-id="9e405-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9e405-131">If successful, this method returns a `200 OK` response code and [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e405-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9e405-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e405-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e405-133">Request</span></span>
<span data-ttu-id="9e405-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9e405-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9e405-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e405-135">Response</span></span>
<span data-ttu-id="9e405-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e405-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "value": {
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
}
```




