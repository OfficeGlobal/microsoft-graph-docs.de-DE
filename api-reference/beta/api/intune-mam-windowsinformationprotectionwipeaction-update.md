---
title: WindowsInformationProtectionWipeAction aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsInformationProtectionWipeAction-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f49b79d6ebd12d81332613c646623d68dc0b09a2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430090"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="ef62d-103">WindowsInformationProtectionWipeAction aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ef62d-103">Update windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="ef62d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ef62d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ef62d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ef62d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef62d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ef62d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef62d-107">Aktualisieren Sie die Eigenschaften eines [WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ef62d-107">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef62d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ef62d-108">Prerequisites</span></span>
<span data-ttu-id="ef62d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ef62d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ef62d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef62d-111">Permission type</span></span>|<span data-ttu-id="ef62d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef62d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef62d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef62d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef62d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef62d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef62d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef62d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef62d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef62d-116">Not supported.</span></span>|
|<span data-ttu-id="ef62d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef62d-117">Application</span></span>|<span data-ttu-id="ef62d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef62d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef62d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef62d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="ef62d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef62d-120">Request headers</span></span>
|<span data-ttu-id="ef62d-121">Header</span><span class="sxs-lookup"><span data-stu-id="ef62d-121">Header</span></span>|<span data-ttu-id="ef62d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ef62d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef62d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ef62d-123">Authorization</span></span>|<span data-ttu-id="ef62d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ef62d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef62d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ef62d-125">Accept</span></span>|<span data-ttu-id="ef62d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef62d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef62d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef62d-127">Request body</span></span>
<span data-ttu-id="ef62d-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ef62d-128">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="ef62d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="ef62d-129">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="ef62d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ef62d-130">Property</span></span>|<span data-ttu-id="ef62d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ef62d-131">Type</span></span>|<span data-ttu-id="ef62d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef62d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef62d-133">id</span><span class="sxs-lookup"><span data-stu-id="ef62d-133">id</span></span>|<span data-ttu-id="ef62d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef62d-134">String</span></span>|<span data-ttu-id="ef62d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ef62d-135">Key of the entity.</span></span>|
|<span data-ttu-id="ef62d-136">status</span><span class="sxs-lookup"><span data-stu-id="ef62d-136">status</span></span>|[<span data-ttu-id="ef62d-137">actionState</span><span class="sxs-lookup"><span data-stu-id="ef62d-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ef62d-138">Wischen Sie Aktionsstatus.</span><span class="sxs-lookup"><span data-stu-id="ef62d-138">Wipe action status.</span></span> <span data-ttu-id="ef62d-139">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ef62d-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ef62d-140">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="ef62d-140">targetedUserId</span></span>|<span data-ttu-id="ef62d-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef62d-141">String</span></span>|<span data-ttu-id="ef62d-142">Die Benutzer-ID, die diese Aktion Remotegerätzurücksetzung darstellt.</span><span class="sxs-lookup"><span data-stu-id="ef62d-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="ef62d-143">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="ef62d-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="ef62d-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef62d-144">String</span></span>|<span data-ttu-id="ef62d-145">Die DeviceRegistrationId diese Aktion Remotegerätzurücksetzung darstellt.</span><span class="sxs-lookup"><span data-stu-id="ef62d-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="ef62d-146">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="ef62d-146">targetedDeviceName</span></span>|<span data-ttu-id="ef62d-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef62d-147">String</span></span>|<span data-ttu-id="ef62d-148">Gezielte Gerätename.</span><span class="sxs-lookup"><span data-stu-id="ef62d-148">Targeted device name.</span></span>|
|<span data-ttu-id="ef62d-149">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="ef62d-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="ef62d-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef62d-150">String</span></span>|<span data-ttu-id="ef62d-151">Zielgerät Mac-Adresse.</span><span class="sxs-lookup"><span data-stu-id="ef62d-151">Targeted device Mac address.</span></span>|



## <a name="response"></a><span data-ttu-id="ef62d-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef62d-152">Response</span></span>
<span data-ttu-id="ef62d-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ef62d-153">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef62d-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef62d-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef62d-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef62d-155">Request</span></span>
<span data-ttu-id="ef62d-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef62d-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
Content-type: application/json
Content-length: 350

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value"
}
```

### <a name="response"></a><span data-ttu-id="ef62d-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef62d-157">Response</span></span>
<span data-ttu-id="ef62d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef62d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 399

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "2620a996-a996-2620-96a9-202696a92026",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value"
}
```




