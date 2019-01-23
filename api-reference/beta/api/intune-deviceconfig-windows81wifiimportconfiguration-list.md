---
title: Liste windows81WifiImportConfigurations
description: Listeneigenschaften und Beziehungen der windows81WifiImportConfiguration-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6fd5e17f9bb36939e97c068f2e9f8c54de05e909
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416258"
---
# <a name="list-windows81wifiimportconfigurations"></a><span data-ttu-id="539a3-103">Liste windows81WifiImportConfigurations</span><span class="sxs-lookup"><span data-stu-id="539a3-103">List windows81WifiImportConfigurations</span></span>

> <span data-ttu-id="539a3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="539a3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="539a3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="539a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="539a3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="539a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="539a3-107">Listeneigenschaften und Beziehungen der [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="539a3-107">List properties and relationships of the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="539a3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="539a3-108">Prerequisites</span></span>
<span data-ttu-id="539a3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="539a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="539a3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="539a3-111">Permission type</span></span>|<span data-ttu-id="539a3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="539a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="539a3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="539a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="539a3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="539a3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="539a3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="539a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="539a3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="539a3-116">Not supported.</span></span>|
|<span data-ttu-id="539a3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="539a3-117">Application</span></span>|<span data-ttu-id="539a3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="539a3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="539a3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="539a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="539a3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="539a3-120">Request headers</span></span>
|<span data-ttu-id="539a3-121">Header</span><span class="sxs-lookup"><span data-stu-id="539a3-121">Header</span></span>|<span data-ttu-id="539a3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="539a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="539a3-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="539a3-123">Authorization</span></span>|<span data-ttu-id="539a3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="539a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="539a3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="539a3-125">Accept</span></span>|<span data-ttu-id="539a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="539a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="539a3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="539a3-127">Request body</span></span>
<span data-ttu-id="539a3-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="539a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="539a3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="539a3-129">Response</span></span>
<span data-ttu-id="539a3-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="539a3-130">If successful, this method returns a `200 OK` response code and a collection of [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="539a3-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="539a3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="539a3-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="539a3-132">Request</span></span>
<span data-ttu-id="539a3-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="539a3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="539a3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="539a3-134">Response</span></span>
<span data-ttu-id="539a3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="539a3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 642

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
      "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "payloadFileName": "Payload File Name value",
      "profileName": "Profile Name value",
      "payload": "cGF5bG9hZA=="
    }
  ]
}
```




