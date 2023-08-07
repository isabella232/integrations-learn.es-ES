---
title: Integrar [!DNL Analytics] y datos de clientes en tiempo real [!DNL Platform] con experiencia [!DNL Platform] tutorial del conector de origen
description: Aprenda a integrar Adobe [!DNL Analytics] con datos de clientes en tiempo real [!DNL Platform] uso de la experiencia [!DNL Platform] conector de origen.
solution: Real-Time Customer Data [!DNL Platform], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integración" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 19%

---


# Integrar Adobe [!DNL Analytics] y datos de clientes en tiempo real [!DNL Platform] con experiencia [!DNL Platform] conector de origen

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=es#dashboard/learning" _target="_blank" rel="noopener noreferrer">Cree esquemas</a> para introducir los datos.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=es" _target="_blank" rel="noopener noreferrer">Cree conjuntos de datos</a> para incorporar los datos.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configurar las identidades y áreas de nombres de identidad correctas en el esquema</a> para asegurarse de que los datos introducidos puedan vincularse a un perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=es" _target="_blank" rel="noopener noreferrer">Habilitar los esquemas y conjuntos de datos para el perfil</a>.</li>
    <li>Ingesta [!DNL Analytics] en Experience Platform mediante el <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=es" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] conector de origen</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html" _target="_blank" rel="noopener noreferrer">Creación de segmentos en Experience Platform [!DNL Platform].</a> El sistema determina automáticamente si el segmento se evalúa como por lotes (conector de datos) o por secuencias (red de Edge).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Configure destinos para compartir atributos de perfil y pertenencias de audiencias en los destinos deseados.</a></li>   
</ol>

>[!NOTE]
>
>Los pasos estándar del flujo de trabajo para el Adobe [!DNL Analytics] conector de origen: cree el esquema y el conjunto de datos utilizados para introducir los datos de [!DNL Analytics] &quot;tal cual&quot;. Por lo tanto, el sistema gestiona los dos primeros pasos. El flujo de trabajo de asignación requiere la creación de atributos personalizados; por lo tanto, siga totalmente la secuencia de pasos.
