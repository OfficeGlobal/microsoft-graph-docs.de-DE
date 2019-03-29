---
title: DeviceManagementScripts aufListen
description: AufListen von Eigenschaften und Beziehungen der Devicemanagementscript hinzugefügt-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be5e92ef3d3a916d969443a2648da84f0641714c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967447"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="031b0-103">DeviceManagementScripts aufListen</span><span class="sxs-lookup"><span data-stu-id="031b0-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="031b0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="031b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="031b0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="031b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="031b0-106">AufListen von Eigenschaften und Beziehungen der [devicemanagementscript hinzugefügt](../resources/intune-devices-devicemanagementscript.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="031b0-106">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="031b0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="031b0-107">Prerequisites</span></span>
<span data-ttu-id="031b0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="031b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="031b0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="031b0-110">Permission type</span></span>|<span data-ttu-id="031b0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="031b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="031b0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="031b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="031b0-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="031b0-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="031b0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="031b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="031b0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="031b0-115">Not supported.</span></span>|
|<span data-ttu-id="031b0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="031b0-116">Application</span></span>|<span data-ttu-id="031b0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="031b0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="031b0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="031b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="031b0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="031b0-119">Request headers</span></span>
|<span data-ttu-id="031b0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="031b0-120">Header</span></span>|<span data-ttu-id="031b0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="031b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="031b0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="031b0-122">Authorization</span></span>|<span data-ttu-id="031b0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="031b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="031b0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="031b0-124">Accept</span></span>|<span data-ttu-id="031b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="031b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="031b0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="031b0-126">Request body</span></span>
<span data-ttu-id="031b0-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="031b0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="031b0-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="031b0-128">Response</span></span>
<span data-ttu-id="031b0-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [devicemanagementscript hinzugefügt](../resources/intune-devices-devicemanagementscript.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="031b0-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="031b0-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="031b0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="031b0-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="031b0-131">Request</span></span>
<span data-ttu-id="031b0-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="031b0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="031b0-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="031b0-133">Response</span></span>
<span data-ttu-id="031b0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="031b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 716

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScript",
      "id": "59ea4525-4525-59ea-2545-ea592545ea59",
      "displayName": "Display Name value",
      "description": "Description value",
      "runSchedule": {
        "@odata.type": "microsoft.graph.runSchedule"
      },
      "scriptContent": "c2NyaXB0Q29udGVudA==",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "fileName": "File Name value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "runAs32Bit": true
    }
  ]
}
```




