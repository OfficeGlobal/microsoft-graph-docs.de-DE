---
title: Abrufen von windowsManagementApp
description: Lesen Sie Eigenschaften und Beziehungen des WindowsManagementApp-Objekts.
ms.openlocfilehash: b5a614a4bfdf68d94bef266f6013bade627cc7f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057902"
---
# <a name="get-windowsmanagementapp"></a><span data-ttu-id="112bf-103">Abrufen von windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="112bf-103">Get windowsManagementApp</span></span>

> <span data-ttu-id="112bf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="112bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="112bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="112bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="112bf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="112bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="112bf-107">Lesen Sie Eigenschaften und Beziehungen des [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="112bf-107">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="112bf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="112bf-108">Prerequisites</span></span>
<span data-ttu-id="112bf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="112bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="112bf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="112bf-111">Permission type</span></span>|<span data-ttu-id="112bf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="112bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="112bf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="112bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="112bf-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="112bf-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="112bf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="112bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="112bf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="112bf-116">Not supported.</span></span>|
|<span data-ttu-id="112bf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="112bf-117">Application</span></span>|<span data-ttu-id="112bf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="112bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="112bf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="112bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp
```

## <a name="optional-query-parameters"></a><span data-ttu-id="112bf-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="112bf-120">Optional query parameters</span></span>
<span data-ttu-id="112bf-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="112bf-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="112bf-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="112bf-122">Request headers</span></span>
|<span data-ttu-id="112bf-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="112bf-123">Header</span></span>|<span data-ttu-id="112bf-124">Wert</span><span class="sxs-lookup"><span data-stu-id="112bf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="112bf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="112bf-125">Authorization</span></span>|<span data-ttu-id="112bf-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="112bf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="112bf-127">Accept</span><span class="sxs-lookup"><span data-stu-id="112bf-127">Accept</span></span>|<span data-ttu-id="112bf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="112bf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="112bf-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="112bf-129">Request body</span></span>
<span data-ttu-id="112bf-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="112bf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="112bf-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="112bf-131">Response</span></span>
<span data-ttu-id="112bf-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="112bf-132">If successful, this method returns a `200 OK` response code and [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="112bf-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="112bf-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="112bf-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="112bf-134">Request</span></span>
<span data-ttu-id="112bf-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="112bf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
```

### <a name="response"></a><span data-ttu-id="112bf-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="112bf-136">Response</span></span>
<span data-ttu-id="112bf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="112bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagementApp",
    "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
    "availableVersion": "Available Version value"
  }
}
```





