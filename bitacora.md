# configuracion global vs local
-Global: valores que aplican a todos los repositorios del usuario en esa máquina (por ejemplo: nombre, email, editor por defecto).
-Local (por repositorio): valores específicos para ese repositorio (por ejemplo: remote, hooks, configuración especial).
## Cuándo usar cada una
-Usa global para identidad personal y preferencias generales.
-Usa local cuando colabores usando otro nombre/email, cuando un repo requiera diferente editor, o para ajustar settings que no quieres que afecten otros proyectos.
# Diferencias entre git reset y git revert
## git reset: 
Modifica la referencia de la rama: mueve HEAD y la rama actual a otro commit.
-tipos:
-soft
-mixed 
-hard
## git revert:
Crea un nuevo commit que revierte los cambios introducidos por un commit anterior.
- Seguro en repositorios compartidos: no reescribe el historial, añade un commit que "deshace" a uno anterior.
- Útil cuando quieres deshacer algo que ya fue push a remoto sin romper historial.
# Explicación del Fork y detalles del Pull Request
## Fork
Es una copia independiente de un repositorio.
- Uso típico: colaborar con proyectos en los que no tienes permisos de push directo (proyectos open-source).
## Pull Request (PR)
Es la petición formal para que los cambios de tu rama (en tu fork o en una rama del mismo repo) sean revisados e integrados en otra rama (normalmente main o develop) del repositorio objetivo.
