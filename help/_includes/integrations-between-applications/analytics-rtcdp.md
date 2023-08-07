---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 1%

---


# Integrar Adobe [!DNL Analytics] con datos de clientes en tiempo real [!DNL Platform]

{{analytics-description}}

{{real-time-cdp-description}}

Integrando el Adobe [!DNL Analytics] con Adobe de datos de clientes en tiempo real [!DNL Platform] (Real-Time CDP) puede ofrecer varias ventajas a las empresas que buscan mejorar sus experiencias de cliente y sus esfuerzos de marketing. Estas son algunas de las ventajas clave:

+ **Segmentación y personalización de audiencias mejoradas**: Marketing preciso en dispositivos y canales, mensajes personalizados para una participación optimizada.
+ **Optimización de la página de aterrizaje mejorada**: experiencias adaptadas basadas en el dispositivo y el comportamiento, que mejoran la satisfacción y la conversión del usuario.
+ **Activación de audiencia perfecta**: utilice los perfiles del cliente para una segmentación eficaz a través de los canales preferidos, entregando los mensajes relevantes.

Combinando Adobe [!DNL Analytics] Con Real-Time CDP, las empresas pueden llevar sus esfuerzos de marketing al siguiente nivel, ofreciendo experiencias personalizadas, aumentando la participación de los clientes y optimizando las conversiones en varios puntos de contacto digitales.

<table>
    <thead>
        <tr>
            <th>aplicaciones de Experience Cloud</th>
            <th>Se integra mediante</th>
            <th>Uso</th>
            <th>Casos de uso comunes</th>
        </tr>
    </thead>
    <tr>
        <td rowspan="2">[!DNL Analytics] con Real-Time CDP</td>
        <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Experiencia [!DNL Platform] conector de origen</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Enfoque recomendado para clientes que ya han implementado Adobe [!DNL Analytics]y desean la forma más rápida de introducir estos datos en Experience Platform [!DNL Platform] para usar en el Perfil del cliente en tiempo real.</li>
                <li>Cuando la disponibilidad de los datos para el Perfil del cliente en tiempo real puede estar entre 2 y 30 minutos desde el momento de la recopilación de datos, y la disponibilidad para el lago de datos es de hasta 90 minutos.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>Flujo de trabajo iniciado directamente por la interfaz de usuario.</li>
                <li>Asignación de la interfaz de usuario para copiar [!DNL Analytics] props y eVars para nuevos campos XDM.</li>
                <li>La forma más rápida de obtener valor de Perfil del cliente en tiempo real y Recorrido del cliente [!DNL Analytics].</li>
            </ul>
        </td>
    </tr>
    <tr>
       <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-edge.md" target="_blank" rel="noreferrer">Experiencia [!DNL Platform] Edge</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Enfoque recomendado para nuevas [!DNL Analytics] o cuando desee implementar una estrategia a largo plazo.</li>
                <li>Envía datos directamente desde un dispositivo a Experience Cloud [!DNL Platform] mediante el SDK web de AEP, el SDK móvil de AEP o la API del servidor de red perimetral.</li>
                <li>Clientes nuevos o existentes que necesitan [!DNL Analytics] disponibilidad de datos en el Perfil del cliente en tiempo real para admitir casos de uso de personalización de la misma página y de la siguiente.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>Proporciona el bueno nivel de control para los datos recopilados que se deben utilizar para admitir casos de uso.</li>
                <li>Los datos del lado del cliente se asignan fácilmente a campos XDM.</li>
                <li>La disponibilidad de datos más rápida para el Perfil del cliente en tiempo real.</li>
            </ul>
        </td>
    </tr>            
</table>
