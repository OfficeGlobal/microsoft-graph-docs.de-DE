---
title: Erstellen von „userInstallStateSummary“
description: Diese Methode erstellt ein neues Objekt des Typs userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94b74d6619f3975b8dbdb08c96d58b54c0419392
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260137"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="eac09-103">Erstellen von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="eac09-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="eac09-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="eac09-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eac09-105">Diese Methode erstellt ein neues Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="eac09-105">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eac09-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eac09-106">Prerequisites</span></span>
<span data-ttu-id="eac09-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="eac09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eac09-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eac09-109">Permission type</span></span>|<span data-ttu-id="eac09-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eac09-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eac09-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eac09-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eac09-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eac09-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eac09-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eac09-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eac09-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eac09-114">Not supported.</span></span>|
|<span data-ttu-id="eac09-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eac09-115">Application</span></span>|<span data-ttu-id="eac09-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eac09-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eac09-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eac09-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="eac09-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eac09-118">Request headers</span></span>
|<span data-ttu-id="eac09-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eac09-119">Header</span></span>|<span data-ttu-id="eac09-120">Wert</span><span class="sxs-lookup"><span data-stu-id="eac09-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eac09-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eac09-121">Authorization</span></span>|<span data-ttu-id="eac09-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eac09-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eac09-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eac09-123">Accept</span></span>|<span data-ttu-id="eac09-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eac09-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eac09-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eac09-125">Request body</span></span>
<span data-ttu-id="eac09-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „userInstallStateSummary“ an.</span><span class="sxs-lookup"><span data-stu-id="eac09-126">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="eac09-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „userInstallStateSummary“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="eac09-127">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="eac09-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eac09-128">Property</span></span>|<span data-ttu-id="eac09-129">Typ</span><span class="sxs-lookup"><span data-stu-id="eac09-129">Type</span></span>|<span data-ttu-id="eac09-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eac09-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eac09-131">id</span><span class="sxs-lookup"><span data-stu-id="eac09-131">id</span></span>|<span data-ttu-id="eac09-132">String</span><span class="sxs-lookup"><span data-stu-id="eac09-132">String</span></span>|<span data-ttu-id="eac09-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="eac09-133">Key of the entity.</span></span>|
|<span data-ttu-id="eac09-134">userName</span><span class="sxs-lookup"><span data-stu-id="eac09-134">userName</span></span>|<span data-ttu-id="eac09-135">String</span><span class="sxs-lookup"><span data-stu-id="eac09-135">String</span></span>|<span data-ttu-id="eac09-136">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="eac09-136">User name.</span></span>|
|<span data-ttu-id="eac09-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eac09-137">installedDeviceCount</span></span>|<span data-ttu-id="eac09-138">Int32</span><span class="sxs-lookup"><span data-stu-id="eac09-138">Int32</span></span>|<span data-ttu-id="eac09-139">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="eac09-139">Installed Device Count.</span></span>|
|<span data-ttu-id="eac09-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eac09-140">failedDeviceCount</span></span>|<span data-ttu-id="eac09-141">Int32</span><span class="sxs-lookup"><span data-stu-id="eac09-141">Int32</span></span>|<span data-ttu-id="eac09-142">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="eac09-142">Failed Device Count.</span></span>|
|<span data-ttu-id="eac09-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eac09-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="eac09-144">Int32</span><span class="sxs-lookup"><span data-stu-id="eac09-144">Int32</span></span>|<span data-ttu-id="eac09-145">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="eac09-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="eac09-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="eac09-146">Response</span></span>
<span data-ttu-id="eac09-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eac09-147">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eac09-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eac09-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="eac09-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eac09-149">Request</span></span>
<span data-ttu-id="eac09-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eac09-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
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

### <a name="response"></a><span data-ttu-id="eac09-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="eac09-151">Response</span></span>
<span data-ttu-id="eac09-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eac09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



