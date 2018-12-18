---
title: AutopilotDeviceStream-Funktion
description: Erstellen Sie eine Anforderung Upload mit Autopilot Gerät Stream darin.
author: tfitzmac
ms.openlocfilehash: fd7f2b1c452d69f772d2a3d80cf9a68ba8139df1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307133"
---
# <a name="autopilotdevicestream-function"></a><span data-ttu-id="dd759-103">AutopilotDeviceStream-Funktion</span><span class="sxs-lookup"><span data-stu-id="dd759-103">autopilotDeviceStream function</span></span>

> <span data-ttu-id="dd759-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd759-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd759-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd759-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd759-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dd759-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd759-107">Erstellen Sie eine Anforderung Upload mit Autopilot Gerät Stream darin.</span><span class="sxs-lookup"><span data-stu-id="dd759-107">Create a upload request with autopilot device stream in it.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd759-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dd759-108">Prerequisites</span></span>
<span data-ttu-id="dd759-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd759-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd759-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd759-111">Permission type</span></span>|<span data-ttu-id="dd759-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd759-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd759-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd759-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd759-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd759-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dd759-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd759-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd759-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd759-116">Not supported.</span></span>|
|<span data-ttu-id="dd759-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd759-117">Application</span></span>|<span data-ttu-id="dd759-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd759-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd759-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd759-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="dd759-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd759-120">Request headers</span></span>
|<span data-ttu-id="dd759-121">Header</span><span class="sxs-lookup"><span data-stu-id="dd759-121">Header</span></span>|<span data-ttu-id="dd759-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dd759-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd759-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="dd759-123">Authorization</span></span>|<span data-ttu-id="dd759-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dd759-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd759-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd759-125">Accept</span></span>|<span data-ttu-id="dd759-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd759-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd759-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd759-127">Request body</span></span>
<span data-ttu-id="dd759-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dd759-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd759-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd759-129">Response</span></span>
<span data-ttu-id="dd759-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dd759-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd759-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd759-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd759-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd759-132">Request</span></span>
<span data-ttu-id="dd759-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd759-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="dd759-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd759-134">Response</span></span>
<span data-ttu-id="dd759-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd759-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```





