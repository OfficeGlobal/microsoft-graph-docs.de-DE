---
title: Auflisten von „windowsPhone81CustomConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsPhone81CustomConfiguration auf.
ms.openlocfilehash: 9aae2a0b7e98bded001b1889f304a2f2b8c0a285
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062134"
---
# <a name="list-windowsphone81customconfigurations"></a><span data-ttu-id="d9ced-103">Auflisten von „windowsPhone81CustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="d9ced-103">List windowsPhone81CustomConfigurations</span></span>

> <span data-ttu-id="d9ced-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d9ced-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9ced-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9ced-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9ced-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d9ced-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9ced-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="d9ced-107">List properties and relationships of the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9ced-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d9ced-108">Prerequisites</span></span>
<span data-ttu-id="d9ced-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9ced-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9ced-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9ced-111">Permission type</span></span>|<span data-ttu-id="d9ced-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9ced-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9ced-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9ced-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9ced-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9ced-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d9ced-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9ced-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9ced-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9ced-116">Not supported.</span></span>|
|<span data-ttu-id="d9ced-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9ced-117">Application</span></span>|<span data-ttu-id="d9ced-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9ced-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9ced-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9ced-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d9ced-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9ced-120">Request headers</span></span>
|<span data-ttu-id="d9ced-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d9ced-121">Header</span></span>|<span data-ttu-id="d9ced-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d9ced-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9ced-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9ced-123">Authorization</span></span>|<span data-ttu-id="d9ced-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d9ced-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9ced-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9ced-125">Accept</span></span>|<span data-ttu-id="d9ced-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9ced-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9ced-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9ced-127">Request body</span></span>
<span data-ttu-id="d9ced-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d9ced-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9ced-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9ced-129">Response</span></span>
<span data-ttu-id="d9ced-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d9ced-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9ced-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9ced-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9ced-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9ced-132">Request</span></span>
<span data-ttu-id="d9ced-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9ced-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d9ced-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9ced-134">Response</span></span>
<span data-ttu-id="d9ced-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9ced-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 786

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
      "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```





