---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---


# [!DNL Analytics] Integración de y Audience Manager

{{analytics-description}}

{{audience-manager-description}}

Habilitar esta integración reenviando el Adobe [!DNL Analytics] del lado del servidor de datos al Audience Manager, proporciona al Audience Manager una de sus principales fuentes de datos, a saber, datos de comportamiento del cliente en línea. Estos datos se pueden combinar con otros datos, como datos de CRM de origen o datos de socios de terceros, para crear segmentos de clientes enriquecidos. Además, los segmentos del Audience Manager se envían de vuelta a la página web en la respuesta de para un análisis más detallado del visitante. A continuación se describen ambos casos de uso importantes.

Ventajas clave de la integración de Adobe [!DNL Analytics] y Audience Manager:

+ **Segmentación mejorada**: Combinar Adobe [!DNL Analytics] datos de Audience Manager de y para segmentos de audiencia precisos y personalizados en campañas de marketing.
+ **Perfiles de cliente unificados**: integre fuentes de datos para comprender las interacciones y los comportamientos, creando perfiles de cliente completos.
+ **Mayor eficacia publicitaria**: optimice los anuncios con segmentación basada en datos desde el Adobe [!DNL Analytics] Integración de Audience Manager de y.
+ **Decisiones basadas en datos**: informe a las opciones a través de perspectivas detalladas, combinando Adobes [!DNL Analytics] y datos del Audience Manager.
+ **Experiencias personalizadas**: adapte el contenido y las ofertas, lo que enriquece las interacciones de los clientes entre puntos de contacto mediante ambas plataformas.

En general, esta integración reúne datos valiosos y perspectivas de audiencia. Permite a las empresas crear campañas de marketing más específicas y relevantes, a la vez que logran un conocimiento más profundo de las preferencias y comportamientos de sus clientes.

## Integraciones comunes

<table>
    <thead>
        <tr>
            <th>aplicaciones de Experience Cloud</th>
            <th>Se integra mediante</th>
            <th>Uso</th>
            <th>Casos de uso comunes</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] envío de datos al Audience Manager</a>
            </td>
            <td>Adobe [!DNL Analytics] extensión de etiquetas para AppMeasurement.js con reenvío del lado del servidor habilitado</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Cuando desee enviar el Adobe [!DNL Analytics] datos a Audience Manager para crear segmentos que se puedan compartir con otros destinos de Adobe Experience Cloud, destinos basados en personas u otros destinos basados en dispositivos y personalizados admitidos por Audience Manager.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Comparta segmentos en plataformas de publicidad que incluyan atributos de comportamiento recopilados en [!DNL Analytics].</li>
                    <li>Enriquezca los segmentos con [!DNL Analytics] datos para crear segmentos de canal cruzado de alto valor y utilizarlos en la segmentación en el sitio.</li>
                    <li>Capa en [!DNL Analytics] datos a segmentos desactivados en identificadores hash, como correo electrónico, para usarlos en plataformas de medios sociales.</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html" target="_blank" rel="noreferrer">Audience Manager que devuelve datos a [!DNL Analytics]</a>
            </td>
            <td>Adobe [!DNL Analytics] extensión de etiquetas para AppMeasurement.js con reenvío del lado del servidor habilitado</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Cuando quiera compartir segmentos de Audience Manager a [!DNL Analytics] para informar sobre la detección de audiencias, la segmentación y la optimización.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Utilice segmentos de Audience Manager que incluyan datos demográficos de proveedores externos en [!DNL Analytics] informes.</li>
                    <li>Utilice segmentos del Audience Manager que incluyan datos de campaña de los servidores de publicidad en [!DNL Analytics] informes.</li>
                    <li>Utilice segmentos de Audience Manager que incluyan datos CRM incorporados en [!DNL Analytics] informes.</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
