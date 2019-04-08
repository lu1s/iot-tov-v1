# Una Cripto-garantía e Interfaz de Transferencia de Valor para Dispositivos Conectados

## Deslinde de responsabilidades sobre este documento
```text
(c) Copyright 2019. Todos los derechos reservados.
Autor: Luis Pulido Díaz (lu1s).
El autor y compañía mantienen y se reservan los derechos del contenido de este documento.
Todos los repositorios públicos y documentos serán publicados en https://github.com/lu1salways/iot-tov-v1 a menos que se en una versión futura del mismo se exprese otra ubicación de su publicación.
K_DOCUMENT_TITLE: "+LKNC$: Crypto warranty and transfer of value interface for connected devices."

lu1s.s1gn.201901280002223590000.e3434.e22.nl.eom.
```

## Deslinde de responsabilidades en cuanto a IETF o IETF-México
En muchos documentos de estándares varias palabras son utilizadas para dar significado a los requerimientos en la especificación.

Esas palabras son regularmente escritas en mayúsculas. Este documento define esas palabras como deberían de ser interpretadas en documentos de IETF o de IETF-México.

Los autores que siguen estos lineamientos deberían incorporar estas frases cerca del inicio de su documento:

_Las palabras clave "DEBE", "NO DEBE", "REQUERIDO", "DEBERÍA", "NO DEBERÍA", "DEBIERA", "NO DEBIERA", "RECOMENDADO", "TAL VEZ" y "OPCIONAL" en este documento deberían ser interpretadas como es descrito en el RFC 2119 (o una traducción al español legítima del mismo)._

Cuando las letras unidas en mayúscula "US" se encuentren en este documento, no significa o no hace referencia al país de los Estados Unidos de América, y en su defecto, debería ser interpretada como la palabra "nosotros" en inglés (us); y si en contexto fuese encontrada alguna frase o párrafo en inglés que la contenga, haría referencia a el "nosotros" como los proveedores, autores e implementadores de el RFC (Request For Comments; no RFC de el anterior Instituto Federal Electoral) 2119 (en su entendimiento y traducción al Español o Castellano).

La ciudadanía del autor o los autores es clasificada y va a ser desclasificada en un futuro o en unos futuros.

## Preámbulo

En años recientes el crecimiento global en materia de varios temas incluyendo y enfatizando los tecnológicos, ha sido circunstancialmente grande, y como un efecto natural y también circunstancial, también ha creado mayores retos para los líderes de organizaciones públicas y privadas para habilitar y compartir esos alcances tecnológicos de la humanidad con sus propios ecosistemas y entidades; y con aquellos y aquellas con quienes se relacionan.

El trabajo presentado aquí es una compilación de esfuerzos, ideas, códigos fuente, modelos de negocio, términos, condiciones, políticas de privacidad, licencias y otras informaciones que, como un todo, representan tecnología segura para un mejoramiento más justo de la salud y bienestar de una economía y de la economía como un todo.

En este documento, un Estado o País es una Entidad Soberana que, con los términos, condiciones, políticas de privacidad, licencias y una Asamblea Aprobada de Emisión de Valores \(AAEV\), o una Entidad que funja como ello; es capaz de construir y mantener un ecosistema justo y estable y por ende una economía más saludable y más justamente distribuída.

Como un ejemplo, y en el caso particualar de México \(el País; coomo un completo Conjunto de Estados Conectados\), la AAEV es hoy\[1\] el "Banco de México" \(también concido como "Banco de Mexico" o "BdM" o "BoM"\). El BdM es la Entidad a cargo de todas las emisiones de valores o dinero, así como de su reciclaje y control dentro del País y para los intereses del mismo.

_\[1\] Hoy al ser 201901290001601590000, e invalidado si fuese incorrecto._

## Conceptos básicos y entidades

_Las palabras clave enlistadas aquí están en desorden y se presentan en forma de bosquejo._

| Acrónimo | Nombre | Descripción |
| :--- | :--- | :--- |
| FSF | Free Software Foundation | |
| GNU | El Sistema Operativo de FSF llamado GNU | |
| GNUFL | El Lenguaje Fortran de GNU | |
| COBOL | El Lenguaje Común Orientado a los Negocios (No LCON) | |
| COBOL-IT | La Alternativa en Código Abierto a COBOL | |
| KLANG | El Lenguaje de Programación K | |
| ABM | Asociación de Bancos Mexicanos | |
| IETFMX | La Fuerza de Trabajo de Ingeniería de Internet en México | |
| IETF | La Fuerza de Trabajo de Ingeniería de Internet | Originalmente conocida como "Internet Engineering Task Force" |
| RFC | Requerimiento Para Comentarios del IETF o IETF-México | Es importante no confundir el RFC ni con el RFC del antiguo Instituto Federal Electoral o del Instituto Nacional Electoral; ni con RPC |
| RFCNR | Requerimiento Para Comentarios No Requerido | El RFCNR es un conjunto de uno o más hilos de conversación |
| DRFCE | Bosquejo de un RFC con Errores | |
| DRFCC | Bosquejo de un RFC que está Limpio o sin Errores | |
| PRFC | RFC Publicado (Estándar de Internet) | |
| DoH | DNS-sobre-HTTPS | Formato estandarizado y protocolo para enviar consultas al Sistema de Nombres de Dominio (o DNS) a través de HTTP en vez del tradicional protocolo de DNS (RFC-8484) |
| DoS | Denegación de Servicio (ó DdS) | La Denegación de Servicio es una técnica que puede ser aplicada por un ISP, un atacante, un gobierno o alguna otra entidad y que consiste en interrumpir un servicio temporal o permanentemente |
| PoK | Prueba de Conocimiento (ó PdC) | La Prueba de Conocimiento es una prueba válida de que cierto conocimiento esperado es concevido por una o más entidades individuales |
| RPoHC | Prueba Real de Consentimiento Humano (ó PRdCH) | El PRdCH es una prueba válida que forza el respeto a los derechos humanos dentro del ecosistema y que consiste en que el actor humano está siendo consciente de las decisiones que ella o él está siendo capaz de tomar o hacer sobre algo en particular |
| EFF | La Fundación EFF | La Fundación EFF o "Electronic Frontier Foundation", por sus siglas en inglés, es una fundación que tiene como principal objetivo defender la privacidad, la libre expresión y la innovación |
| ToS | Términos del Servicio (ó TdS) | Los TdS son un conjunto de informaciones organizadas que describen de una manera detallada y entendible cómo es una interacción en particular (la cual también puede ser llamada servicio), funcionaría en un periodo determinado. Los TdS buscan ayudar a ambas partes a establecer un acuerdo concreto e inteligente y no buscan perseguir a ninguna de las partes. |
| IoT | Internet de las Cosas (ó IdlC) | |
| IoH | Internet de los Humanos (ó IdH) | El IdH es un dispositivo que es instalado en un Ser Humano bajo su conocimiento y consentimiento de su respectiva RPOHC y PdC de los TdS, condiciones y políticas de privacidad |
| IoA | Internet de los Animales (ó IdA) | El IdA es un dispositivo IdlC que es instalado en un Ser Vivo que no es Humano y que no está enlistado en la lista de Animales Restringidos de Internet de los Animales (LdARIA) y que su o sus Humanos Oficialmente Responsables (HORdIdA) ha provisto de una PdC de los TdS y Políticas de Privacidad para su interacción y para hacer uso de sus Servicios |
| IoV | Internet de los Vehículos (ó IdV) | El IdV es un dispositivo IoT que es Instalado (kev:cinstall) en un Vehículo y que si otro u otros IdC han sido también instalados en el mismo Vehículo, entonces el IdV es el IdC instalado en el Vehículo que funge como el controlador principal o conciliador principal para la apropiada comunicación entre el Vehículo y el Internet, y el cual su Propietario (KIAM), o Entidad Responsable del Dispositivo (KERD ó KDRE) ha provisto consentimiento y PdC de los Términos, Condiciones y Políticas de Privacidad de sus servicios. Para que un vehículo pueda ser considerado como tal para una instalación y funcionamiento del IdA, este debe ser un dispositivo o artefacto que cumpla con las leyes, legislaciones, regulaciones, términos, condiciones, políticas de privacidad, acuerdos corporativos y civiles, de derechos humanos y consideraciones de sentido común de los Estados en los que del mismo exista pretención de ser utilizado y de funcionar |
| IoTv | Internet de las Televisiones (ó IdTv) | El IdTv es un dispositivo que es embebido o es parte de un Dispositivo de Televisión ó Televisor; y el cual las personas que la estén utilizando o "viendo", mientras el mismo muestre contenido y esté conectado a Internet o a "La Red" en ese mismo tiempo, son sujetos a los términos, condiciones y políticas de privacidad especialmente creadas para esa misma interacción y que no son invasivos ni violan los derechos humanos |
| IoMD | Internet de los Dispositivos Médicos (IdDM) | El IdMD es un dispositivo IdC que es embebido o instalado en el LNCMD y que cumple con todas las regulaciones y MRQ necesarios para ser un LKMD que funciona dentro del ecosistema +LKNC$, y que por definici'on debe incluir un IoMD. Todos los LKMD deben incluir un IoMD para ser considerados como tal |
| LNCMD (LNKMD) | Dispositivo Médico `KClassifiedCertified` de Lucky Network | El `LNCMD`, también llamado `LNKMD` es un dispositivo de grado `K` certificado y seguro que procesa, guarda, transmite y recibe `Datos Médicos`. El procesamiento, almacenamiento, transmisión y recepción de datos médicos también es conocido en el ecosistema +LKNC$ como `"MedKData"`. Todos los datos `MedKData` deben cumplir con los MRQ apropiados para ser ello, y deben cumplir con `HIPAA`, `PCI`, y las actualmente `"más estrictas"` regulaciones a "`nivel mundial`" sobre el manejo de datos médicos. LNSCT y LNSCTVA siempre van a trabajar en esfuerzos para brindar los más altos estándares de seguridad del `protocolo` `MedKData` |
| MedKData | Protocolo `MedKData` | TÉRMINO CLAIFICADO QUE CONSISTE EN UN PROTOCOLO SEGURO Y CLASIFICADO DE TRANSMISIÓN DE DATOS |
| ToV | Transferencia de Valor (ó TdV) | TÉRMINO CLASIFICADO QUE CONSISTE EN LA TRANSMISIÓN O TX O RX DE VALORES O EL TAMBIÉN CLASIFICADO ÁTOMO K |
| UoV | Unidad de Valor (ó UdV) | El UdV es la unidad más atómica del ecosistema +LKNC$ que puede ser utilizado para la Transferencia de Valor. La UdV no puede ser cambiado o modificado en un ecosistema +LKNC$. Si un cambio radical como remplazar el UdV original ocurre, entonces todo un nuevo ecosistema +LKNC$ debería ser habilitado para que ese nuevo UdV pueda funcionar, y entonces el anterior +LKNC$ en el que el anterior UdV había sido utilizado debería ser gradualmente y en óptimas condiciones migrado hacia el nuevo ecosistema +LKNC$ a través de uno o mas LKNCTEs para su más saludable transición |
| CoToV | Contrato de Transferencia de Valor (CdTdV) | EL CONTRATO DE TRANSFERENCIA DE VALOR ES UN TÉRMINO CLASIFICADO QUE CONSISTE EN UN CONTRATO "K" O "CONTRATO INTELIGENTE" QUE A SU VEZ ES UN CONJUNTO DE TÉRMINOS, CONDICIONES, POLÍTICAS DE PRIVACIDAD, ACUERDO DE ACEPTACIÓN Y PRUEBA DE CONOCIMIENTO PARA QUE SE EJERZA UNA TRANSFERENCIA DE VALOR DETERMINADA |
| ToToV | Marca de Tiempo de una Transferencia de Valor (MTdTdV) | |
| KSTATE | El Estado K | Todos y cada uno de los Dispositivos que initeractúan con +LKNC$, ya sea que estén habilitados para transaccionar o sólo para leer, existen y están en uno y sólamente uno de los Estado que son parte dl conjunto de Estados de el Ecosistema de Estados Finitos de +LKNC$ |
