---
title: Abrufen von deviceManagementExchangeOnPremisesPolicy
description: Lesen Sie Eigenschaften und Beziehungen des DeviceManagementExchangeOnPremisesPolicy-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 48bd2a3d8ba9122cd529ceee977117210933add8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392850"
---
# <a name="get-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="deeef-103">Abrufen von deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="deeef-103">Get deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="deeef-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="deeef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="deeef-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="deeef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="deeef-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="deeef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deeef-107">Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="deeef-107">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="deeef-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="deeef-108">Prerequisites</span></span>
<span data-ttu-id="deeef-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="deeef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="deeef-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="deeef-111">Permission type</span></span>|<span data-ttu-id="deeef-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="deeef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="deeef-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="deeef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="deeef-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="deeef-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="deeef-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="deeef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="deeef-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="deeef-116">Not supported.</span></span>|
|<span data-ttu-id="deeef-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="deeef-117">Application</span></span>|<span data-ttu-id="deeef-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="deeef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="deeef-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="deeef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeOnPremisesPolicy
GET /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="deeef-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="deeef-120">Optional query parameters</span></span>
<span data-ttu-id="deeef-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="deeef-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="deeef-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="deeef-122">Request headers</span></span>
|<span data-ttu-id="deeef-123">Header</span><span class="sxs-lookup"><span data-stu-id="deeef-123">Header</span></span>|<span data-ttu-id="deeef-124">Wert</span><span class="sxs-lookup"><span data-stu-id="deeef-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="deeef-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="deeef-125">Authorization</span></span>|<span data-ttu-id="deeef-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="deeef-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="deeef-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="deeef-127">Accept</span></span>|<span data-ttu-id="deeef-128">application/json</span><span class="sxs-lookup"><span data-stu-id="deeef-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="deeef-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="deeef-129">Request body</span></span>
<span data-ttu-id="deeef-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="deeef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deeef-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="deeef-131">Response</span></span>
<span data-ttu-id="deeef-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="deeef-132">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="deeef-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="deeef-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="deeef-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="deeef-134">Request</span></span>
<span data-ttu-id="deeef-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="deeef-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
```

### <a name="response"></a><span data-ttu-id="deeef-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="deeef-136">Response</span></span>
<span data-ttu-id="deeef-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="deeef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 777

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
    "id": "16e76336-6336-16e7-3663-e7163663e716",
    "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
    "defaultAccessLevel": "allow",
    "accessRules": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
        "deviceClass": {
          "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
          "name": "Name value",
          "type": "model"
        },
        "accessLevel": "allow"
      }
    ],
    "knownDeviceClasses": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      }
    ]
  }
}
```




