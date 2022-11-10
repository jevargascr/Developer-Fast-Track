# Lab. 1 - Aprovisionamiento de recursos 

En esta etapa, se aprovisionarán recursos dentro de OCI utilizando Terraform con el servicio **Resource Manager**!

- 🌀 [Página oficial de Resource Manager](https://www.oracle.com/pe/devops/resource-manager/)
- 🧾 [Documentaçión de Resource Manager](https://docs.oracle.com/en-us/iaas/Content/ResourceManager/home.htm)

Los recursos a aprovicionar serán:
- OKE
- Artifact Registry
- Container Registry
- OCI DevOps
- APM
- API Gateway
- Streaming
- Object Storage
- Functions

Junto con recursos de red y administración como:
- VCN
- Subnets
- Dynamic Groups
- Policies
- Compartments

- - -

# Requisitos Previos - creación de compartments
Como requisito previo, es una buena idea crear un compartment aislado para poder agrupar nuestros recursos.

1. Para hacer esto, inicie sesión o [login](https://www.oracle.com/cloud/sign-in.html) en su cuenta de OCI.
2. Desde el menú ☰ acceder: **Identity & Security** → **Identity** → **Compartments**.


![](./Imágenes/IMG00_1.png)

3. En la nueva ventana, haga clic en Crear compartment.
 
![](./Imágenes/IMG00_2.png)

4. Introduzca un nombre para el compartment y también una descripción. Una vez hecho esto, haga clic en **Crear compartment**.
Ejemplo: 
   - ***Name:*** DevFT 
   - ***Description:*** Compartment para labs Developer Fast Track 

![](./Imágenes/IMG00_3.png)

**¡¡¡Excelente!!!**  💯 ¡Ahora podemos comenzar con nuestros pasos de laboratorio!

- - -

## Paso 1 - Descarga el repositorio

Como primer paso, debemos descargar el archivo (zip) desde el repositorio de github.

1. Para hacer esto, vaya al [repositorio](https://github.com/jevargascr/Terraform-Developer-Fast-Track) y haga clic en **Descargar ZIP**.

![](./Imágenes/IMG01_2.png)



- - -

## Paso 2: Cargar terraform en Resource Manager

1. Inicie sesión en [login](https://www.oracle.com/cloud/sign-in.html) en su cuenta de OCI.
2. Desde el menú ☰ acceder a: **Developer Services** → **Resource Manager** → **Stacks**.

![](./Imágenes/IMG02.png)

3. En esta nueva ventana, acceda al compartment creado anteriormente y haga clic en **Create Stack**.

![](./Imágenes/IMG03.png)

4. Seleccione la opción "Zip file", haga clic en "browse" y arrastre el archivo (.zip), que contiene los archivos .tf. Resource Manager completará todos los campos por defecto.

![](./Imágenes/IMG04.png)

5. Haga clic en **Next**, para que podamos configurar algunos parámetros sobre los recursos a provisionar.

6. En esta nueva pantalla, recuerda seleccionar el compartment creado anteriormente y haz clic en **Mostrar opciones avanzadas**.

![](./Imágenes/IMG05.png)

7. Antes de continuar, recuerda seleccionar la versión "v1.23.4" en la opción **Versión de Kubernetes**.

![](./Imágenes/IMG06.png)

8. Haga clic en **Siguiente**.

9. Una vez creada nuestro stack, haga clic en **Apply** y confirme la acción.

![](./Imágenes/IMG07.png)

10. El aprovisionamiento de recursos debería tomar alrededor de 25 minutos.

11. ¡Después de finalizar con éxito la aplicación, podemos verificar el aprovisionamiento de nuestros recursos!

### ✔ ¡¡¡Entornos aprovisionados con éxito!!! ¡Has aprovisionado recursos usando Terraform en OCI! 🚀

COMPLETASTE EXITOSAMENTE EL LABORATORIO N#1 !! 💯✅

<a href="https://github.com/jevargascr/Developer-Fast-Track">Regresar</a>





