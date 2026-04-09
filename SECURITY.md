<p align="center">
  <img src="https://img.shields.io/badge/◈_SECURITY-4C1D95?style=for-the-badge" alt="Security"/>
</p>

<p align="center">
  <sub>Politica de seguridad de <strong>K-Forge</strong>.</sub>
</p>

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

<p align="center">
  <sub>Gracias por ayudarnos a mantener K-Forge seguro.</sub>
</p>
