# Guía de Seguridad de la Información, Azure Identity Manager y Microsoft Entra ID

Este documento proporciona una visión general sobre la seguridad de la información y el uso de herramientas de gestión de identidades en Azure, como Azure Identity Manager y Microsoft Entra ID.

## Contenido
- [Seguridad de la Información](#seguridad-de-la-información)
  - [Concepto](#concepto)
  - [Vulnerabilidades](#vulnerabilidades)
  - [Políticas de Seguridad de la Información (PSI)](#políticas-de-seguridad-de-la-información-psi)
- [Azure Identity Manager](#azure-identity-manager)
  - [Concepto](#concepto-1)
  - [Gestión de IAM](#gestión-de-iam)
  - [IAM a nivel de Grupo de Recursos](#iam-a-nivel-de-grupo-de-recursos)
- [Microsoft Entra ID](#microsoft-entra-id)
  - [Concepto](#concepto-2)
  - [Usuarios](#usuarios)
  - [Grupos](#grupos)

## Seguridad de la Información

### Concepto

La seguridad de la información es fundamental en el ámbito de TI, ya que la información es el activo más valioso tanto para empresas como para individuos. Comprender cómo se desarrollan los ataques que pueden comprometer nuestros sistemas es esencial para proteger la **Confidencialidad**, **Integridad** y **Disponibilidad** de la información.

Un ataque generalmente comienza con una amenaza, como un hacker o un bot que explota una vulnerabilidad en el sistema. Esta vulnerabilidad puede derivar en un riesgo que, de no ser gestionado, se convierte en un incidente que afecta a los pilares de la seguridad de la información.

Ejemplos de ataques a la Triada CIA:
- **Disponibilidad**: DoS (Denegación de Servicio)
- **Integridad**: Robo de sesiones, elevación de privilegios
- **Confidencialidad**: Phishing, robo de contraseñas, Shoulder Surfing

Para evitar que estos ataques ocurran, es crucial seguir un conjunto de pasos básicos:
1. **Identificar los activos de la organización**.
2. **Identificar las vulnerabilidades de los activos**.
3. **Realizar un análisis de riesgos**.
4. **Implementar acciones correctivas**.

### Vulnerabilidades

Identificar las vulnerabilidades de los activos es esencial para proteger a la organización contra ataques y fallos. Para ello, se deben considerar las siguientes acciones:

1. **Análisis de riesgos informáticos**: Consiste en identificar activos y vulnerabilidades para tomar medidas que permitan mitigar, eliminar, asumir o transferir los riesgos detectados.

2. **Estudio de la importancia de los incidentes**.
3. **Implementación de salvaguardas y medidas de seguridad**.
4. **Uso de herramientas criptográficas**: Emplear algoritmos de cifrado para proteger la información.

### Políticas de Seguridad de la Información (PSI)

Una PSI es un conjunto de normas y procedimientos que regulan la seguridad de los sistemas de información en una empresa. Se basa en cuatro etapas:

1. **Definición de necesidades**.
2. **Implementación**.
3. **Auditoría de seguridad**.
4. **Definición de acciones frente a desastres**.

La norma **ISO 27001** establece cómo implementar un Sistema de Gestión de Seguridad de la Información (SGSI) usando el ciclo de Deming (Plan, Do, Check, Act).

## Azure Identity Manager

### Concepto

Azure Identity Manager permite gestionar roles, usuarios y permisos de acceso a recursos en Azure, facilitando la administración de identidades y accesos.

- **Usuario**: Representa a una persona con credenciales para acceder y gestionar recursos.
- **Grupo**: Un conjunto de usuarios con permisos comunes.
- **Roles**: Azure ofrece roles predefinidos y la opción de crear roles personalizados que agrupan permisos específicos.

### Gestión de IAM

En Azure, el IAM se puede configurar a tres niveles:
- **Suscripción**: Nivel más macro, generalmente no recomendado para definir IAM.
- **Grupo de recursos**: Permite controlar permisos a un grupo de recursos específicos.
- **Recurso**: Nivel más específico, ideal para aplicar el principio de mínimo privilegio.

### IAM a nivel de Grupo de Recursos

En este nivel, se puede asignar roles a usuarios o grupos específicos, controlar niveles de acceso y definir roles personalizados con permisos específicos.

## Microsoft Entra ID

### Concepto

Microsoft Entra ID es un servicio de Azure que gestiona grupos y usuarios, y se integra con otros servicios como Office365. Anteriormente conocido como Azure Active Directory.

### Usuarios

Para crear un usuario en Microsoft Entra ID, se debe especificar el nombre principal, dominio, nombre para mostrar, contraseña y rol asignado.

### Grupos

Los grupos se crean definiendo el tipo de grupo, nombre y descripción, lo que permite gestionar permisos de manera más eficiente.

