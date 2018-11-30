---
title: Aktion „assign“
description: Noch nicht dokumentiert
ms.openlocfilehash: 615f8b760b908de1eb69aae2cdfbdf2eafdd64e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018853"
---
# <a name="assign-action"></a><span data-ttu-id="bc176-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="bc176-103">assign action</span></span>

> <span data-ttu-id="bc176-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bc176-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc176-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bc176-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc176-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bc176-106">Prerequisites</span></span>
<span data-ttu-id="bc176-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc176-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc176-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc176-109">Permission type</span></span>|<span data-ttu-id="bc176-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc176-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc176-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc176-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bc176-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc176-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc176-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc176-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc176-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc176-114">Not supported.</span></span>|
|<span data-ttu-id="bc176-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc176-115">Application</span></span>|<span data-ttu-id="bc176-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc176-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc176-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc176-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="bc176-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc176-118">Request headers</span></span>
|<span data-ttu-id="bc176-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bc176-119">Header</span></span>|<span data-ttu-id="bc176-120">Wert</span><span class="sxs-lookup"><span data-stu-id="bc176-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc176-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc176-121">Authorization</span></span>|<span data-ttu-id="bc176-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc176-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc176-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bc176-123">Accept</span></span>|<span data-ttu-id="bc176-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bc176-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc176-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc176-125">Request body</span></span>
<span data-ttu-id="bc176-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="bc176-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bc176-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="bc176-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bc176-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc176-128">Property</span></span>|<span data-ttu-id="bc176-129">Typ</span><span class="sxs-lookup"><span data-stu-id="bc176-129">Type</span></span>|<span data-ttu-id="bc176-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc176-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc176-131">assignments</span><span class="sxs-lookup"><span data-stu-id="bc176-131">assignments</span></span>|<span data-ttu-id="bc176-132">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bc176-132">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="bc176-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bc176-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bc176-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc176-134">Response</span></span>
<span data-ttu-id="bc176-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bc176-135">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc176-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc176-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc176-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc176-137">Request</span></span>
<span data-ttu-id="bc176-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc176-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 277

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="bc176-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc176-139">Response</span></span>
<span data-ttu-id="bc176-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc176-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



