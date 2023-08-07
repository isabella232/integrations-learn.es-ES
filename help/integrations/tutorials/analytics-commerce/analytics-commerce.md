---
title: Integrar [!DNL Analytics] con [!DNL Commerce] tutorial
description: Aprenda a integrar [!DNL Analytics] con [!DNL Commerce].
solution: Analytics, Commerce
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: null
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integración" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 5%

---


# Integrar [!DNL Analytics] con [!DNL Commerce]

## Incorporación inicial

Estas instrucciones son para el Adobe [!DNL Commerce] Proyectos alojados en la nube. El alojamiento propio puede variar hasta cierto punto, pero el proceso general debe ser similar.

1. Compruebe el código en su entorno local
1. Usar el módulo Compositor e instalación
1. Siga las instrucciones individuales aquí y vuelva cuando haya terminado para finalizar los pasos restantes
   [Instalación y configuración de Experience Cloud [!DNL Platform] conector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. Confirme el archivo composer.json y, si se encuentra en la nube, los archivos composer.lock.
1. Compruebe que el módulo esté en los entornos de ensayo o producción. Para ello, inicie sesión en la sección de administración del Adobe [!DNL Commerce] y buscando estas nuevas secciones en Sistema > Servicios
   ![Experiencia [!DNL Platform] extensión de conector](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Configure el módulo con sus credenciales de dentro de la Adobe [!DNL Commerce] oficina de atrás.
   * Primero, el [!DNL Commerce] Configuraciones del conector de servicios, como se muestra a continuación.
     ![[!DNL Commerce] Configuración de Services Connector](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * A continuación, la experiencia [!DNL Platform] ajustes del conector, como se muestra a continuación.
     ![Experiencia [!DNL Platform] conector](./assets/analytics-commerce/experience-platform-connector.png)

Para obtener buenos detalles sobre cada fase y paso del proceso de incorporación, siga las instrucciones de la [Experiencia [!DNL Platform] descripción general del conector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"}. La experiencia [!DNL Platform] el tutorial del conector cubre cada sección en profundidad y responde a cualquier pregunta que pueda tener. Utilice este tutorial para el resto de los pasos de configuración rápida.

## Configuración de Experience Edge y Adobe [!DNL Analytics]

1. Compruebe que su organización tiene acceso al Adobe (y usted lo tiene) [!DNL Analytics]. Esto se puede confirmar en la página de [Página principal de Adobe Experience Cloud](https://experience.adobe.com/) y haciendo clic en el conmutador de aplicaciones (nueve puntos) en la barra de navegación superior.

1. Crear un nuevo grupo de informes en Adobe [!DNL Analytics]o identifique el ID del grupo de informes que va a insertar [!DNL Commerce] datos en. Para obtener más información, vea un tutorial sobre [creación de un nuevo grupo de informes](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html?lang=es). Necesitará este ID de grupo de informes en el paso del conjunto de datos a continuación.

1. Vaya a [Adobe Experience Platform [!DNL Platform] interfaz](https://platform.adobe.com) si tiene acceso a Experience Cloud [!DNL Platform]. Si no tiene acceso a esa interfaz, puede realizar todos los pasos necesarios que se enumeran a continuación en Adobe Experience Platform [!DNL Platform] [Interfaz de recopilación de datos](https://experience.adobe.com/#/data-collection).

1. Cree o actualice su esquema XDM con [!DNL Commerce]Grupos de campos específicos de. Para obtener más información sobre cómo crear un esquema, consulte la [&quot;Crear esquemas&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html?lang=es) tutorial.
   * Deberá seleccionar este esquema de las opciones del paso del conjunto de datos a continuación. Para crear un esquema, busque en la columna izquierda debajo de **Administración de datos** y buscar **Esquemas**. Ahora, en la parte superior derecha de la interfaz, haga clic en **Crear esquema**. Seleccione ExperienceEvent de XDM.
   * Después de crear un nuevo esquema, agregará el [!DNL Commerce] grupos de campos. En la parte izquierda de la interfaz de usuario, busque Grupos de campos y haga clic en **Añadir**
      * En la búsqueda, puede filtrar introduciendo `ExperienceEvent [!DNL Commerce]`
      * Seleccione el **Adobe [!DNL Analytics] ExperienceEvent[!DNL Commerce]** marcando la casilla
      * Luego haga clic en **Adición de grupos de campos** en la parte superior derecha para guardar y continuar

1. De forma opcional (y solo si está en Experience Cloud) [!DNL Platform] interfaz): cree un nuevo conjunto de datos
   * Este paso le permite llevar el [!DNL Commerce] datos en Experience Platform [!DNL Platform] (por separado de introducir los datos en el Adobe [!DNL Analytics]). Realice este paso si tiene acceso a Experience Cloud [!DNL Platform], y planean utilizar el [!DNL Commerce] datos en Experience Platform [!DNL Platform]Aplicaciones compatibles con, como Real-Time Customer Data [!DNL Platform], Recorrido del cliente [!DNL Analytics]o Journey Optimizer.
   * Deberá seleccionar este conjunto de datos de las opciones del paso de secuencia de datos a continuación.
   * En la columna izquierda **Administración de datos** encabezado en el panel de navegación izquierdo, seleccione **Conjuntos de datos**.
   * Clic **Crear conjunto de datos** en la parte superior derecha. Elija la **Crear conjunto de datos a partir de esquema** opción.
   * Busque y utilice el esquema que ha creado en el último paso

1. Cree la secuencia de datos para enviar el [!DNL Commerce] datos para el Adobe [!DNL Analytics]
   * En el **Recopilación de datos** encabezado en la columna izquierda, seleccione **Datastreams**.
   * Clic **Nueva secuencia de datos** en la parte superior derecha de la interfaz.
   * Proporcione un nombre y una descripción opcional.
   * Busque y seleccione el esquema que ha creado o identificado en el paso anterior.
   * Añada las opciones avanzadas que desee. Para obtener más información sobre las opciones avanzadas, visite la [documentación](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=es).
   * Clic **Guardar** para continuar.
   * Clic **Añadir servicio** y elija **Adobe[!DNL Analytics]** en el campo desplegable.
   * Clic **Agregar grupo de informes** e introduzca el ID del grupo de informes que creó o identificó en un paso anterior. Puede agregar más de un grupo de informes si desea que los datos fluyan a varios grupos de informes.
   * De forma opcional, y si creó un conjunto de datos en un paso anterior, haga clic en **Añadir servicio** de nuevo, elegir **Adobe Experience Platform[!DNL Platform]** en el campo desplegable. En el campo Conjunto de datos de evento, seleccione el conjunto de datos que ha creado anteriormente.
   * Guarde la secuencia de datos.

1. Por último, para ver su [!DNL Commerce] para acceder a los datos de, deberá ir a Analysis Workspace en Adobe [!DNL Analytics], cree un proyecto, elija su grupo de informes y añada tablas de forma libre y otras visualizaciones para crear informes y analizar su [!DNL Commerce] datos. La siguiente imagen muestra un ejemplo de una tabla que puede crear en Analysis Workspace.

   ![[!DNL Analytics] Captura de pantalla de algunos datos comerciales](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   Estos son algunos recursos adicionales para ayudarle a trabajar en Analysis Workspace:

   * [Información general de Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [Creación de un proyecto del Espacio de trabajo desde cero](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [Uso de tablas, visualizaciones y paneles en Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [Casos de uso de visualización](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   Además, hay cursos gratuitos disponibles en Experience League. Consulte [!DNL Analytics] cursos disponibles [AQUÍ](https://experienceleague.adobe.com/?lang=en&amp;Solution=[!DNL Analytics]#courses).
