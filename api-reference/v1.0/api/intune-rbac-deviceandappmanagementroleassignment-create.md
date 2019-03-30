---
title: DeviceAndAppManagementRoleAssignment erstellen
description: Erstellen eines neuen deviceAndAppManagementRoleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04797f0674ff824d2881ffdfa2500d3d3e7c79bc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989063"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="b8c62-103">DeviceAndAppManagementRoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="b8c62-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="b8c62-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b8c62-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8c62-105">Erstellen eines neuen [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b8c62-105">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8c62-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b8c62-106">Prerequisites</span></span>
<span data-ttu-id="b8c62-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8c62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8c62-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8c62-109">Permission type</span></span>|<span data-ttu-id="b8c62-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8c62-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8c62-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8c62-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8c62-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8c62-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b8c62-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8c62-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8c62-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8c62-114">Not supported.</span></span>|
|<span data-ttu-id="b8c62-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8c62-115">Application</span></span>|<span data-ttu-id="b8c62-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8c62-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8c62-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8c62-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="b8c62-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8c62-118">Request headers</span></span>
|<span data-ttu-id="b8c62-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b8c62-119">Header</span></span>|<span data-ttu-id="b8c62-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b8c62-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8c62-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8c62-121">Authorization</span></span>|<span data-ttu-id="b8c62-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b8c62-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8c62-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b8c62-123">Accept</span></span>|<span data-ttu-id="b8c62-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b8c62-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8c62-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8c62-125">Request body</span></span>
<span data-ttu-id="b8c62-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceAndAppManagementRoleAssignment an.</span><span class="sxs-lookup"><span data-stu-id="b8c62-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="b8c62-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceAndAppManagementRoleAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="b8c62-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="b8c62-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8c62-128">Property</span></span>|<span data-ttu-id="b8c62-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b8c62-129">Type</span></span>|<span data-ttu-id="b8c62-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8c62-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8c62-131">id</span><span class="sxs-lookup"><span data-stu-id="b8c62-131">id</span></span>|<span data-ttu-id="b8c62-132">String</span><span class="sxs-lookup"><span data-stu-id="b8c62-132">String</span></span>|<span data-ttu-id="b8c62-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b8c62-133">Key of the entity.</span></span> <span data-ttu-id="b8c62-134">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="b8c62-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="b8c62-135">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b8c62-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b8c62-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b8c62-136">displayName</span></span>|<span data-ttu-id="b8c62-137">String</span><span class="sxs-lookup"><span data-stu-id="b8c62-137">String</span></span>|<span data-ttu-id="b8c62-138">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="b8c62-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="b8c62-139">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b8c62-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b8c62-140">description</span><span class="sxs-lookup"><span data-stu-id="b8c62-140">description</span></span>|<span data-ttu-id="b8c62-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8c62-141">String</span></span>|<span data-ttu-id="b8c62-142">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="b8c62-142">Description of the Role Assignment.</span></span> <span data-ttu-id="b8c62-143">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b8c62-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b8c62-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b8c62-144">resourceScopes</span></span>|<span data-ttu-id="b8c62-145">String collection</span><span class="sxs-lookup"><span data-stu-id="b8c62-145">String collection</span></span>|<span data-ttu-id="b8c62-146">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="b8c62-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b8c62-147">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8c62-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="b8c62-148">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b8c62-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b8c62-149">members</span><span class="sxs-lookup"><span data-stu-id="b8c62-149">members</span></span>|<span data-ttu-id="b8c62-150">String collection</span><span class="sxs-lookup"><span data-stu-id="b8c62-150">String collection</span></span>|<span data-ttu-id="b8c62-151">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="b8c62-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="b8c62-152">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8c62-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b8c62-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8c62-153">Response</span></span>
<span data-ttu-id="b8c62-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b8c62-154">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8c62-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8c62-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8c62-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8c62-156">Request</span></span>
<span data-ttu-id="b8c62-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8c62-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b8c62-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8c62-158">Response</span></span>
<span data-ttu-id="b8c62-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8c62-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



