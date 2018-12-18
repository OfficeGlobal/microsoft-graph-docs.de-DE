---
title: windows10SecureAssessmentConfiguration löschen
description: Löscht ein windows10SecureAssessmentConfiguration-Objekt.
author: tfitzmac
ms.openlocfilehash: 861848bc7525d47e6eb274a985a69bd2595cf0bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325200"
---
# <a name="delete-windows10secureassessmentconfiguration"></a><span data-ttu-id="ff727-103">windows10SecureAssessmentConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="ff727-103">Delete windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="ff727-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff727-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff727-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff727-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff727-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff727-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff727-107">Löscht ein [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="ff727-107">Deletes a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff727-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ff727-108">Prerequisites</span></span>
<span data-ttu-id="ff727-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff727-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff727-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff727-111">Permission type</span></span>|<span data-ttu-id="ff727-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff727-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff727-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff727-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff727-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff727-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff727-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff727-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff727-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff727-116">Not supported.</span></span>|
|<span data-ttu-id="ff727-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff727-117">Application</span></span>|<span data-ttu-id="ff727-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff727-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff727-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff727-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ff727-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff727-120">Request headers</span></span>
|<span data-ttu-id="ff727-121">Header</span><span class="sxs-lookup"><span data-stu-id="ff727-121">Header</span></span>|<span data-ttu-id="ff727-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ff727-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff727-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ff727-123">Authorization</span></span>|<span data-ttu-id="ff727-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ff727-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff727-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff727-125">Accept</span></span>|<span data-ttu-id="ff727-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff727-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff727-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff727-127">Request body</span></span>
<span data-ttu-id="ff727-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ff727-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff727-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff727-129">Response</span></span>
<span data-ttu-id="ff727-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff727-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff727-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff727-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff727-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff727-132">Request</span></span>
<span data-ttu-id="ff727-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff727-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ff727-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff727-134">Response</span></span>
<span data-ttu-id="ff727-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff727-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





