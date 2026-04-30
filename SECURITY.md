<img src="./assets/banner-security.svg" width="100%" alt="Security — K-Forge"/>

<br/>

## ◈ Reportar una vulnerabilidad

Si descubres una vulnerabilidad de seguridad en cualquier proyecto de K-Forge:

**No abras un Issue publico.**

Envia un correo a:

**kforge.dev@gmail.com** — asunto: *Vulnerabilidad de seguridad*

Incluye:

- Descripcion de la vulnerabilidad y su impacto potencial.
- Pasos para reproducirla.
- Componente afectado (backend API, frontend, base de datos, autenticacion, etc.).
- Logs, capturas de pantalla o prueba de concepto relevantes.
- Solucion sugerida (si la tienes).

<br/>

## ◈ Que constituye un problema de seguridad

Los siguientes casos **deben** reportarse por el canal descrito arriba:

- Bypass de autenticacion o autorizacion
- Inyeccion SQL, XSS, CSRF u otros ataques de inyeccion
- Exposicion de datos sensibles (credenciales, informacion personal)
- Insecure Direct Object References (IDOR)
- Server-Side Request Forgery (SSRF)
- Endpoints expuestos que deberian requerir autenticacion
- Credenciales o secretos hardcodeados en el codigo
- Vulnerabilidades en dependencias con exploits conocidos

Los siguientes **no** se consideran problemas de seguridad:

- Bugs sin impacto de seguridad
- Solicitudes de funcionalidades o problemas de usabilidad
- Vulnerabilidades en dependencias sin exploit demostrado contra el proyecto

<br/>

## ◈ Divulgacion responsable

- **No** divulgues publicamente la vulnerabilidad antes de que sea resuelta.
- **No** accedas, modifiques ni elimines datos de otros usuarios durante tu investigacion.
- **No** realices acciones que puedan degradar el servicio.
- Actua de buena fe para evitar violaciones de privacidad, destruccion de datos e interrupciones del servicio.

<br/>

## ◈ Tiempo de respuesta

| Etapa | Plazo |
|---|---|
| Confirmacion de recepcion | 48 horas |
| Evaluacion inicial | 7 dias |
| Resolucion / Parche | Segun severidad |

<br/>

## ◈ Practicas de seguridad

- **Nunca** subas credenciales, tokens o API keys al codigo.
- Usa variables de entorno para datos sensibles.
- Manten las dependencias actualizadas.
- Revisa permisos de acceso periodicamente.

<br/>

## ◈ Versiones soportadas

Las actualizaciones de seguridad se aplican a la ultima version en la rama `main`. No mantenemos parches de seguridad para versiones anteriores.

| Rama | Soportada |
|---|---|
| `main` | Si |
| Otras | No |

<br/>

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=100&color=0:000000,100:8B5CF6&section=footer" width="100%"/>
  <br/>
  <a href="https://github.com/K-Forge">
    <img src="https://img.shields.io/badge/GitHub-K--Forge-111827?style=for-the-badge&logo=github&logoColor=8B5CF6" alt="GitHub K-Forge"/>
  </a>
  &nbsp;
  <a href="https://kforge.vercel.app">
    <img src="https://img.shields.io/badge/Web-kforge.vercel.app-8B5CF6?style=for-the-badge&logo=vercel&logoColor=white" alt="Web"/>
  </a>
  &nbsp;
  <a href="mailto:kforge.dev@gmail.com">
    <img src="https://img.shields.io/badge/Email-kforge.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
  <br/><br/>
  <sub>Gracias por ayudarnos a mantener K-Forge seguro.</sub>
  <br/><br/>
  <a href="#top">
    <img src="https://img.shields.io/badge/%E2%96%B2_Volver_arriba-8B5CF6?style=flat-square" alt="Volver arriba"/>
  </a>
</div>
