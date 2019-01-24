---
title: SetAndroidDeviceOwnerFullyManagedEnrollmentState Aktion
description: Legt die AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled auf den angegebenen Wert fest.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 840c4a3781a993648abb77ad46f1967073c1b3e8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430227"
---
# <a name="setandroiddeviceownerfullymanagedenrollmentstate-action"></a><span data-ttu-id="5fbfd-103">SetAndroidDeviceOwnerFullyManagedEnrollmentState Aktion</span><span class="sxs-lookup"><span data-stu-id="5fbfd-103">setAndroidDeviceOwnerFullyManagedEnrollmentState action</span></span>

> <span data-ttu-id="5fbfd-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5fbfd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5fbfd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5fbfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5fbfd-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5fbfd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fbfd-107">Legt die AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled auf den angegebenen Wert fest.</span><span class="sxs-lookup"><span data-stu-id="5fbfd-107">Sets the AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled to the given value.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fbfd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5fbfd-108">Prerequisites</span></span>
<span data-ttu-id="5fbfd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5fbfd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5fbfd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5fbfd-111">Permission type</span></span>|<span data-ttu-id="5fbfd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5fbfd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fbfd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5fbfd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5fbfd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fbfd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5fbfd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5fbfd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fbfd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fbfd-116">Not supported.</span></span>|
|<span data-ttu-id="5fbfd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5fbfd-117">Application</span></span>|<span data-ttu-id="5fbfd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fbfd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fbfd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fbfd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState
```

## <a name="request-headers"></a><span data-ttu-id="5fbfd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5fbfd-120">Request headers</span></span>
|<span data-ttu-id="5fbfd-121">Header</span><span class="sxs-lookup"><span data-stu-id="5fbfd-121">Header</span></span>|<span data-ttu-id="5fbfd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5fbfd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fbfd-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5fbfd-123">Authorization</span></span>|<span data-ttu-id="5fbfd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5fbfd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fbfd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5fbfd-125">Accept</span></span>|<span data-ttu-id="5fbfd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5fbfd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fbfd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5fbfd-127">Request body</span></span>
<span data-ttu-id="5fbfd-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="5fbfd-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5fbfd-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="5fbfd-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5fbfd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5fbfd-130">Property</span></span>|<span data-ttu-id="5fbfd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5fbfd-131">Type</span></span>|<span data-ttu-id="5fbfd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5fbfd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fbfd-133">aktiviert</span><span class="sxs-lookup"><span data-stu-id="5fbfd-133">enabled</span></span>|<span data-ttu-id="5fbfd-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbfd-134">Boolean</span></span>|<span data-ttu-id="5fbfd-135">Der Wert auf AndroidDeviceOwnerFullyManagedEnrollmentEnabled festgelegt werden soll.</span><span class="sxs-lookup"><span data-stu-id="5fbfd-135">The value to set AndroidDeviceOwnerFullyManagedEnrollmentEnabled to.</span></span>|



## <a name="response"></a><span data-ttu-id="5fbfd-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fbfd-136">Response</span></span>
<span data-ttu-id="5fbfd-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="5fbfd-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5fbfd-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5fbfd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fbfd-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fbfd-139">Request</span></span>
<span data-ttu-id="5fbfd-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5fbfd-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/setAndroidDeviceOwnerFullyManagedEnrollmentState

Content-type: application/json
Content-length: 23

{
  "enabled": true
}
```

### <a name="response"></a><span data-ttu-id="5fbfd-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fbfd-141">Response</span></span>
<span data-ttu-id="5fbfd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5fbfd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



