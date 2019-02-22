---
title: managedMobileApp löschen
description: Löscht ein managedMobileApp-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e45e28f8fb365dd2996b4a70659457c0a1eb325
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162601"
---
# <a name="delete-managedmobileapp"></a><span data-ttu-id="f3b66-103">managedMobileApp löschen</span><span class="sxs-lookup"><span data-stu-id="f3b66-103">Delete managedMobileApp</span></span>

> <span data-ttu-id="f3b66-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3b66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3b66-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f3b66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3b66-106">Löscht ein [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="f3b66-106">Deletes a [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3b66-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f3b66-107">Prerequisites</span></span>
<span data-ttu-id="f3b66-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f3b66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f3b66-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3b66-110">Permission type</span></span>|<span data-ttu-id="f3b66-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3b66-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3b66-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3b66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3b66-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3b66-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3b66-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3b66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3b66-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3b66-115">Not supported.</span></span>|
|<span data-ttu-id="f3b66-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3b66-116">Application</span></span>|<span data-ttu-id="f3b66-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3b66-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3b66-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3b66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
DELETE /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
DELETE /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
DELETE /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f3b66-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3b66-119">Request headers</span></span>
|<span data-ttu-id="f3b66-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f3b66-120">Header</span></span>|<span data-ttu-id="f3b66-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f3b66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3b66-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3b66-122">Authorization</span></span>|<span data-ttu-id="f3b66-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f3b66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3b66-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f3b66-124">Accept</span></span>|<span data-ttu-id="f3b66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3b66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3b66-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3b66-126">Request body</span></span>
<span data-ttu-id="f3b66-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f3b66-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3b66-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3b66-128">Response</span></span>
<span data-ttu-id="f3b66-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3b66-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f3b66-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3b66-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3b66-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3b66-131">Request</span></span>
<span data-ttu-id="f3b66-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3b66-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="f3b66-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3b66-133">Response</span></span>
<span data-ttu-id="f3b66-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3b66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




