---
title: windows10CustomConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des windows10CustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f20bf7f9bccd6b342273ec83651abb541691bef4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852073"
---
# <a name="get-windows10customconfiguration"></a><span data-ttu-id="10852-103">windows10CustomConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="10852-103">Get windows10CustomConfiguration</span></span>

> <span data-ttu-id="10852-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="10852-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10852-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10852-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10852-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="10852-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10852-107">Lesen von Eigenschaften und Beziehungen des [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="10852-107">Read properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10852-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="10852-108">Prerequisites</span></span>
<span data-ttu-id="10852-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10852-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10852-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10852-111">Permission type</span></span>|<span data-ttu-id="10852-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10852-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10852-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10852-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10852-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="10852-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="10852-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10852-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10852-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10852-116">Not supported.</span></span>|
|<span data-ttu-id="10852-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10852-117">Application</span></span>|<span data-ttu-id="10852-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10852-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10852-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10852-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10852-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="10852-120">Optional query parameters</span></span>
<span data-ttu-id="10852-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="10852-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="10852-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10852-122">Request headers</span></span>
|<span data-ttu-id="10852-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="10852-123">Header</span></span>|<span data-ttu-id="10852-124">Wert</span><span class="sxs-lookup"><span data-stu-id="10852-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10852-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="10852-125">Authorization</span></span>|<span data-ttu-id="10852-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="10852-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10852-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="10852-127">Accept</span></span>|<span data-ttu-id="10852-128">application/json</span><span class="sxs-lookup"><span data-stu-id="10852-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10852-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10852-129">Request body</span></span>
<span data-ttu-id="10852-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="10852-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10852-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="10852-131">Response</span></span>
<span data-ttu-id="10852-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10852-132">If successful, this method returns a `200 OK` response code and [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10852-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10852-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="10852-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10852-134">Request</span></span>
<span data-ttu-id="10852-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10852-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="10852-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="10852-136">Response</span></span>
<span data-ttu-id="10852-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10852-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 727

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
    "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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





