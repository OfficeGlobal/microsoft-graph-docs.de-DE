---
title: Aktualisieren von „userInstallStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fabf57da88e740eea1ac43dd7c24e2d6884e5bbc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969855"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="7c209-103">Aktualisieren von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="7c209-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="7c209-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7c209-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c209-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7c209-105">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c209-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7c209-106">Prerequisites</span></span>
<span data-ttu-id="7c209-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c209-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c209-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c209-109">Permission type</span></span>|<span data-ttu-id="7c209-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c209-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c209-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c209-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c209-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c209-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7c209-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c209-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c209-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c209-114">Not supported.</span></span>|
|<span data-ttu-id="7c209-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c209-115">Application</span></span>|<span data-ttu-id="7c209-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c209-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c209-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c209-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="7c209-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c209-118">Request headers</span></span>
|<span data-ttu-id="7c209-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7c209-119">Header</span></span>|<span data-ttu-id="7c209-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7c209-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c209-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c209-121">Authorization</span></span>|<span data-ttu-id="7c209-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7c209-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c209-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7c209-123">Accept</span></span>|<span data-ttu-id="7c209-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7c209-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c209-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c209-125">Request body</span></span>
<span data-ttu-id="7c209-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="7c209-126">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="7c209-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7c209-127">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="7c209-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c209-128">Property</span></span>|<span data-ttu-id="7c209-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7c209-129">Type</span></span>|<span data-ttu-id="7c209-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c209-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c209-131">id</span><span class="sxs-lookup"><span data-stu-id="7c209-131">id</span></span>|<span data-ttu-id="7c209-132">String</span><span class="sxs-lookup"><span data-stu-id="7c209-132">String</span></span>|<span data-ttu-id="7c209-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7c209-133">Key of the entity.</span></span>|
|<span data-ttu-id="7c209-134">userName</span><span class="sxs-lookup"><span data-stu-id="7c209-134">userName</span></span>|<span data-ttu-id="7c209-135">String</span><span class="sxs-lookup"><span data-stu-id="7c209-135">String</span></span>|<span data-ttu-id="7c209-136">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="7c209-136">User name.</span></span>|
|<span data-ttu-id="7c209-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c209-137">installedDeviceCount</span></span>|<span data-ttu-id="7c209-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7c209-138">Int32</span></span>|<span data-ttu-id="7c209-139">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="7c209-139">Installed Device Count.</span></span>|
|<span data-ttu-id="7c209-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c209-140">failedDeviceCount</span></span>|<span data-ttu-id="7c209-141">Int32</span><span class="sxs-lookup"><span data-stu-id="7c209-141">Int32</span></span>|<span data-ttu-id="7c209-142">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="7c209-142">Failed Device Count.</span></span>|
|<span data-ttu-id="7c209-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c209-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="7c209-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7c209-144">Int32</span></span>|<span data-ttu-id="7c209-145">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="7c209-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="7c209-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c209-146">Response</span></span>
<span data-ttu-id="7c209-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7c209-147">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c209-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c209-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c209-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c209-149">Request</span></span>
<span data-ttu-id="7c209-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c209-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="7c209-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c209-151">Response</span></span>
<span data-ttu-id="7c209-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c209-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



