---
title: Arbeiten mit Education-APIs in Microsoft Graph
description: Office 365-Ressourcen und Daten mit der relevante Informationen für Bildungseinrichtungen Szenarien, einschließlich Schulen, Studenten, Lehrer, Klassen, Registrierung und Zuordnungen der Education-APIs in Microsoft Graph zu verbessern. Dies erleichtert das Erstellen von Lösungen, die in Bildungsressourcen integriert werden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e106da7eb717a091941e16f4a70af8a012802f3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516931"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="74520-104">Arbeiten mit Education-APIs in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="74520-104">Working with education APIs in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74520-105">Office 365-Ressourcen und Daten mit der relevante Informationen für Bildungseinrichtungen Szenarien, einschließlich Schulen, Studenten, Lehrer, Klassen, Registrierung und Zuordnungen der Education-APIs in Microsoft Graph zu verbessern.</span><span class="sxs-lookup"><span data-stu-id="74520-105">The education APIs in Microsoft Graph enhance Office 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, enrollments, and assignments.</span></span> <span data-ttu-id="74520-106">Dies erleichtert das Erstellen von Lösungen, die in Bildungsressourcen integriert werden.</span><span class="sxs-lookup"><span data-stu-id="74520-106">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="74520-107">Die Education umfassen APIs Rostering und Zuordnungen Ressourcen, die Sie für die Interaktion mit den Rostering und Zuweisen von Diensten in Microsoft-Teams verwenden können.</span><span class="sxs-lookup"><span data-stu-id="74520-107">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering and assignment services in Microsoft Teams.</span></span> <span data-ttu-id="74520-108">Diese Ressourcen können Sie eine Schule Teilnehmerliste verwalten und Automatisierung von Hausaufgaben.</span><span class="sxs-lookup"><span data-stu-id="74520-108">You can use these resources to manage a school roster and automate student assignments.</span></span>

## <a name="authorization"></a><span data-ttu-id="74520-109">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="74520-109">Authorization</span></span>

<span data-ttu-id="74520-110">Damit die Education-APIs in Microsoft Graph aufgerufen werden können, muss Ihre App ein Zugriffstoken erwerben.</span><span class="sxs-lookup"><span data-stu-id="74520-110">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="74520-111">Weitere Informationen zu Zugriffstoken finden Sie unter [Abrufen von Zugriffstoken zum Aufrufen von Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="74520-111">For details about access tokens, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="74520-112">Zudem muss Ihre App über die entsprechenden Berechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="74520-112">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="74520-113">Weitere Informationen finden Sie unter [Education-Berechtigungen](/graph/permissions-reference#education-permissions).</span><span class="sxs-lookup"><span data-stu-id="74520-113">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span> 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="74520-114">App-Berechtigungen zum Aktivieren der Zustimmung von Schul-IT-Administratoren</span><span class="sxs-lookup"><span data-stu-id="74520-114">App permissions to enable school IT admins to consent</span></span> 

<span data-ttu-id="74520-115">Um Apps bereitzustellen, die in Education-APIs in Microsoft Graph integriert sind, müssen Schul-IT-Administratoren zunächst ihre Zustimmung für die von der App angeforderten Berechtigungen erteilen.</span><span class="sxs-lookup"><span data-stu-id="74520-115">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="74520-116">Diese Zustimmung muss nur einmal erteilt werden, sofern sich die Berechtigungen nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="74520-116">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="74520-117">Nachdem der Administrator seine Zustimmung erteilt hat, wird die App für alle Benutzer im Mandanten bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="74520-117">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="74520-118">Verwenden Sie den folgenden REST-Aufruf, um ein Dialogfeld für die Zustimmung auszulösen.</span><span class="sxs-lookup"><span data-stu-id="74520-118">To trigger a consent dialog box, use the following REST call.</span></span>

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|<span data-ttu-id="74520-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="74520-119">Parameter</span></span>|<span data-ttu-id="74520-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74520-120">Description</span></span>|
|:--------|:----------|
|<span data-ttu-id="74520-121">Mandant</span><span class="sxs-lookup"><span data-stu-id="74520-121">Tenant</span></span>|<span data-ttu-id="74520-122">Mandanten-ID der Schule.</span><span class="sxs-lookup"><span data-stu-id="74520-122">Tenant ID of the school.</span></span> <span data-ttu-id="74520-123">Verwenden Sie die vollständige-ID, die „onmicrosoft.com“ enthält.</span><span class="sxs-lookup"><span data-stu-id="74520-123">Use the full ID, which includes onmicrosoft.com.</span></span>|
|<span data-ttu-id="74520-124">clientId</span><span class="sxs-lookup"><span data-stu-id="74520-124">clientId</span></span>|<span data-ttu-id="74520-125">Client-ID der App.</span><span class="sxs-lookup"><span data-stu-id="74520-125">Client ID of the app.</span></span>|
|<span data-ttu-id="74520-126">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="74520-126">redirectUrl</span></span>|<span data-ttu-id="74520-127">App-Umleitungs-URL.</span><span class="sxs-lookup"><span data-stu-id="74520-127">App redirect URL.</span></span>|


## <a name="rostering"></a><span data-ttu-id="74520-128">Listenerstellung</span><span class="sxs-lookup"><span data-stu-id="74520-128">Rostering</span></span>

<span data-ttu-id="74520-129">Mit Listenerstellungs-APIs können Sie Daten von einem Office 365-Mandanten der Schule extrahieren, der mit [Microsoft School Data Sync](https://sds.microsoft.com/) bereitgestellt wurde. Diese APIs bieten Zugriff auf Informationen zu Schulen, Abschnitten, Lehrern, Schülern, Studenten und Listen.</span><span class="sxs-lookup"><span data-stu-id="74520-129">The rostering APIs enable you to extract data from a school's Office 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="74520-130">Die APIs unterstützen sowohl Szenarien vom Typ „Nur App“ (Synchronisierung) als auch vom Typ „App und Benutzer“ (interaktiv).</span><span class="sxs-lookup"><span data-stu-id="74520-130">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="74520-131">APIs, die interaktive Szenarien unterstützen, erzwingen auf Grundlage der Benutzerrolle, die die API aufruft, regionsspezifische RBAC-Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="74520-131">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="74520-132">Dies ermöglicht eine konsistente API und eine minimale Richtlinienoberfläche, unabhängig von der Verwaltungskonfiguration innerhalb der Mandanten.</span><span class="sxs-lookup"><span data-stu-id="74520-132">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="74520-133">Die APIs bieten darüber hinaus auch bildungsspezifische Berechtigungen, um sicherzustellen, dass der richtige Benutzer auf die Daten zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="74520-133">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="74520-134">Mithilfe von Listenerstellungs-APIs erhält der App-Benutzer Antworten auf die folgenden Fragen:</span><span class="sxs-lookup"><span data-stu-id="74520-134">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="74520-135">Wer bin ich?</span><span class="sxs-lookup"><span data-stu-id="74520-135">Who I am</span></span>
- <span data-ttu-id="74520-136">An welchen Kursen nehme ich teil bzw. welche Kurse unterrichte ich?</span><span class="sxs-lookup"><span data-stu-id="74520-136">What classes I attend or teach</span></span>
- <span data-ttu-id="74520-137">Was muss ich wann tun?</span><span class="sxs-lookup"><span data-stu-id="74520-137">What I need to do and by when</span></span>

<span data-ttu-id="74520-138">Die Listenerstellungs-APIs bieten die folgenden zentralen Ressourcen:</span><span class="sxs-lookup"><span data-stu-id="74520-138">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="74520-139">[educationSchool](educationschool.md): Schule.</span><span class="sxs-lookup"><span data-stu-id="74520-139">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="74520-140">[educationClass](educationclass.md): Kurs in einer Schule.</span><span class="sxs-lookup"><span data-stu-id="74520-140">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="74520-141">[educationTerm](educationterm.md): Ein festgelegter Teil des akademischen Jahres.</span><span class="sxs-lookup"><span data-stu-id="74520-141">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="74520-142">[educationTeacher](educationteacher.md): Ein Benutzer mit der primären Rolle „Lehrer“.</span><span class="sxs-lookup"><span data-stu-id="74520-142">[educationTeacher](educationteacher.md) - Represents a users with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="74520-143">[educationStudent](educationstudent.md): Ein Benutzer mit der primären Rolle „Schüler/Student“.</span><span class="sxs-lookup"><span data-stu-id="74520-143">[educationStudent](educationstudent.md) - Represents a users with the primary role of 'student'.</span></span>

<span data-ttu-id="74520-144">Die Listenerstellungs-APIs unterstützen die folgenden Szenarien:</span><span class="sxs-lookup"><span data-stu-id="74520-144">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="74520-145">Auflisten aller Schulen</span><span class="sxs-lookup"><span data-stu-id="74520-145">List all schools</span></span>](../api/educationroot-list-schools.md) 
- [<span data-ttu-id="74520-146">Auflisten von Schulen, in denen ein Kurs unterrichtet wird</span><span class="sxs-lookup"><span data-stu-id="74520-146">List schools in which a class is taught</span></span>](../api/educationclass-list-schools.md)
- [<span data-ttu-id="74520-147">Auflisten von Schulen für einen Benutzer</span><span class="sxs-lookup"><span data-stu-id="74520-147">List schools for a user</span></span>](../api/educationuser-list-schools.md)
- [<span data-ttu-id="74520-148">Abrufen aller Kurse</span><span class="sxs-lookup"><span data-stu-id="74520-148">Get all classes</span></span>](../api/educationroot_list_classes.md )
- [<span data-ttu-id="74520-149">Abrufen von Kursen einer Schule</span><span class="sxs-lookup"><span data-stu-id="74520-149">Get classes in a school</span></span>](../api/educationschool-list-classes.md)
- [<span data-ttu-id="74520-150">Auflisten von Kursen für einen Benutzer</span><span class="sxs-lookup"><span data-stu-id="74520-150">List classes for a user</span></span>](../api/educationuser-list-classes.md)
- [<span data-ttu-id="74520-151">Hinzufügen von Kursen zu einer Schule</span><span class="sxs-lookup"><span data-stu-id="74520-151">Add classes to a school</span></span>](../api/educationschool-post-classes.md)
- [<span data-ttu-id="74520-152">Abrufen von Schülern/Studenten und Lehrern für einen Kurs</span><span class="sxs-lookup"><span data-stu-id="74520-152">Get students and teachers for a class</span></span>](../api/educationclass-list-members.md)
- [<span data-ttu-id="74520-153">Hinzufügen von Mitgliedern zu einem Kurs</span><span class="sxs-lookup"><span data-stu-id="74520-153">Add members to a class</span></span>](../api/educationclass-post-members.md) 
- [<span data-ttu-id="74520-154">Auflisten von Lehrern für einen Kurs</span><span class="sxs-lookup"><span data-stu-id="74520-154">List teachers for a class</span></span>](../api/educationclass-list-teachers.md)
- [<span data-ttu-id="74520-155">Abrufen von Benutzern in einer Schule</span><span class="sxs-lookup"><span data-stu-id="74520-155">Get users in a school</span></span>](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a><span data-ttu-id="74520-156">Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="74520-156">Assignments</span></span> 

<span data-ttu-id="74520-157">Die Education Assignment-bezogene APIs können Sie um Zuordnungen in Microsoft-Teams, zu integrieren.</span><span class="sxs-lookup"><span data-stu-id="74520-157">You can use the assignment-related education APIs to integrate with assignments in Microsoft Teams.</span></span> <span data-ttu-id="74520-158">Microsoft-Teams in Office 365 für Bildungseinrichtungen basiert auf der gleichen Education-APIs und bietet einen Anwendungsfall für die Arbeit mit den APIs.</span><span class="sxs-lookup"><span data-stu-id="74520-158">Microsoft Teams in Office 365 for Education is based on the same education APIs, and provides a use case for what you can do with the APIs.</span></span> <span data-ttu-id="74520-159">Ihre app kann diese APIs Interaktion mit Zuordnungen im gesamten Lebenszyklus Zuordnung verwenden.</span><span class="sxs-lookup"><span data-stu-id="74520-159">Your app can use these APIs to interact with assignments throughout the assignment lifecycle.</span></span> 

<span data-ttu-id="74520-160">Die Zuordnung APIs bieten die folgenden wichtigen Ressourcen:</span><span class="sxs-lookup"><span data-stu-id="74520-160">The assignment APIs provide the following key resources:</span></span>

- <span data-ttu-id="74520-161">[EducationAssignment](educationassignment.md) - Core-Objekts der Zuordnungen API.</span><span class="sxs-lookup"><span data-stu-id="74520-161">[educationAssignment](educationassignment.md) - The core object of the assignments API.</span></span> <span data-ttu-id="74520-162">Stellt einen Vorgang oder eine Arbeitsschritt Mitglied Student oder ein Team in einer Klasse als Teil ihrer Studie zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="74520-162">Represents a task or unit of work assigned to a student or team member in a class as part of their study.</span></span>
- <span data-ttu-id="74520-163">[EducationSubmission](educationsubmission.md) – stellt die Ressourcen, die eine einzelne (oder Gruppe) für eine Zuordnung und die zugehörigen Note und Feedback für diese Aufgabe sendet.</span><span class="sxs-lookup"><span data-stu-id="74520-163">[educationSubmission](educationsubmission.md) - Represents the resources that an individual (or group) submits for an assignment and the associated grade and feedback for that assignment.</span></span>
- <span data-ttu-id="74520-164">[EducationResource](educationresource.md) - stellt also das Learning-Objekt zugewiesen wird, oder übermittelt.</span><span class="sxs-lookup"><span data-stu-id="74520-164">[educationResource](educationresource.md) - Represents the learning object that is being assigned or submitted.</span></span> <span data-ttu-id="74520-165">Ein **EducationResource** ist ein **EducationAssignment** und/oder ein **EducationSubmission**zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="74520-165">An **educationResource** is associated with an **educationAssignment** and/or an **educationSubmission**.</span></span>

<span data-ttu-id="74520-166">Die Zuordnung APIs unterstützen die folgenden Szenarien:</span><span class="sxs-lookup"><span data-stu-id="74520-166">The assignment APIs support the following scenarios:</span></span>

- [<span data-ttu-id="74520-167">Erstellen der Zuordnung</span><span class="sxs-lookup"><span data-stu-id="74520-167">Create assignment</span></span>](../api/educationclass-post-assignments.md)
- [<span data-ttu-id="74520-168">Zuordnung veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="74520-168">Publish assignment</span></span>](../api/educationassignment-publish.md)
- [<span data-ttu-id="74520-169">Erstellen der Zuordnung Ressource</span><span class="sxs-lookup"><span data-stu-id="74520-169">Create assignment resource</span></span>](../api/educationassignment-post-resources.md)
- [<span data-ttu-id="74520-170">Erstellen Sie zum Absenden-Ressource</span><span class="sxs-lookup"><span data-stu-id="74520-170">Create submission resource</span></span>](../api/educationsubmission-post-resources.md)
- [<span data-ttu-id="74520-171">Aufgabe abgeben</span><span class="sxs-lookup"><span data-stu-id="74520-171">Submit assignment</span></span>](../api/educationsubmission-submit.md) 
- [<span data-ttu-id="74520-172">Zuordnung unsubmit</span><span class="sxs-lookup"><span data-stu-id="74520-172">Unsubmit assignment</span></span>](../api/educationsubmission-unsubmit.md)   
- [<span data-ttu-id="74520-173">Klassen und Feedback zur Student zurückzukehren.</span><span class="sxs-lookup"><span data-stu-id="74520-173">Return grades and feedback to student</span></span>](../api/educationsubmission-return.md) 
- [<span data-ttu-id="74520-174">Abrufen von Zuordnungsdetails</span><span class="sxs-lookup"><span data-stu-id="74520-174">Get assignment details</span></span>](../api/educationuser-list-assignments.md)

<span data-ttu-id="74520-175">Es folgen einige allgemeine Verwendungsszenarien für die Zuordnung-bezogene Bildungseinrichtungen APIs.</span><span class="sxs-lookup"><span data-stu-id="74520-175">The following are some common use cases for the assignment-related education APIs.</span></span>

|<span data-ttu-id="74520-176">Anwendungsfall</span><span class="sxs-lookup"><span data-stu-id="74520-176">Use case</span></span>|<span data-ttu-id="74520-177">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74520-177">Description</span></span>|<span data-ttu-id="74520-178">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="74520-178">See also</span></span>|
|:-------|:----------|:-------|
|<span data-ttu-id="74520-179">Erstellen von Aufgaben</span><span class="sxs-lookup"><span data-stu-id="74520-179">Create assignments</span></span>|<span data-ttu-id="74520-180">Ein externes System kann eine Zuordnung für die Klasse erstellt und die Zuordnung Ressourcen zuordnen.</span><span class="sxs-lookup"><span data-stu-id="74520-180">An external system can create an assignment for the class and attach resources to the assignment.</span></span>|[<span data-ttu-id="74520-181">Erstellen der Zuordnung</span><span class="sxs-lookup"><span data-stu-id="74520-181">Create assignment</span></span>](../api/educationassignment-post-resources.md)|
|<span data-ttu-id="74520-182">Lesen Sie die Informationen zur Zuordnung</span><span class="sxs-lookup"><span data-stu-id="74520-182">Read assignment information</span></span>|<span data-ttu-id="74520-183">Eine Anwendung Analytics erhalten Informationen zu Aufgaben und Student Übermittlungen, einschließlich Datums- und Klassen.</span><span class="sxs-lookup"><span data-stu-id="74520-183">An analytics application can get information about assignments and student submissions, including dates and grades.</span></span>|[<span data-ttu-id="74520-184">Abrufen der Zuordnung</span><span class="sxs-lookup"><span data-stu-id="74520-184">Get assignment</span></span>](../api/educationassignment-get.md)|
|<span data-ttu-id="74520-185">Nachverfolgen von Student Übermittlungen</span><span class="sxs-lookup"><span data-stu-id="74520-185">Track student submissions</span></span>|<span data-ttu-id="74520-186">Ihre app kann ein Dashboard Lehrer bereitstellen, das zeigt, wie viele eingereichten Studenten bewertet werden müssen.</span><span class="sxs-lookup"><span data-stu-id="74520-186">Your app can provide a teacher dashboard that shows how many submissions from students need to be graded.</span></span>|[<span data-ttu-id="74520-187">Übermittlung Ressource</span><span class="sxs-lookup"><span data-stu-id="74520-187">Submission resource</span></span>](educationsubmission.md)|

## <a name="school-data-sync-management"></a><span data-ttu-id="74520-188">Schule Sync-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="74520-188">School data sync management</span></span>

<span data-ttu-id="74520-189">[Schule Daten Sync](https://sds.microsoft.com/) hilft importieren und Synchronisieren von Daten aus Student Informationssysteme Teilnehmerliste einer mit Azure Active Directory (AD Azure) und Office 365 automatisieren.</span><span class="sxs-lookup"><span data-stu-id="74520-189">[School Data Sync](https://sds.microsoft.com/) helps to automate the process of importing and synchronizing roster data from student information systems with Azure Active Directory (Azure AD) and Office 365.</span></span> <span data-ttu-id="74520-190">Sync-datenverwaltung Schule APIs können in Microsoft Graph Sie aus einer CSV-Datei oder einen unterstützten SIS API-Connector-Synchronisierung einrichten.</span><span class="sxs-lookup"><span data-stu-id="74520-190">You can use the school data sync management APIs in Microsoft Graph to set up synchronization from either a CSV file or a supported SIS API connector.</span></span>

<span data-ttu-id="74520-191">Die Schuldaten synchronisieren Management APIs unterstützt die folgenden Szenarien:</span><span class="sxs-lookup"><span data-stu-id="74520-191">The school data sync management APIs support the following scenarios:</span></span>

- [<span data-ttu-id="74520-192">Liste Synchronisierungsprofile</span><span class="sxs-lookup"><span data-stu-id="74520-192">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md)
- [<span data-ttu-id="74520-193">Synchronisierung Profil abrufen</span><span class="sxs-lookup"><span data-stu-id="74520-193">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md)
- [<span data-ttu-id="74520-194">Erstellen Sie Synchronisierung Profil</span><span class="sxs-lookup"><span data-stu-id="74520-194">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md)
- [<span data-ttu-id="74520-195">Synchronisierung Profil löschen</span><span class="sxs-lookup"><span data-stu-id="74520-195">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md)
- [<span data-ttu-id="74520-196">Eine laufende Synchronisierung anhalten</span><span class="sxs-lookup"><span data-stu-id="74520-196">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md)
- [<span data-ttu-id="74520-197">Fortsetzen einer angehaltenen sync</span><span class="sxs-lookup"><span data-stu-id="74520-197">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md)
- [<span data-ttu-id="74520-198">Zurücksetzen einer Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="74520-198">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md)
- [<span data-ttu-id="74520-199">Synchronisierung für Uploaddateien starten</span><span class="sxs-lookup"><span data-stu-id="74520-199">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) 
- [<span data-ttu-id="74520-200">Abrufen einer Upload-URL</span><span class="sxs-lookup"><span data-stu-id="74520-200">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md)
- [<span data-ttu-id="74520-201">Abrufen des Status der Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="74520-201">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md)
- [<span data-ttu-id="74520-202">Abrufen von Synchronisierungsfehler</span><span class="sxs-lookup"><span data-stu-id="74520-202">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a><span data-ttu-id="74520-203">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="74520-203">Next steps</span></span>
<span data-ttu-id="74520-204">Verwenden Sie das Microsoft Graph Education APIs Education-Lösungen zu erstellen, der Hausaufgaben und Schule konferenzlisten zugreifen.</span><span class="sxs-lookup"><span data-stu-id="74520-204">Use the Microsoft Graph education APIs to build education solutions that access student assignments and school rosters.</span></span> <span data-ttu-id="74520-205">So erhalten Sie weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="74520-205">To learn more:</span></span>

- <span data-ttu-id="74520-206">Erfahren Sie, welche Ressourcen und Methoden für Ihr Szenario am besten geeignet sind.</span><span class="sxs-lookup"><span data-stu-id="74520-206">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="74520-207">Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.</span><span class="sxs-lookup"><span data-stu-id="74520-207">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/education-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
