---
title: Erstellen von „userInstallStateSummary“
description: Diese Methode erstellt ein neues Objekt des Typs userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79481cb943b962484f9d216c0e32665afd440243
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139313"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="263f1-103">Erstellen von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="263f1-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="263f1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="263f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="263f1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="263f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="263f1-106">Diese Methode erstellt ein neues Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="263f1-106">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="263f1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="263f1-107">Prerequisites</span></span>
<span data-ttu-id="263f1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="263f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="263f1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="263f1-110">Permission type</span></span>|<span data-ttu-id="263f1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="263f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="263f1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="263f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="263f1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="263f1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="263f1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="263f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="263f1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="263f1-115">Not supported.</span></span>|
|<span data-ttu-id="263f1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="263f1-116">Application</span></span>|<span data-ttu-id="263f1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="263f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="263f1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="263f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="263f1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="263f1-119">Request headers</span></span>
|<span data-ttu-id="263f1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="263f1-120">Header</span></span>|<span data-ttu-id="263f1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="263f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="263f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="263f1-122">Authorization</span></span>|<span data-ttu-id="263f1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="263f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="263f1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="263f1-124">Accept</span></span>|<span data-ttu-id="263f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="263f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="263f1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="263f1-126">Request body</span></span>
<span data-ttu-id="263f1-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „userInstallStateSummary“ an.</span><span class="sxs-lookup"><span data-stu-id="263f1-127">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="263f1-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „userInstallStateSummary“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="263f1-128">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="263f1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="263f1-129">Property</span></span>|<span data-ttu-id="263f1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="263f1-130">Type</span></span>|<span data-ttu-id="263f1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="263f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="263f1-132">id</span><span class="sxs-lookup"><span data-stu-id="263f1-132">id</span></span>|<span data-ttu-id="263f1-133">String</span><span class="sxs-lookup"><span data-stu-id="263f1-133">String</span></span>|<span data-ttu-id="263f1-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="263f1-134">Key of the entity.</span></span>|
|<span data-ttu-id="263f1-135">userName</span><span class="sxs-lookup"><span data-stu-id="263f1-135">userName</span></span>|<span data-ttu-id="263f1-136">String</span><span class="sxs-lookup"><span data-stu-id="263f1-136">String</span></span>|<span data-ttu-id="263f1-137">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="263f1-137">User name.</span></span>|
|<span data-ttu-id="263f1-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="263f1-138">installedDeviceCount</span></span>|<span data-ttu-id="263f1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="263f1-139">Int32</span></span>|<span data-ttu-id="263f1-140">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="263f1-140">Installed Device Count.</span></span>|
|<span data-ttu-id="263f1-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="263f1-141">failedDeviceCount</span></span>|<span data-ttu-id="263f1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="263f1-142">Int32</span></span>|<span data-ttu-id="263f1-143">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="263f1-143">Failed Device Count.</span></span>|
|<span data-ttu-id="263f1-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="263f1-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="263f1-145">Int32</span><span class="sxs-lookup"><span data-stu-id="263f1-145">Int32</span></span>|<span data-ttu-id="263f1-146">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="263f1-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="263f1-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="263f1-147">Response</span></span>
<span data-ttu-id="263f1-148">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="263f1-148">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="263f1-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="263f1-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="263f1-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="263f1-150">Request</span></span>
<span data-ttu-id="263f1-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="263f1-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="263f1-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="263f1-152">Response</span></span>
<span data-ttu-id="263f1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="263f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```




