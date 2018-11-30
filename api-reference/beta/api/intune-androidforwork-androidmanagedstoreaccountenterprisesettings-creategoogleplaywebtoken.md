---
title: CreateGooglePlayWebToken Aktion
description: Generiert ein Web-Token, das verwendet wird, in eine Komponente eingebettet werden.
ms.openlocfilehash: 26b58e5973063a74cac69d0bb70aa02adde7093f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063415"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="f5ed5-103">CreateGooglePlayWebToken Aktion</span><span class="sxs-lookup"><span data-stu-id="f5ed5-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="f5ed5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f5ed5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5ed5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5ed5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5ed5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f5ed5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5ed5-107">Generiert ein Web-Token, das verwendet wird, in eine Komponente eingebettet werden.</span><span class="sxs-lookup"><span data-stu-id="f5ed5-107">Generates a web token that is used in an embeddable component.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5ed5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f5ed5-108">Prerequisites</span></span>
<span data-ttu-id="f5ed5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5ed5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5ed5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5ed5-111">Permission type</span></span>|<span data-ttu-id="f5ed5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5ed5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5ed5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5ed5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5ed5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5ed5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5ed5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5ed5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5ed5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5ed5-116">Not supported.</span></span>|
|<span data-ttu-id="f5ed5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5ed5-117">Application</span></span>|<span data-ttu-id="f5ed5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5ed5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5ed5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5ed5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="f5ed5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5ed5-120">Request headers</span></span>
|<span data-ttu-id="f5ed5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f5ed5-121">Header</span></span>|<span data-ttu-id="f5ed5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f5ed5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5ed5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5ed5-123">Authorization</span></span>|<span data-ttu-id="f5ed5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f5ed5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5ed5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f5ed5-125">Accept</span></span>|<span data-ttu-id="f5ed5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5ed5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5ed5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5ed5-127">Request body</span></span>
<span data-ttu-id="f5ed5-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="f5ed5-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f5ed5-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="f5ed5-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f5ed5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f5ed5-130">Property</span></span>|<span data-ttu-id="f5ed5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f5ed5-131">Type</span></span>|<span data-ttu-id="f5ed5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5ed5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5ed5-133">parentUri</span><span class="sxs-lookup"><span data-stu-id="f5ed5-133">parentUri</span></span>|<span data-ttu-id="f5ed5-134">String</span><span class="sxs-lookup"><span data-stu-id="f5ed5-134">String</span></span>|<span data-ttu-id="f5ed5-135">Die Https-Pfad der Seite hosting der Komponente.</span><span class="sxs-lookup"><span data-stu-id="f5ed5-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="f5ed5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5ed5-136">Response</span></span>
<span data-ttu-id="f5ed5-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f5ed5-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5ed5-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5ed5-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5ed5-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5ed5-139">Request</span></span>
<span data-ttu-id="f5ed5-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5ed5-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="f5ed5-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5ed5-141">Response</span></span>
<span data-ttu-id="f5ed5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5ed5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```





