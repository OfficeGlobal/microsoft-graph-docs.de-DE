---
title: WindowsPhone81TrustedRootCertificate löschen
description: Löscht eine windowsPhone81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d98bec3f7dd3bdcde038a18d578c9066ed73d6a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852129"
---
# <a name="delete-windowsphone81trustedrootcertificate"></a><span data-ttu-id="15b8c-103">WindowsPhone81TrustedRootCertificate löschen</span><span class="sxs-lookup"><span data-stu-id="15b8c-103">Delete windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="15b8c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="15b8c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15b8c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15b8c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15b8c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="15b8c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15b8c-107">Löscht eine [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="15b8c-107">Deletes a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15b8c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="15b8c-108">Prerequisites</span></span>
<span data-ttu-id="15b8c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15b8c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15b8c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15b8c-111">Permission type</span></span>|<span data-ttu-id="15b8c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15b8c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15b8c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15b8c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15b8c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15b8c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15b8c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15b8c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15b8c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15b8c-116">Not supported.</span></span>|
|<span data-ttu-id="15b8c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15b8c-117">Application</span></span>|<span data-ttu-id="15b8c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15b8c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15b8c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15b8c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="15b8c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15b8c-120">Request headers</span></span>
|<span data-ttu-id="15b8c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="15b8c-121">Header</span></span>|<span data-ttu-id="15b8c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="15b8c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15b8c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15b8c-123">Authorization</span></span>|<span data-ttu-id="15b8c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="15b8c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15b8c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="15b8c-125">Accept</span></span>|<span data-ttu-id="15b8c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15b8c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15b8c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15b8c-127">Request body</span></span>
<span data-ttu-id="15b8c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="15b8c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15b8c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="15b8c-129">Response</span></span>
<span data-ttu-id="15b8c-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15b8c-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="15b8c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15b8c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="15b8c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15b8c-132">Request</span></span>
<span data-ttu-id="15b8c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15b8c-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

### <a name="response"></a><span data-ttu-id="15b8c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="15b8c-134">Response</span></span>
<span data-ttu-id="15b8c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15b8c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





