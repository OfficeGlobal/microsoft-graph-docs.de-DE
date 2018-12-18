---
title: ExportMobileConfig-Funktion
description: Exportiert die mobile Konfiguration
author: tfitzmac
ms.openlocfilehash: d6f663a729e45433c6f56f08ba02bb642749f5f5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350673"
---
# <a name="exportmobileconfig-function"></a><span data-ttu-id="fdbfd-103">ExportMobileConfig-Funktion</span><span class="sxs-lookup"><span data-stu-id="fdbfd-103">exportMobileConfig function</span></span>

> <span data-ttu-id="fdbfd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fdbfd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdbfd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fdbfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdbfd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fdbfd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdbfd-107">Exportiert die mobile Konfiguration</span><span class="sxs-lookup"><span data-stu-id="fdbfd-107">Exports the mobile configuration</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fdbfd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fdbfd-108">Prerequisites</span></span>
<span data-ttu-id="fdbfd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdbfd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdbfd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fdbfd-111">Permission type</span></span>|<span data-ttu-id="fdbfd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fdbfd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdbfd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fdbfd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdbfd-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdbfd-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fdbfd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fdbfd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdbfd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fdbfd-116">Not supported.</span></span>|
|<span data-ttu-id="fdbfd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fdbfd-117">Application</span></span>|<span data-ttu-id="fdbfd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fdbfd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdbfd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fdbfd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

## <a name="request-headers"></a><span data-ttu-id="fdbfd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fdbfd-120">Request headers</span></span>
|<span data-ttu-id="fdbfd-121">Header</span><span class="sxs-lookup"><span data-stu-id="fdbfd-121">Header</span></span>|<span data-ttu-id="fdbfd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fdbfd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdbfd-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fdbfd-123">Authorization</span></span>|<span data-ttu-id="fdbfd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fdbfd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdbfd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fdbfd-125">Accept</span></span>|<span data-ttu-id="fdbfd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdbfd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdbfd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fdbfd-127">Request body</span></span>
<span data-ttu-id="fdbfd-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fdbfd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdbfd-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="fdbfd-129">Response</span></span>
<span data-ttu-id="fdbfd-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fdbfd-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdbfd-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fdbfd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fdbfd-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fdbfd-132">Request</span></span>
<span data-ttu-id="fdbfd-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fdbfd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

### <a name="response"></a><span data-ttu-id="fdbfd-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fdbfd-134">Response</span></span>
<span data-ttu-id="fdbfd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fdbfd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Export Mobile Config value"
}
```





