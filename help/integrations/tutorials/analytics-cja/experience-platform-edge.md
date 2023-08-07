---
title: Integrar Adobe [!DNL Analytics] y Recorrido del cliente [!DNL Analytics] con la experiencia [!DNL Platform] Tutorial de Edge
description: Aprenda a integrar Adobe [!DNL Analytics] con el Recorrido del cliente [!DNL Analytics] mediante el SDK web de AEP, el SDK móvil de AEP o la API del servidor de red perimetral.
solution: Customer Journey [!DNL Analytics], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
hidefromtoc: true
kt: null
thumbnail: 13728
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integración" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 21%

---


# Integrar Adobe [!DNL Analytics] y Recorrido del cliente [!DNL Analytics] con la experiencia [!DNL Platform] Tutorial de Edge

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=es#dashboard/learning" _target="_blank" rel="noopener noreferrer">Cree esquemas</a> para introducir los datos.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=es" _target="_blank" rel="noopener noreferrer">Cree conjuntos de datos</a> para incorporar los datos.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configurar las identidades y áreas de nombres de identidad correctas en el esquema</a> para asegurarse de que los datos introducidos puedan vincularse a un perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=es" _target="_blank" rel="noopener noreferrer">Habilitar los esquemas y conjuntos de datos para el perfil</a>.</li>
    <li>Ingesta de datos en Experience Platform [!DNL Platform] mediante uno de estos métodos:</li>
        <ul>
            <li>Experiencia [!DNL Platform] SDK web:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=es" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Lista de comprobación</a></li>
                </ul>
            <li>Experiencia [!DNL Platform] SDK móvil:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Lista de comprobación</a></li>
                </ul></li>
            <li>API del servidor de red perimetral:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html?lang=es" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><i>(Opcional)</i>. Si utiliza varios conjuntos de datos, vincule el ID de la persona a <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">generar un conjunto de datos combinado</a>. Si se usa un solo [!DNL Analytics] o si existe un identificador común en todos los conjuntos de datos que planea utilizar en Customer Recorrido [!DNL Analytics], omita este paso.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=es" _target="_blank" rel="noopener noreferrer"></a>Crear una conexión en Customer Journey [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">Creación de una vista de datos</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">configurar los ajustes del componente</a>, y <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">formatear métricas</a> en Recorrido del cliente [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html" _target="_blank" rel="noopener noreferrer">Creación de un proyecto en Recorrido del cliente [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>Los pasos estándar del flujo de trabajo para el Adobe [!DNL Analytics] conector de origen: cree el esquema y el conjunto de datos utilizados para introducir los datos de [!DNL Analytics] &quot;tal cual&quot;. Por lo tanto, el sistema gestiona los dos primeros pasos. El flujo de trabajo de asignación requiere la creación de atributos personalizados; por lo tanto, siga totalmente la secuencia de pasos.
