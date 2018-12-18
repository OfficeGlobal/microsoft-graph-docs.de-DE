---
title: Abrufen von „androidCustomConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs androidCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 27c057af115e48621a46218c6743962adef73312
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321924"
---
# <a name="get-androidcustomconfiguration"></a><span data-ttu-id="c5e79-103">Abrufen von „androidCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="c5e79-103">Get androidCustomConfiguration</span></span>

> <span data-ttu-id="c5e79-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c5e79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5e79-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5e79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5e79-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c5e79-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5e79-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5e79-107">Read properties and relationships of the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5e79-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c5e79-108">Prerequisites</span></span>
<span data-ttu-id="c5e79-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5e79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5e79-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5e79-111">Permission type</span></span>|<span data-ttu-id="c5e79-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5e79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5e79-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5e79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5e79-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5e79-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c5e79-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5e79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5e79-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5e79-116">Not supported.</span></span>|
|<span data-ttu-id="c5e79-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5e79-117">Application</span></span>|<span data-ttu-id="c5e79-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5e79-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5e79-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5e79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5e79-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c5e79-120">Optional query parameters</span></span>
<span data-ttu-id="c5e79-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c5e79-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c5e79-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5e79-122">Request headers</span></span>
|<span data-ttu-id="c5e79-123">Header</span><span class="sxs-lookup"><span data-stu-id="c5e79-123">Header</span></span>|<span data-ttu-id="c5e79-124">Wert</span><span class="sxs-lookup"><span data-stu-id="c5e79-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5e79-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c5e79-125">Authorization</span></span>|<span data-ttu-id="c5e79-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c5e79-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5e79-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c5e79-127">Accept</span></span>|<span data-ttu-id="c5e79-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c5e79-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5e79-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5e79-129">Request body</span></span>
<span data-ttu-id="c5e79-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c5e79-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5e79-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5e79-131">Response</span></span>
<span data-ttu-id="c5e79-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c5e79-132">If successful, this method returns a `200 OK` response code and [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5e79-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5e79-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5e79-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5e79-134">Request</span></span>
<span data-ttu-id="c5e79-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5e79-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c5e79-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5e79-136">Response</span></span>
<span data-ttu-id="c5e79-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5e79-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 725

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCustomConfiguration",
    "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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
}
```





