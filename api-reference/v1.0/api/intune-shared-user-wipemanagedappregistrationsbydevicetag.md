---
title: Aktion „wipeManagedAppRegistrationsByDeviceTag“
description: Diese Aktion stößt einen Zurücksetzungsvorgang für eine App-Registrierung mit dem jeweils angegebenen Gerätetag an.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5613a3e80acf8e6091cfb37c9e9818231854321b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851114"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="15ae2-103">Aktion „wipeManagedAppRegistrationsByDeviceTag“</span><span class="sxs-lookup"><span data-stu-id="15ae2-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>



> <span data-ttu-id="15ae2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="15ae2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15ae2-105">Diese Aktion stößt einen Zurücksetzungsvorgang für eine App-Registrierung mit dem jeweils angegebenen Gerätetag an.</span><span class="sxs-lookup"><span data-stu-id="15ae2-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15ae2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="15ae2-106">Prerequisites</span></span>
<span data-ttu-id="15ae2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15ae2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15ae2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15ae2-109">Permission type</span></span>|<span data-ttu-id="15ae2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15ae2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15ae2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15ae2-111">Delegated (work or school account)</span></span>| <span data-ttu-id="15ae2-112">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="15ae2-112">_varies by context_</span></span> |
| <span data-ttu-id="15ae2-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="15ae2-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="15ae2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ae2-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="15ae2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15ae2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15ae2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15ae2-116">Not supported.</span></span>|
|<span data-ttu-id="15ae2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15ae2-117">Application</span></span>|<span data-ttu-id="15ae2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15ae2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15ae2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15ae2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="15ae2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15ae2-120">Request headers</span></span>
|<span data-ttu-id="15ae2-121">Header</span><span class="sxs-lookup"><span data-stu-id="15ae2-121">Header</span></span>|<span data-ttu-id="15ae2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="15ae2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15ae2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15ae2-123">Authorization</span></span>|<span data-ttu-id="15ae2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="15ae2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15ae2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="15ae2-125">Accept</span></span>|<span data-ttu-id="15ae2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15ae2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15ae2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15ae2-127">Request body</span></span>
<span data-ttu-id="15ae2-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="15ae2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="15ae2-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="15ae2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="15ae2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15ae2-130">Property</span></span>|<span data-ttu-id="15ae2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="15ae2-131">Type</span></span>|<span data-ttu-id="15ae2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15ae2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15ae2-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="15ae2-133">deviceTag</span></span>|<span data-ttu-id="15ae2-134">String</span><span class="sxs-lookup"><span data-stu-id="15ae2-134">String</span></span>|<span data-ttu-id="15ae2-135">Gerätetag</span><span class="sxs-lookup"><span data-stu-id="15ae2-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="15ae2-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="15ae2-136">Response</span></span>
<span data-ttu-id="15ae2-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="15ae2-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="15ae2-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15ae2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="15ae2-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15ae2-139">Request</span></span>
<span data-ttu-id="15ae2-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15ae2-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="15ae2-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="15ae2-141">Response</span></span>
<span data-ttu-id="15ae2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15ae2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



