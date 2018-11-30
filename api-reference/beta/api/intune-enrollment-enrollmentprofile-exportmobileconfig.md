---
title: ExportMobileConfig-Funktion
description: Exportiert die mobile Konfiguration
ms.openlocfilehash: 44af58f78ed3f26b5ecb00c86dc6ffb675e86162
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065515"
---
# <a name="exportmobileconfig-function"></a><span data-ttu-id="79753-103">ExportMobileConfig-Funktion</span><span class="sxs-lookup"><span data-stu-id="79753-103">exportMobileConfig function</span></span>

> <span data-ttu-id="79753-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="79753-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79753-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79753-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79753-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="79753-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79753-107">Exportiert die mobile Konfiguration</span><span class="sxs-lookup"><span data-stu-id="79753-107">Exports the mobile configuration</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79753-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="79753-108">Prerequisites</span></span>
<span data-ttu-id="79753-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79753-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79753-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79753-111">Permission type</span></span>|<span data-ttu-id="79753-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79753-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79753-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79753-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79753-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="79753-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="79753-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79753-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79753-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79753-116">Not supported.</span></span>|
|<span data-ttu-id="79753-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79753-117">Application</span></span>|<span data-ttu-id="79753-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79753-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79753-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79753-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

## <a name="request-headers"></a><span data-ttu-id="79753-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79753-120">Request headers</span></span>
|<span data-ttu-id="79753-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="79753-121">Header</span></span>|<span data-ttu-id="79753-122">Wert</span><span class="sxs-lookup"><span data-stu-id="79753-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79753-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79753-123">Authorization</span></span>|<span data-ttu-id="79753-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="79753-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79753-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79753-125">Accept</span></span>|<span data-ttu-id="79753-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79753-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79753-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79753-127">Request body</span></span>
<span data-ttu-id="79753-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="79753-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79753-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="79753-129">Response</span></span>
<span data-ttu-id="79753-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="79753-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79753-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79753-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="79753-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79753-132">Request</span></span>
<span data-ttu-id="79753-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79753-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

### <a name="response"></a><span data-ttu-id="79753-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="79753-134">Response</span></span>
<span data-ttu-id="79753-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79753-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Export Mobile Config value"
}
```





