---
title: WindowsInformationProtectionDeviceRegistration löschen
description: Löscht eine windowsInformationProtectionDeviceRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f78f0db97dcf9ce2906e76b8bd402aac6b4d5998
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963807"
---
# <a name="delete-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="2aea1-103">WindowsInformationProtectionDeviceRegistration löschen</span><span class="sxs-lookup"><span data-stu-id="2aea1-103">Delete windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="2aea1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2aea1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2aea1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2aea1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2aea1-106">Löscht eine [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span><span class="sxs-lookup"><span data-stu-id="2aea1-106">Deletes a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2aea1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2aea1-107">Prerequisites</span></span>
<span data-ttu-id="2aea1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2aea1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2aea1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2aea1-110">Permission type</span></span>|<span data-ttu-id="2aea1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2aea1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2aea1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2aea1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2aea1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aea1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2aea1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2aea1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2aea1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2aea1-115">Not supported.</span></span>|
|<span data-ttu-id="2aea1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2aea1-116">Application</span></span>|<span data-ttu-id="2aea1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2aea1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2aea1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2aea1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="2aea1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2aea1-119">Request headers</span></span>
|<span data-ttu-id="2aea1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2aea1-120">Header</span></span>|<span data-ttu-id="2aea1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2aea1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2aea1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2aea1-122">Authorization</span></span>|<span data-ttu-id="2aea1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2aea1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2aea1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2aea1-124">Accept</span></span>|<span data-ttu-id="2aea1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2aea1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2aea1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2aea1-126">Request body</span></span>
<span data-ttu-id="2aea1-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2aea1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2aea1-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2aea1-128">Response</span></span>
<span data-ttu-id="2aea1-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2aea1-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2aea1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2aea1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2aea1-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2aea1-131">Request</span></span>
<span data-ttu-id="2aea1-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2aea1-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

### <a name="response"></a><span data-ttu-id="2aea1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2aea1-133">Response</span></span>
<span data-ttu-id="2aea1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2aea1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




