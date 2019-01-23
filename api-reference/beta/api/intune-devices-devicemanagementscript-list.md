---
title: Liste deviceManagementScripts
description: Listeneigenschaften und Beziehungen der DeviceManagementScript-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: db25a4211775785806b7d6a252c880079d2e40fc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419513"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="faecf-103">Liste deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="faecf-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="faecf-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="faecf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="faecf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="faecf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="faecf-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="faecf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faecf-107">Listeneigenschaften und Beziehungen der [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="faecf-107">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faecf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="faecf-108">Prerequisites</span></span>
<span data-ttu-id="faecf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="faecf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="faecf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="faecf-111">Permission type</span></span>|<span data-ttu-id="faecf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="faecf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faecf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="faecf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="faecf-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="faecf-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="faecf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="faecf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faecf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="faecf-116">Not supported.</span></span>|
|<span data-ttu-id="faecf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="faecf-117">Application</span></span>|<span data-ttu-id="faecf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="faecf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faecf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="faecf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="faecf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="faecf-120">Request headers</span></span>
|<span data-ttu-id="faecf-121">Header</span><span class="sxs-lookup"><span data-stu-id="faecf-121">Header</span></span>|<span data-ttu-id="faecf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="faecf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faecf-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="faecf-123">Authorization</span></span>|<span data-ttu-id="faecf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="faecf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faecf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="faecf-125">Accept</span></span>|<span data-ttu-id="faecf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="faecf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faecf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="faecf-127">Request body</span></span>
<span data-ttu-id="faecf-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="faecf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="faecf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="faecf-129">Response</span></span>
<span data-ttu-id="faecf-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="faecf-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faecf-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="faecf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="faecf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="faecf-132">Request</span></span>
<span data-ttu-id="faecf-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="faecf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="faecf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="faecf-134">Response</span></span>
<span data-ttu-id="faecf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="faecf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




