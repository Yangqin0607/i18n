# globalShortcut

> Detecta los eventos del teclado cuando la aplicación no tiene el enfoque en el teclado.

Process: [Main](../glossary.md#main-process)

El módulo `globalShortcut` puede registrar o quitar un atajo del teclado global con el sistema operativo para que se puedan personalizar las operaciones para varios atajos.

**Nota:** El atajo es global; funcionará incluso si la aplicación no tiene enfocado el teclado. No se debe utilizar este módulo hasta que el evento `ready` del módulo de la aplicación no se emita.

```javascript
const {app, globalShortcut} = require('electron')

app.on('ready', () => {
  // Regista un grabador de atajo 'CommandOrControl+X'.
  const ret = globalShortcut.register('CommandOrControl+X', () => {
    console.log('CommandOrControl+X is pressed')
  })

  if (!ret) {
    console.log('registration failed')
  }

  // Revisa si un atajo está registrado.
  console.log(globalShortcut.isRegistered('CommandOrControl+X'))
})

app.on('will-quit', () => {
  // Desregistra un atajo.
  globalShortcut.unregister('CommandOrControl+X')

  // Desregistra todos los atajos.
  globalShortcut.unregisterAll()
})
```

## Métodos

El módulo `globalShortcut` tiene los siguientes métodos:

### `globalShortcut.register(accelerator, callback)`

* `accelerator` [Accelerator](accelerator.md)
* `callback` Función

Registra un atajo global de`accelerator`. El `callback` es llamado cuando el atajo registrado es presionado por el usuario.

Cuando el acelerador ha sido tomado por otras aplicaciones, esta llamada fallará silenciosamente. Este comportamiento está diseñado por los sistemas operativos, debido a que no desean que las aplicaciones tengan conflictos por los atajos globales.

### `globalShortcut.isRegistered(accelerator)`

* `accelerator` [Accelerator](accelerator.md)

Devuelve `Boolean` - Si esta aplicación tiene registrado `accelerator`.

Cuando el acelerador ha sido tomado por otras aplicaciones, esta llamada aun devolverá `false`. Este comportamiento está diseñado por los sistemas operativos, debido a que no desean que las aplicaciones tengan conflictos por los atajos globales.

### `globalShortcut.unregister(accelerator)`

* `accelerator` [Accelerator](accelerator.md)

Anula el registro del atajo del `accelerator`.

### `globalShortcut.unregisterAll()`

Anula el registro todos los atajos globales.