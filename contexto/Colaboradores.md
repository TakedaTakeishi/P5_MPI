# Contributors visibles en GitHub

| Usuario | Nombre visible | Observación |
|---|---|---|
| CristianIDL | KiranFaux | Aparece como contributor con nombre visible adicional |
| TakedaTakeishi | Takeishi | Aparece como contributor con nombre visible adicional |
| hakoluna |  | Solo aparece el usuario |
| Frem10 |  | Solo aparece el usuario |

## Mapeo de trabajo rápido

Para agregar o revisar colaboradores con GitHub CLI, usa el usuario de GitHub tal como aparece en la lista anterior.

    gh api -X PUT repos/TakedaTakeishi/p6-cisco-packet-tracer/collaborators/USERNAME -f permission=push

Para revisar los colaboradores actuales:

    gh api repos/TakedaTakeishi/repo/collaborators

## Nota de verificación

GitHub puede mostrar dos textos por persona: el usuario y, si existe, el nombre visible del perfil. Para automatizar invitaciones o permisos, el dato que importa es el usuario; el nombre visible solo sirve como referencia humana.