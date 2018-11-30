---
title: Aktion „wipeManagedAppRegistrationsByDeviceTag“
description: Diese Aktion stößt einen Zurücksetzungsvorgang für eine App-Registrierung mit dem jeweils angegebenen Gerätetag an.
ms.openlocfilehash: 8f31e7f4217ff638654e3e6d780830b9540e1872
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060704"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="5221d-103">Aktion „wipeManagedAppRegistrationsByDeviceTag“</span><span class="sxs-lookup"><span data-stu-id="5221d-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="5221d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5221d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5221d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5221d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5221d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5221d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5221d-107">Diese Aktion stößt einen Zurücksetzungsvorgang für eine App-Registrierung mit dem jeweils angegebenen Gerätetag an.</span><span class="sxs-lookup"><span data-stu-id="5221d-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5221d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5221d-108">Prerequisites</span></span>

<span data-ttu-id="5221d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5221d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5221d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5221d-111">Permission type</span></span>|<span data-ttu-id="5221d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5221d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5221d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5221d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5221d-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="5221d-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="5221d-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5221d-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5221d-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5221d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5221d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5221d-117">Not supported.</span></span>|
|<span data-ttu-id="5221d-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5221d-118">Application</span></span>|<span data-ttu-id="5221d-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5221d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5221d-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5221d-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="5221d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5221d-121">Request headers</span></span>

|<span data-ttu-id="5221d-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5221d-122">Header</span></span>|<span data-ttu-id="5221d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="5221d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5221d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5221d-124">Authorization</span></span>|<span data-ttu-id="5221d-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5221d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5221d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5221d-126">Accept</span></span>|<span data-ttu-id="5221d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5221d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5221d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5221d-128">Request body</span></span>

<span data-ttu-id="5221d-129">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="5221d-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5221d-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="5221d-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5221d-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5221d-131">Property</span></span>|<span data-ttu-id="5221d-132">Typ</span><span class="sxs-lookup"><span data-stu-id="5221d-132">Type</span></span>|<span data-ttu-id="5221d-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5221d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5221d-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="5221d-134">deviceTag</span></span>|<span data-ttu-id="5221d-135">String</span><span class="sxs-lookup"><span data-stu-id="5221d-135">String</span></span>|<span data-ttu-id="5221d-136">Gerätetag</span><span class="sxs-lookup"><span data-stu-id="5221d-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="5221d-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="5221d-137">Response</span></span>

<span data-ttu-id="5221d-138">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="5221d-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5221d-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5221d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="5221d-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5221d-140">Request</span></span>

<span data-ttu-id="5221d-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5221d-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="5221d-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="5221d-142">Response</span></span>

<span data-ttu-id="5221d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5221d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






