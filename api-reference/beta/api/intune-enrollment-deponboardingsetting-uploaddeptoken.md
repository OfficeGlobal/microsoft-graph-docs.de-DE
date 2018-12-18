---
title: UploadDepToken Aktion
description: Lädt ein neues Gerät Registrierung Programm Token hoch
author: tfitzmac
ms.openlocfilehash: 6fc303afa5efb5fab312732c95545b73004660a0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330646"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="b1c12-103">UploadDepToken Aktion</span><span class="sxs-lookup"><span data-stu-id="b1c12-103">uploadDepToken action</span></span>

> <span data-ttu-id="b1c12-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b1c12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1c12-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1c12-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1c12-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b1c12-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1c12-107">Lädt ein neues Gerät Registrierung Programm Token hoch</span><span class="sxs-lookup"><span data-stu-id="b1c12-107">Uploads a new Device Enrollment Program token</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1c12-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b1c12-108">Prerequisites</span></span>
<span data-ttu-id="b1c12-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1c12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1c12-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1c12-111">Permission type</span></span>|<span data-ttu-id="b1c12-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1c12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1c12-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1c12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1c12-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1c12-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b1c12-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1c12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1c12-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1c12-116">Not supported.</span></span>|
|<span data-ttu-id="b1c12-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1c12-117">Application</span></span>|<span data-ttu-id="b1c12-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1c12-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1c12-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1c12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="b1c12-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1c12-120">Request headers</span></span>
|<span data-ttu-id="b1c12-121">Header</span><span class="sxs-lookup"><span data-stu-id="b1c12-121">Header</span></span>|<span data-ttu-id="b1c12-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b1c12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1c12-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b1c12-123">Authorization</span></span>|<span data-ttu-id="b1c12-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b1c12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1c12-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1c12-125">Accept</span></span>|<span data-ttu-id="b1c12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1c12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1c12-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1c12-127">Request body</span></span>
<span data-ttu-id="b1c12-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="b1c12-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b1c12-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="b1c12-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b1c12-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b1c12-130">Property</span></span>|<span data-ttu-id="b1c12-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b1c12-131">Type</span></span>|<span data-ttu-id="b1c12-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1c12-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1c12-133">appleId</span><span class="sxs-lookup"><span data-stu-id="b1c12-133">appleId</span></span>|<span data-ttu-id="b1c12-134">String</span><span class="sxs-lookup"><span data-stu-id="b1c12-134">String</span></span>|<span data-ttu-id="b1c12-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b1c12-135">Not yet documented</span></span>|
|<span data-ttu-id="b1c12-136">depToken</span><span class="sxs-lookup"><span data-stu-id="b1c12-136">depToken</span></span>|<span data-ttu-id="b1c12-137">String</span><span class="sxs-lookup"><span data-stu-id="b1c12-137">String</span></span>|<span data-ttu-id="b1c12-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b1c12-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b1c12-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1c12-139">Response</span></span>
<span data-ttu-id="b1c12-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="b1c12-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b1c12-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1c12-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1c12-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1c12-142">Request</span></span>
<span data-ttu-id="b1c12-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1c12-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="b1c12-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1c12-144">Response</span></span>
<span data-ttu-id="b1c12-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1c12-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





