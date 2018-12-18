---
title: Aktion „completeSignup“
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 8a5d0635f575e6ab7b577b4cd0d20fd441cc5e4a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350302"
---
# <a name="completesignup-action"></a><span data-ttu-id="6d710-103">Aktion „completeSignup“</span><span class="sxs-lookup"><span data-stu-id="6d710-103">completeSignup action</span></span>

> <span data-ttu-id="6d710-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6d710-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d710-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6d710-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d710-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6d710-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d710-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6d710-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6d710-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6d710-108">Prerequisites</span></span>
<span data-ttu-id="6d710-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d710-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d710-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d710-111">Permission type</span></span>|<span data-ttu-id="6d710-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d710-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d710-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d710-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d710-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d710-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d710-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d710-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d710-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d710-116">Not supported.</span></span>|
|<span data-ttu-id="6d710-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d710-117">Application</span></span>|<span data-ttu-id="6d710-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d710-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d710-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d710-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/completeSignup
```

## <a name="request-headers"></a><span data-ttu-id="6d710-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d710-120">Request headers</span></span>
|<span data-ttu-id="6d710-121">Header</span><span class="sxs-lookup"><span data-stu-id="6d710-121">Header</span></span>|<span data-ttu-id="6d710-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6d710-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d710-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6d710-123">Authorization</span></span>|<span data-ttu-id="6d710-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6d710-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d710-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6d710-125">Accept</span></span>|<span data-ttu-id="6d710-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d710-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d710-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d710-127">Request body</span></span>
<span data-ttu-id="6d710-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="6d710-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6d710-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="6d710-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6d710-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d710-130">Property</span></span>|<span data-ttu-id="6d710-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6d710-131">Type</span></span>|<span data-ttu-id="6d710-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d710-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d710-133">enterpriseToken</span><span class="sxs-lookup"><span data-stu-id="6d710-133">enterpriseToken</span></span>|<span data-ttu-id="6d710-134">String</span><span class="sxs-lookup"><span data-stu-id="6d710-134">String</span></span>|<span data-ttu-id="6d710-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6d710-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6d710-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d710-136">Response</span></span>
<span data-ttu-id="6d710-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="6d710-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6d710-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d710-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d710-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d710-139">Request</span></span>
<span data-ttu-id="6d710-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6d710-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/completeSignup

Content-type: application/json
Content-length: 51

{
  "enterpriseToken": "Enterprise Token value"
}
```

### <a name="response"></a><span data-ttu-id="6d710-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d710-141">Response</span></span>
<span data-ttu-id="6d710-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d710-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





