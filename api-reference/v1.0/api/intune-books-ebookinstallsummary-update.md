---
title: eBookInstallSummary aktualisieren
description: Aktualisieren der Eigenschaften des eBookInstallSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f9927dc4c757a83afa02f101815536b1b81d81e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988854"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="fcb7a-103">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fcb7a-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="fcb7a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcb7a-105">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-105">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcb7a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fcb7a-106">Prerequisites</span></span>
<span data-ttu-id="fcb7a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcb7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcb7a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fcb7a-109">Permission type</span></span>|<span data-ttu-id="fcb7a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fcb7a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcb7a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fcb7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fcb7a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcb7a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fcb7a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fcb7a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcb7a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fcb7a-114">Not supported.</span></span>|
|<span data-ttu-id="fcb7a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fcb7a-115">Application</span></span>|<span data-ttu-id="fcb7a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fcb7a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcb7a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fcb7a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="fcb7a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fcb7a-118">Request headers</span></span>
|<span data-ttu-id="fcb7a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fcb7a-119">Header</span></span>|<span data-ttu-id="fcb7a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="fcb7a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcb7a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcb7a-121">Authorization</span></span>|<span data-ttu-id="fcb7a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fcb7a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcb7a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fcb7a-123">Accept</span></span>|<span data-ttu-id="fcb7a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fcb7a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcb7a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fcb7a-125">Request body</span></span>
<span data-ttu-id="fcb7a-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-126">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="fcb7a-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-127">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="fcb7a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fcb7a-128">Property</span></span>|<span data-ttu-id="fcb7a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="fcb7a-129">Type</span></span>|<span data-ttu-id="fcb7a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fcb7a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcb7a-131">id</span><span class="sxs-lookup"><span data-stu-id="fcb7a-131">id</span></span>|<span data-ttu-id="fcb7a-132">String</span><span class="sxs-lookup"><span data-stu-id="fcb7a-132">String</span></span>|<span data-ttu-id="fcb7a-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fcb7a-133">Key of the entity.</span></span>|
|<span data-ttu-id="fcb7a-134">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fcb7a-134">installedDeviceCount</span></span>|<span data-ttu-id="fcb7a-135">Int32</span><span class="sxs-lookup"><span data-stu-id="fcb7a-135">Int32</span></span>|<span data-ttu-id="fcb7a-136">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-136">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="fcb7a-137">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fcb7a-137">failedDeviceCount</span></span>|<span data-ttu-id="fcb7a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="fcb7a-138">Int32</span></span>|<span data-ttu-id="fcb7a-139">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-139">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="fcb7a-140">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fcb7a-140">notInstalledDeviceCount</span></span>|<span data-ttu-id="fcb7a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="fcb7a-141">Int32</span></span>|<span data-ttu-id="fcb7a-142">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-142">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="fcb7a-143">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="fcb7a-143">installedUserCount</span></span>|<span data-ttu-id="fcb7a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="fcb7a-144">Int32</span></span>|<span data-ttu-id="fcb7a-145">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-145">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="fcb7a-146">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="fcb7a-146">failedUserCount</span></span>|<span data-ttu-id="fcb7a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="fcb7a-147">Int32</span></span>|<span data-ttu-id="fcb7a-148">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-148">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="fcb7a-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="fcb7a-149">notInstalledUserCount</span></span>|<span data-ttu-id="fcb7a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="fcb7a-150">Int32</span></span>|<span data-ttu-id="fcb7a-151">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-151">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="fcb7a-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="fcb7a-152">Response</span></span>
<span data-ttu-id="fcb7a-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-153">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcb7a-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fcb7a-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcb7a-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fcb7a-155">Request</span></span>
<span data-ttu-id="fcb7a-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="fcb7a-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="fcb7a-157">Response</span></span>
<span data-ttu-id="fcb7a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fcb7a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```



