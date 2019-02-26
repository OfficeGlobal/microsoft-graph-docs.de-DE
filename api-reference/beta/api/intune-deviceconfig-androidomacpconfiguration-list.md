---
title: AndroidOmaCpConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der androidOmaCpConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7bc60982e52f16e17b3a9df0063e551768c1f0ad
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177980"
---
# <a name="list-androidomacpconfigurations"></a><span data-ttu-id="a37a9-103">AndroidOmaCpConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="a37a9-103">List androidOmaCpConfigurations</span></span>

> <span data-ttu-id="a37a9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a37a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a37a9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a37a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a37a9-106">AufListen von Eigenschaften und Beziehungen der [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="a37a9-106">List properties and relationships of the [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a37a9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a37a9-107">Prerequisites</span></span>
<span data-ttu-id="a37a9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a37a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a37a9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a37a9-110">Permission type</span></span>|<span data-ttu-id="a37a9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a37a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a37a9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a37a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a37a9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a37a9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a37a9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a37a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a37a9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a37a9-115">Not supported.</span></span>|
|<span data-ttu-id="a37a9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a37a9-116">Application</span></span>|<span data-ttu-id="a37a9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a37a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a37a9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a37a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a37a9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a37a9-119">Request headers</span></span>
|<span data-ttu-id="a37a9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a37a9-120">Header</span></span>|<span data-ttu-id="a37a9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a37a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a37a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a37a9-122">Authorization</span></span>|<span data-ttu-id="a37a9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a37a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a37a9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a37a9-124">Accept</span></span>|<span data-ttu-id="a37a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a37a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a37a9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a37a9-126">Request body</span></span>
<span data-ttu-id="a37a9-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a37a9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a37a9-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="a37a9-128">Response</span></span>
<span data-ttu-id="a37a9-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a37a9-129">If successful, this method returns a `200 OK` response code and a collection of [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a37a9-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a37a9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a37a9-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a37a9-131">Request</span></span>
<span data-ttu-id="a37a9-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a37a9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a37a9-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a37a9-133">Response</span></span>
<span data-ttu-id="a37a9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a37a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 559

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
      "id": "5f682e4a-2e4a-5f68-4a2e-685f4a2e685f",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
    }
  ]
}
```




