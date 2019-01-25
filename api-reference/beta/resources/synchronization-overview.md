---
title: Azure AD-Synchronisierung API (Übersicht)
description: ') können Sie die Erstellung automatisieren Wartung und Entfernen von Identitäten in cloud (Software als Dienst oder SaaS) Anwendungen wie Ablage, Vertriebs, ServiceNow und vieles mehr. Die Synchronisierung-APIs können in Microsoft Graph Sie programmgesteuert verwalten Identität Synchronisierung einschließlich:'
localization_priority: Normal
ms.openlocfilehash: ed994b8204fdee38f558da499259538e85eacd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529558"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="a49f8-104">Azure AD-Synchronisierung API (Übersicht)</span><span class="sxs-lookup"><span data-stu-id="a49f8-104">Azure AD synchronization API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a49f8-105">Azure Active Directory (AD Azure) Identität Synchronisierung (auch als "Bereitstellung" bezeichnet) können Sie die Erstellung, Wartung und Entfernen von Identitäten in der Cloud (Software als Dienst oder SaaS) automatisieren Applications wie Ablage, Vertriebs, ServiceNow, und vieles mehr.</span><span class="sxs-lookup"><span data-stu-id="a49f8-105">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="a49f8-106">Die Synchronisierung-APIs können in Microsoft Graph Sie programmgesteuert verwalten Identität Synchronisierung einschließlich:</span><span class="sxs-lookup"><span data-stu-id="a49f8-106">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="a49f8-107">Erstellen Sie, starten Sie und beenden Sie der Aufträge für die Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="a49f8-107">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="a49f8-108">Vornehmen von Änderungen an der Synchronisierungsschema für Aufträge</span><span class="sxs-lookup"><span data-stu-id="a49f8-108">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="a49f8-109">Überprüfen Sie den aktuellen Synchronisierungsstatus</span><span class="sxs-lookup"><span data-stu-id="a49f8-109">Verify the current synchronization status</span></span> 

<span data-ttu-id="a49f8-110">Weitere Informationen zur Synchronisierung in Azure Active Directory finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="a49f8-110">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="a49f8-111">Automatisieren der Benutzer bereitstellen und entziehen für SaaS Clientanwendungen mit Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a49f8-111">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="a49f8-112">Verwalten von Benutzerkonto für Enterprise-apps im Azure-Portal-Bereitstellung</span><span class="sxs-lookup"><span data-stu-id="a49f8-112">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="a49f8-113">Sie können auch die API im [Graph-Explorer](https://developer.microsoft.com/graph/graph-explorer) in einer Beispiel-Mandanten oder Ihre eigene Mandanten versuchen.</span><span class="sxs-lookup"><span data-stu-id="a49f8-113">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="a49f8-114">Synchronisierungsauftrag</span><span class="sxs-lookup"><span data-stu-id="a49f8-114">Synchronization job</span></span>

<span data-ttu-id="a49f8-115">Aufträge für die Synchronisierung ausführen Synchronisierung von in regelmäßigen Abständen im Hintergrund ausgeführt, abrufen, damit die Änderungen in ein Verzeichnis und pushen von in ein anderes Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="a49f8-115">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="a49f8-116">Der Synchronisierungsauftrag ist immer spezifisch für eine bestimmte Instanz einer Anwendung in Ihrem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a49f8-116">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="a49f8-117">Im Rahmen der Synchronisierung Einrichtung müssen Sie die Autorisierung zum Lesen und Schreiben von Objekten in Ihrem Zielverzeichnis übergeben, und passen den Auftrag Synchronisierungsschema.</span><span class="sxs-lookup"><span data-stu-id="a49f8-117">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="a49f8-118">Weitere Informationen finden Sie unter [Synchronisierungsauftrag](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-118">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="a49f8-119">Synchronisierungsschema</span><span class="sxs-lookup"><span data-stu-id="a49f8-119">Synchronization schema</span></span>

<span data-ttu-id="a49f8-120">Das Synchronisierungsschema definiert, welche Objekte werden synchronisiert, und wie diese synchronisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a49f8-120">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="a49f8-121">Das Synchronisierungsschema enthält die meisten der Setupinformationen für einen bestimmten Synchronisierungsauftrag.</span><span class="sxs-lookup"><span data-stu-id="a49f8-121">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="a49f8-122">Sie werden in der Regel anpassen einiger [Attribut Zuordnungen](synchronization-attributemapping.md)oder Hinzufügen eines [Gültigkeitsbereichs Filter](synchronization-filter.md) , um nur die Objekte zu synchronisieren, die eine bestimmte Bedingung erfüllen.</span><span class="sxs-lookup"><span data-stu-id="a49f8-122">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="a49f8-123">Das Synchronisierungsschema umfasst die folgenden Komponenten:</span><span class="sxs-lookup"><span data-stu-id="a49f8-123">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="a49f8-124">Directory-Definitionen</span><span class="sxs-lookup"><span data-stu-id="a49f8-124">Directory definitions</span></span>
- <span data-ttu-id="a49f8-125">Synchronisierungsregeln</span><span class="sxs-lookup"><span data-stu-id="a49f8-125">Synchronization rules</span></span>
- <span data-ttu-id="a49f8-126">Objekt-Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="a49f8-126">Object mappings</span></span>

<span data-ttu-id="a49f8-127">Weitere Informationen finden Sie unter [Synchronisierungsschema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-127">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="a49f8-128">Synchronisierung-Vorlage</span><span class="sxs-lookup"><span data-stu-id="a49f8-128">Synchronization template</span></span>

<span data-ttu-id="a49f8-129">Die Synchronisierung Vorlage enthält vorkonfigurierte synchronisierungseinstellungen für eine bestimmte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="a49f8-129">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="a49f8-130">Diese Einstellungen (vor allem [Synchronisierungsschema](synchronization-synchronizationschema.md)) werden standardmäßig für alle [Synchronisierungsauftrag](synchronization-synchronizationjob.md) verwendet werden, die auf der Vorlage basiert.</span><span class="sxs-lookup"><span data-stu-id="a49f8-130">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="a49f8-131">Vorlagen, die vom Anwendungsentwickler festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="a49f8-131">Templates are specified by the application developer.</span></span>

<span data-ttu-id="a49f8-132">Weitere Informationen finden Sie unter [Synchronisierung Vorlage](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-132">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="a49f8-133">Arbeiten mit der API-Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="a49f8-133">Working with the synchronization API</span></span>

<span data-ttu-id="a49f8-134">Arbeiten mit Synchronisierung umfasst API in erster Linie den Zugriff auf die [SynchronizationJob](synchronization-synchronizationjob.md) und [SynchronizationSchema](synchronization-synchronizationschema.md) Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="a49f8-134">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="a49f8-135">Damit die Ressource [SynchronizationJob](synchronization-synchronizationjob.md) ermittelt wird, müssen Sie die ID des Service principal-Objekts wissen, zu der der Synchronisierungsauftrag gehört.</span><span class="sxs-lookup"><span data-stu-id="a49f8-135">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="a49f8-136">Die folgenden Beispiele zeigen, wie die Ressourcen **SynchronizationJob** und **SynchronizationSchema** entwickelt.</span><span class="sxs-lookup"><span data-stu-id="a49f8-136">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="a49f8-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="a49f8-137">Authorization</span></span>

<span data-ttu-id="a49f8-138">Die Azure AD-Synchronisierung API verwendet OAuth 2.0 für die Autorisierung.</span><span class="sxs-lookup"><span data-stu-id="a49f8-138">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="a49f8-139">Vor der Durchführung von alle Anforderungen an die API, müssen Sie ein Zugriffstoken abzurufen.</span><span class="sxs-lookup"><span data-stu-id="a49f8-139">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="a49f8-140">Weitere Informationen finden Sie unter [Get Access tokens Microsoft Graph aufrufen](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="a49f8-140">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="a49f8-141">Um den Zugriff auf Ressourcen Synchronisierung benötigt Ihre Anwendung Directory.ReadWrite.All Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="a49f8-141">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="a49f8-142">Weitere Informationen finden Sie unter [Directory-Berechtigungen](/graph/permissions-reference#directory-permissions).</span><span class="sxs-lookup"><span data-stu-id="a49f8-142">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="a49f8-143">Hier finden Sie das principal-Objekt nach Anzeigename</span><span class="sxs-lookup"><span data-stu-id="a49f8-143">Find the service principal object by display name</span></span>

<span data-ttu-id="a49f8-144">Im folgenden Beispiel wird gezeigt, wie Service principal-Objekt nach dem Anzeigenamen zu suchen.</span><span class="sxs-lookup"><span data-stu-id="a49f8-144">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="a49f8-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a49f8-145">**Request**</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="a49f8-146">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="a49f8-146">**Response**</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="a49f8-147">Hier finden Sie das principal-Objekt von app-ID</span><span class="sxs-lookup"><span data-stu-id="a49f8-147">Find the service principal object by app ID</span></span>

<span data-ttu-id="a49f8-148">Das folgende Beispiel zeigt, wie Sie finden das principal-Objekt nach app-ID.</span><span class="sxs-lookup"><span data-stu-id="a49f8-148">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="a49f8-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a49f8-149">**Request** 
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="a49f8-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="a49f8-150">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="a49f8-151">Liste der vorhandenen Aufträge für die Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="a49f8-151">List existing synchronization jobs</span></span>

<span data-ttu-id="a49f8-152">Das folgende Beispiel veranschaulicht das Auflisten der vorhandenen Aufträge für die Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="a49f8-152">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="a49f8-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a49f8-153">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="a49f8-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="a49f8-154">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a><span data-ttu-id="a49f8-155">Erste Synchronisierung Auftragsstatus</span><span class="sxs-lookup"><span data-stu-id="a49f8-155">Get synchronization job status</span></span>
<span data-ttu-id="a49f8-156">Im folgende Beispiel wird das Abrufen des Status eines Auftrags zur Synchronisierung veranschaulicht.</span><span class="sxs-lookup"><span data-stu-id="a49f8-156">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="a49f8-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a49f8-157">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="a49f8-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="a49f8-158">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a><span data-ttu-id="a49f8-159">Erste Synchronisierungsschema</span><span class="sxs-lookup"><span data-stu-id="a49f8-159">Get synchronization schema</span></span>
<span data-ttu-id="a49f8-160">Im folgende Beispiel wird das Abrufen des Synchronisierungsschemas veranschaulicht.</span><span class="sxs-lookup"><span data-stu-id="a49f8-160">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="a49f8-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a49f8-161">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="a49f8-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="a49f8-162">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="a49f8-163">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="a49f8-163">See also</span></span>

* [<span data-ttu-id="a49f8-164">Konfigurieren der Synchronisierung mit Verzeichnis Extension-Attribute</span><span class="sxs-lookup"><span data-stu-id="a49f8-164">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="a49f8-165">Konfigurieren der Synchronisierung mit benutzerdefinierten Ziel-Attribute</span><span class="sxs-lookup"><span data-stu-id="a49f8-165">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
