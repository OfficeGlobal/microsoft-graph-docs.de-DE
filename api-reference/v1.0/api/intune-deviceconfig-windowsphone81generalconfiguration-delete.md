---
title: windowsPhone81GeneralConfiguration löschen
description: Löscht ein windowsPhone81GeneralConfiguration-Objekt.
ms.openlocfilehash: e0093544835cc8b15a46d37e9080211a8955c683
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016157"
---
# <a name="delete-windowsphone81generalconfiguration"></a><span data-ttu-id="7cc05-103">windowsPhone81GeneralConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="7cc05-103">Delete windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="7cc05-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7cc05-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cc05-105">Löscht ein [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="7cc05-105">Deletes a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cc05-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7cc05-106">Prerequisites</span></span>
<span data-ttu-id="7cc05-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cc05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cc05-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7cc05-109">Permission type</span></span>|<span data-ttu-id="7cc05-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7cc05-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cc05-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7cc05-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7cc05-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cc05-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7cc05-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7cc05-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cc05-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7cc05-114">Not supported.</span></span>|
|<span data-ttu-id="7cc05-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7cc05-115">Application</span></span>|<span data-ttu-id="7cc05-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7cc05-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cc05-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cc05-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7cc05-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7cc05-118">Request headers</span></span>
|<span data-ttu-id="7cc05-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7cc05-119">Header</span></span>|<span data-ttu-id="7cc05-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7cc05-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cc05-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cc05-121">Authorization</span></span>|<span data-ttu-id="7cc05-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7cc05-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cc05-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7cc05-123">Accept</span></span>|<span data-ttu-id="7cc05-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7cc05-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cc05-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7cc05-125">Request body</span></span>
<span data-ttu-id="7cc05-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7cc05-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cc05-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cc05-127">Response</span></span>
<span data-ttu-id="7cc05-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7cc05-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7cc05-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7cc05-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cc05-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cc05-130">Request</span></span>
<span data-ttu-id="7cc05-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7cc05-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7cc05-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cc05-132">Response</span></span>
<span data-ttu-id="7cc05-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7cc05-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



