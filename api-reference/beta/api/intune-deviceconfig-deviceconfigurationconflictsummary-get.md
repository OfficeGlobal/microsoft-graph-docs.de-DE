---
title: Abrufen von deviceConfigurationConflictSummary
description: Lesen Sie Eigenschaften und Beziehungen des DeviceConfigurationConflictSummary-Objekts.
author: tfitzmac
ms.openlocfilehash: b5f38a613d10ebfd610bc8bf71bfaa30243d0d5b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333971"
---
# <a name="get-deviceconfigurationconflictsummary"></a><span data-ttu-id="34b64-103">Abrufen von deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="34b64-103">Get deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="34b64-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34b64-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34b64-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34b64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34b64-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="34b64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34b64-107">Lesen Sie Eigenschaften und Beziehungen des [DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="34b64-107">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34b64-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="34b64-108">Prerequisites</span></span>
<span data-ttu-id="34b64-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34b64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34b64-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34b64-111">Permission type</span></span>|<span data-ttu-id="34b64-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34b64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34b64-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34b64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34b64-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34b64-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="34b64-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34b64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34b64-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34b64-116">Not supported.</span></span>|
|<span data-ttu-id="34b64-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34b64-117">Application</span></span>|<span data-ttu-id="34b64-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34b64-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34b64-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34b64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34b64-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="34b64-120">Optional query parameters</span></span>
<span data-ttu-id="34b64-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="34b64-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="34b64-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34b64-122">Request headers</span></span>
|<span data-ttu-id="34b64-123">Header</span><span class="sxs-lookup"><span data-stu-id="34b64-123">Header</span></span>|<span data-ttu-id="34b64-124">Wert</span><span class="sxs-lookup"><span data-stu-id="34b64-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34b64-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="34b64-125">Authorization</span></span>|<span data-ttu-id="34b64-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="34b64-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34b64-127">Accept</span><span class="sxs-lookup"><span data-stu-id="34b64-127">Accept</span></span>|<span data-ttu-id="34b64-128">application/json</span><span class="sxs-lookup"><span data-stu-id="34b64-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34b64-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34b64-129">Request body</span></span>
<span data-ttu-id="34b64-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="34b64-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34b64-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="34b64-131">Response</span></span>
<span data-ttu-id="34b64-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="34b64-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34b64-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34b64-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="34b64-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34b64-134">Request</span></span>
<span data-ttu-id="34b64-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34b64-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

### <a name="response"></a><span data-ttu-id="34b64-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="34b64-136">Response</span></span>
<span data-ttu-id="34b64-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34b64-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 455

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
    "conflictingDeviceConfigurations": [
      {
        "@odata.type": "microsoft.graph.settingSource",
        "id": "Id value",
        "displayName": "Display Name value"
      }
    ],
    "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
    "contributingSettings": [
      "Contributing Settings value"
    ],
    "deviceCheckinsImpacted": 6
  }
}
```





