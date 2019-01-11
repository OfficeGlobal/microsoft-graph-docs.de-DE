---
title: Auflisten von „iosCustomConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosCustomConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: df649e11cfcffd2f9091cac178852b9f689f6b65
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828063"
---
# <a name="list-ioscustomconfigurations"></a><span data-ttu-id="f893c-103">Auflisten von „iosCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="f893c-103">List iosCustomConfigurations</span></span>

> <span data-ttu-id="f893c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f893c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f893c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f893c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f893c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f893c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f893c-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="f893c-107">List properties and relationships of the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f893c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f893c-108">Prerequisites</span></span>
<span data-ttu-id="f893c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f893c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f893c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f893c-111">Permission type</span></span>|<span data-ttu-id="f893c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f893c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f893c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f893c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f893c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f893c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f893c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f893c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f893c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f893c-116">Not supported.</span></span>|
|<span data-ttu-id="f893c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f893c-117">Application</span></span>|<span data-ttu-id="f893c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f893c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f893c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f893c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f893c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f893c-120">Request headers</span></span>
|<span data-ttu-id="f893c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f893c-121">Header</span></span>|<span data-ttu-id="f893c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f893c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f893c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f893c-123">Authorization</span></span>|<span data-ttu-id="f893c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f893c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f893c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f893c-125">Accept</span></span>|<span data-ttu-id="f893c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f893c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f893c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f893c-127">Request body</span></span>
<span data-ttu-id="f893c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f893c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f893c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f893c-129">Response</span></span>
<span data-ttu-id="f893c-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f893c-130">If successful, this method returns a `200 OK` response code and a collection of [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f893c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f893c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f893c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f893c-132">Request</span></span>
<span data-ttu-id="f893c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f893c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f893c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f893c-134">Response</span></span>
<span data-ttu-id="f893c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f893c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCustomConfiguration",
      "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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





