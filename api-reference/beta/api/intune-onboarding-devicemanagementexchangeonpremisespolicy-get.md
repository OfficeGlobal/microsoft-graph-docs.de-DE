---
title: Abrufen von deviceManagementExchangeOnPremisesPolicy
description: Lesen Sie Eigenschaften und Beziehungen des DeviceManagementExchangeOnPremisesPolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a587e369fc99f1f6b3a0ec7478271e1669a19aba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832942"
---
# <a name="get-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="ba88c-103">Abrufen von deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="ba88c-103">Get deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="ba88c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ba88c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba88c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ba88c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba88c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ba88c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba88c-107">Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ba88c-107">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ba88c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ba88c-108">Prerequisites</span></span>
<span data-ttu-id="ba88c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba88c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba88c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ba88c-111">Permission type</span></span>|<span data-ttu-id="ba88c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ba88c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba88c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ba88c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba88c-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba88c-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ba88c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ba88c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba88c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba88c-116">Not supported.</span></span>|
|<span data-ttu-id="ba88c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba88c-117">Application</span></span>|<span data-ttu-id="ba88c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba88c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba88c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba88c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeOnPremisesPolicy
GET /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba88c-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ba88c-120">Optional query parameters</span></span>
<span data-ttu-id="ba88c-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ba88c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ba88c-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ba88c-122">Request headers</span></span>
|<span data-ttu-id="ba88c-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ba88c-123">Header</span></span>|<span data-ttu-id="ba88c-124">Wert</span><span class="sxs-lookup"><span data-stu-id="ba88c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba88c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba88c-125">Authorization</span></span>|<span data-ttu-id="ba88c-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ba88c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba88c-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ba88c-127">Accept</span></span>|<span data-ttu-id="ba88c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ba88c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba88c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ba88c-129">Request body</span></span>
<span data-ttu-id="ba88c-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ba88c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba88c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba88c-131">Response</span></span>
<span data-ttu-id="ba88c-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ba88c-132">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba88c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ba88c-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ba88c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba88c-134">Request</span></span>
<span data-ttu-id="ba88c-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ba88c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
```

### <a name="response"></a><span data-ttu-id="ba88c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba88c-136">Response</span></span>
<span data-ttu-id="ba88c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ba88c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





