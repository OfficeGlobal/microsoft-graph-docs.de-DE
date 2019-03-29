---
title: IosEducationDeviceConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der iosEducationDeviceConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa4f568bc041b9fc74faeffd97b5c62c1b7f346f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981629"
---
# <a name="list-ioseducationdeviceconfigurations"></a><span data-ttu-id="6202f-103">IosEducationDeviceConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="6202f-103">List iosEducationDeviceConfigurations</span></span>

> <span data-ttu-id="6202f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6202f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6202f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6202f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6202f-106">AufListen von Eigenschaften und Beziehungen der [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="6202f-106">List properties and relationships of the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6202f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6202f-107">Prerequisites</span></span>
<span data-ttu-id="6202f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6202f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6202f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6202f-110">Permission type</span></span>|<span data-ttu-id="6202f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6202f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6202f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6202f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6202f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6202f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6202f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6202f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6202f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6202f-115">Not supported.</span></span>|
|<span data-ttu-id="6202f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6202f-116">Application</span></span>|<span data-ttu-id="6202f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6202f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6202f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6202f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6202f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6202f-119">Request headers</span></span>
|<span data-ttu-id="6202f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6202f-120">Header</span></span>|<span data-ttu-id="6202f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6202f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6202f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6202f-122">Authorization</span></span>|<span data-ttu-id="6202f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6202f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6202f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6202f-124">Accept</span></span>|<span data-ttu-id="6202f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6202f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6202f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6202f-126">Request body</span></span>
<span data-ttu-id="6202f-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6202f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6202f-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="6202f-128">Response</span></span>
<span data-ttu-id="6202f-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6202f-129">If successful, this method returns a `200 OK` response code and a collection of [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6202f-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6202f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6202f-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6202f-131">Request</span></span>
<span data-ttu-id="6202f-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6202f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6202f-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6202f-133">Response</span></span>
<span data-ttu-id="6202f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6202f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 510

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
      "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




