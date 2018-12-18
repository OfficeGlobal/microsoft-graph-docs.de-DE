---
title: Abrufen von „macOSCustomConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs macOSCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 20e5cb57507bee1636fdb4dd299a7b8948ecd4f2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332858"
---
# <a name="get-macoscustomconfiguration"></a><span data-ttu-id="5b837-103">Abrufen von „macOSCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="5b837-103">Get macOSCustomConfiguration</span></span>

> <span data-ttu-id="5b837-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5b837-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b837-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b837-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b837-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5b837-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b837-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b837-107">Read properties and relationships of the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b837-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5b837-108">Prerequisites</span></span>
<span data-ttu-id="5b837-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b837-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b837-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b837-111">Permission type</span></span>|<span data-ttu-id="5b837-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b837-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b837-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b837-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b837-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b837-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5b837-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b837-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b837-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b837-116">Not supported.</span></span>|
|<span data-ttu-id="5b837-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b837-117">Application</span></span>|<span data-ttu-id="5b837-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b837-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b837-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b837-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b837-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5b837-120">Optional query parameters</span></span>
<span data-ttu-id="5b837-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b837-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5b837-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b837-122">Request headers</span></span>
|<span data-ttu-id="5b837-123">Header</span><span class="sxs-lookup"><span data-stu-id="5b837-123">Header</span></span>|<span data-ttu-id="5b837-124">Wert</span><span class="sxs-lookup"><span data-stu-id="5b837-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b837-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5b837-125">Authorization</span></span>|<span data-ttu-id="5b837-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5b837-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b837-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5b837-127">Accept</span></span>|<span data-ttu-id="5b837-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5b837-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b837-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b837-129">Request body</span></span>
<span data-ttu-id="5b837-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5b837-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b837-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b837-131">Response</span></span>
<span data-ttu-id="5b837-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5b837-132">If successful, this method returns a `200 OK` response code and [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b837-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b837-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b837-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b837-134">Request</span></span>
<span data-ttu-id="5b837-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b837-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5b837-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b837-136">Response</span></span>
<span data-ttu-id="5b837-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b837-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





