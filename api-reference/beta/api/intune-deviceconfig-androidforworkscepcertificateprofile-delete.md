---
title: AndroidForWorkScepCertificateProfile löschen
description: Löscht eine AndroidForWorkScepCertificateProfile.
ms.openlocfilehash: d40ca1b1dedd2dd161352d5b9a22cae9606a7264
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064699"
---
# <a name="delete-androidforworkscepcertificateprofile"></a><span data-ttu-id="f09ba-103">AndroidForWorkScepCertificateProfile löschen</span><span class="sxs-lookup"><span data-stu-id="f09ba-103">Delete androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="f09ba-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f09ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f09ba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f09ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f09ba-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f09ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f09ba-107">Löscht eine [AndroidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f09ba-107">Deletes a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f09ba-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f09ba-108">Prerequisites</span></span>
<span data-ttu-id="f09ba-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f09ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f09ba-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f09ba-111">Permission type</span></span>|<span data-ttu-id="f09ba-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f09ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f09ba-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f09ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f09ba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f09ba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f09ba-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f09ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f09ba-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f09ba-116">Not supported.</span></span>|
|<span data-ttu-id="f09ba-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f09ba-117">Application</span></span>|<span data-ttu-id="f09ba-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f09ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f09ba-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f09ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f09ba-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f09ba-120">Request headers</span></span>
|<span data-ttu-id="f09ba-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f09ba-121">Header</span></span>|<span data-ttu-id="f09ba-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f09ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f09ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f09ba-123">Authorization</span></span>|<span data-ttu-id="f09ba-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f09ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f09ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f09ba-125">Accept</span></span>|<span data-ttu-id="f09ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f09ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f09ba-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f09ba-127">Request body</span></span>
<span data-ttu-id="f09ba-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f09ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f09ba-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f09ba-129">Response</span></span>
<span data-ttu-id="f09ba-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f09ba-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f09ba-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f09ba-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f09ba-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f09ba-132">Request</span></span>
<span data-ttu-id="f09ba-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f09ba-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f09ba-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f09ba-134">Response</span></span>
<span data-ttu-id="f09ba-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f09ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





