REPORTE DE LABORATORIO 04 (INDIVIDUAL)
Curso:

Control de Versiones para Desarrollo Full Stack

Docente:

Ing. Luis Flores

1. Identificación del Desarrollador

Nombre Completo: Carlos mathias Gaitan Urbina

Usuario de GitHub: @DevMathus

Fecha de Entrega: 29/05/2026

2. Hito 1: Implementación de Seguridad Perimetral (.gitignore)
1. Estructura del archivo .gitignore consolidada localmente:
# Secretos locales de ApexPay
.env
.env.local

# Temporales de compilacion y dependencias generadas por el script
node_modules/
dist/
*.log
2. Prueba de Inmunidad de Credenciales
On branch main
nothing to commit, working tree clean
3. Hito 2: Resolución de la Colisión de Interfaces (Merge Conflict Solo)
1. Discrepancia Técnica Inicial

Respuesta:

El rechazo ocurrió porque existían cambios nuevos en el repositorio remoto realizados directamente desde GitHub mientras el entorno local estaba desactualizado. Git detectó diferencias entre ambos historiales y rechazó el push para evitar sobrescribir cambios remotos. Durante el pull, Git insertó marcadores de conflicto como <<<<<<<, ======= y >>>>>>> dentro del archivo README.md.

2. Resultado Consolidado de Consenso
# apexpay-dashboard
Tema del proyecto: Hibrido
4. Hito 3: Mitigación de Exposición de Infraestructura (git revert)
1. Histórico del Historial Clínico de Producción (Git Log)


2bbe54f (HEAD -> main, origin/main, origin/HEAD) Merge pull request #2 from D
evMathus/feat/footer
4a198e2 Merge pull request #1 from DevMathus/feat/menu-principal
e2e5cea (origin/feat/footer, feat/footer) fix: incorporar politicas de privac
idad en footer
da37342 (origin/feat/menu-principal, feat/menu-principal) fix: ajustar menu d
e navegacion segun auditoria interna
72e6234 feat: estructurar pie de pagina corporativo
6df16a9 feat: estructurar el menu principal de navegacion
6713856 Revert "feat: modulo de pruebas de red expuestas"
d9678f1 feat: modulo de pruebas de red expuestas
5d31193 merge: conciliar conflicto de temas en solitario
af618ec feat: configurar tema claro localmente
94838d4 "feat : configurar tema oscuro de forma remota"
4a04199 chore: inicializar codigo base de ApexPay y configurar gitignore
059537d Initial commit




2. Análisis de Resiliencia Organizacional

Respuesta:

El comando git reset --hard se considera peligroso en ramas públicas porque modifica el historial compartido del repositorio remoto, provocando desincronización entre los integrantes del equipo y posible pérdida de commits importantes.

Por otro lado, git revert mantiene intacto el historial original y genera un nuevo commit que revierte los cambios problemáticos. Esto permite conservar trazabilidad, estabilidad y transparencia dentro del flujo colaborativo de desarrollo.

5. Hito 4: Enlaces de Gobernanza y Solicitudes de Integración
Pull Request de Menú (feat/menu-principal)

https://github.com/DevMathus/apexpay-dashboard/pull/1

Pull Request de Footer (feat/footer)

https://github.com/DevMathus/apexpay-dashboard/pull/2