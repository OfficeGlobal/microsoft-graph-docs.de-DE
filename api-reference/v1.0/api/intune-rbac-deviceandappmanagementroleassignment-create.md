---
title: DeviceAndAppManagementRoleAssignment erstellen
description: Erstellen eines neuen deviceAndAppManagementRoleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0d5c47d764caa567ecdffd84c75e3f8db6957364
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884196"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="8fe18-103">DeviceAndAppManagementRoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="8fe18-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="8fe18-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8fe18-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fe18-105">Erstellen eines neuen [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8fe18-105">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8fe18-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8fe18-106">Prerequisites</span></span>
<span data-ttu-id="8fe18-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fe18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fe18-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8fe18-109">Permission type</span></span>|<span data-ttu-id="8fe18-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8fe18-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fe18-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8fe18-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8fe18-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fe18-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8fe18-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8fe18-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fe18-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fe18-114">Not supported.</span></span>|
|<span data-ttu-id="8fe18-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8fe18-115">Application</span></span>|<span data-ttu-id="8fe18-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fe18-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fe18-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fe18-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="8fe18-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8fe18-118">Request headers</span></span>
|<span data-ttu-id="8fe18-119">Header</span><span class="sxs-lookup"><span data-stu-id="8fe18-119">Header</span></span>|<span data-ttu-id="8fe18-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8fe18-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fe18-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fe18-121">Authorization</span></span>|<span data-ttu-id="8fe18-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8fe18-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fe18-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8fe18-123">Accept</span></span>|<span data-ttu-id="8fe18-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8fe18-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fe18-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8fe18-125">Request body</span></span>
<span data-ttu-id="8fe18-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceAndAppManagementRoleAssignment an.</span><span class="sxs-lookup"><span data-stu-id="8fe18-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="8fe18-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceAndAppManagementRoleAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="8fe18-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="8fe18-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8fe18-128">Property</span></span>|<span data-ttu-id="8fe18-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8fe18-129">Type</span></span>|<span data-ttu-id="8fe18-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fe18-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fe18-131">id</span><span class="sxs-lookup"><span data-stu-id="8fe18-131">id</span></span>|<span data-ttu-id="8fe18-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fe18-132">String</span></span>|<span data-ttu-id="8fe18-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8fe18-133">Key of the entity.</span></span> <span data-ttu-id="8fe18-134">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="8fe18-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="8fe18-135">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8fe18-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="8fe18-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8fe18-136">displayName</span></span>|<span data-ttu-id="8fe18-137">String</span><span class="sxs-lookup"><span data-stu-id="8fe18-137">String</span></span>|<span data-ttu-id="8fe18-138">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="8fe18-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="8fe18-139">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8fe18-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="8fe18-140">description</span><span class="sxs-lookup"><span data-stu-id="8fe18-140">description</span></span>|<span data-ttu-id="8fe18-141">String</span><span class="sxs-lookup"><span data-stu-id="8fe18-141">String</span></span>|<span data-ttu-id="8fe18-142">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="8fe18-142">Description of the Role Assignment.</span></span> <span data-ttu-id="8fe18-143">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8fe18-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="8fe18-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="8fe18-144">resourceScopes</span></span>|<span data-ttu-id="8fe18-145">String collection</span><span class="sxs-lookup"><span data-stu-id="8fe18-145">String collection</span></span>|<span data-ttu-id="8fe18-146">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="8fe18-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="8fe18-147">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8fe18-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="8fe18-148">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8fe18-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="8fe18-149">Elemente</span><span class="sxs-lookup"><span data-stu-id="8fe18-149">members</span></span>|<span data-ttu-id="8fe18-150">String collection</span><span class="sxs-lookup"><span data-stu-id="8fe18-150">String collection</span></span>|<span data-ttu-id="8fe18-151">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="8fe18-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="8fe18-152">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8fe18-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="8fe18-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fe18-153">Response</span></span>
<span data-ttu-id="8fe18-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8fe18-154">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fe18-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8fe18-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="8fe18-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fe18-156">Request</span></span>
<span data-ttu-id="8fe18-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8fe18-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8fe18-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fe18-158">Response</span></span>
<span data-ttu-id="8fe18-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8fe18-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



