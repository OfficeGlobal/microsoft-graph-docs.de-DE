---
title: windowsInformationProtectionNetworkLearningSummary löschen
description: Löscht ein windowsInformationProtectionNetworkLearningSummary-Objekt.
ms.openlocfilehash: 098230894f1aa60becada7c301650034940d7e46
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060703"
---
# <a name="delete-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="23015-103">windowsInformationProtectionNetworkLearningSummary löschen</span><span class="sxs-lookup"><span data-stu-id="23015-103">Delete windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="23015-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23015-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23015-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23015-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23015-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="23015-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23015-107">Löscht ein [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="23015-107">Deletes a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23015-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="23015-108">Prerequisites</span></span>
<span data-ttu-id="23015-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23015-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23015-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23015-111">Permission type</span></span>|<span data-ttu-id="23015-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23015-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23015-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23015-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23015-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23015-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="23015-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23015-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23015-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23015-116">Not supported.</span></span>|
|<span data-ttu-id="23015-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23015-117">Application</span></span>|<span data-ttu-id="23015-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23015-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23015-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23015-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="23015-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23015-120">Request headers</span></span>
|<span data-ttu-id="23015-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="23015-121">Header</span></span>|<span data-ttu-id="23015-122">Wert</span><span class="sxs-lookup"><span data-stu-id="23015-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23015-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23015-123">Authorization</span></span>|<span data-ttu-id="23015-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="23015-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23015-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23015-125">Accept</span></span>|<span data-ttu-id="23015-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23015-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23015-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23015-127">Request body</span></span>
<span data-ttu-id="23015-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="23015-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23015-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="23015-129">Response</span></span>
<span data-ttu-id="23015-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23015-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="23015-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23015-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="23015-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23015-132">Request</span></span>
<span data-ttu-id="23015-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="23015-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="23015-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="23015-134">Response</span></span>
<span data-ttu-id="23015-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23015-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





